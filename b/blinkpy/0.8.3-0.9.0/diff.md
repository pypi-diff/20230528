# Comparing `tmp/blinkpy-0.8.3-py3-none-any.whl.zip` & `tmp/blinkpy-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 9555 bytes, number of entries: 9
+Zip file size: 12843 bytes, number of entries: 12
 -rw-rw-r--  2.0 unx       29 b- defN 18-Sep-23 15:45 blinkpy/__init__.py
--rw-rw-r--  2.0 unx    21090 b- defN 18-Sep-25 02:32 blinkpy/blinkpy.py
+-rw-rw-r--  2.0 unx     6999 b- defN 18-Sep-28 01:46 blinkpy/blinkpy.py
+-rw-rw-r--  2.0 unx     7740 b- defN 18-Sep-28 01:46 blinkpy/camera.py
+-rw-rw-r--  2.0 unx     8661 b- defN 18-Sep-28 01:46 blinkpy/sync_module.py
 -rw-rw-r--  2.0 unx       47 b- defN 18-Sep-23 15:45 blinkpy/helpers/__init__.py
--rw-rw-r--  2.0 unx     1660 b- defN 18-Sep-25 02:32 blinkpy/helpers/constants.py
+-rw-rw-r--  2.0 unx     1660 b- defN 18-Sep-28 01:46 blinkpy/helpers/constants.py
 -rw-rw-r--  2.0 unx      409 b- defN 18-Sep-23 15:45 blinkpy/helpers/errors.py
--rw-rw-r--  2.0 unx        8 b- defN 18-Sep-25 02:32 blinkpy-0.8.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx       92 b- defN 18-Sep-25 02:32 blinkpy-0.8.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx     3779 b- defN 18-Sep-25 02:32 blinkpy-0.8.3.dist-info/METADATA
--rw-rw-r--  2.0 unx      704 b- defN 18-Sep-25 02:32 blinkpy-0.8.3.dist-info/RECORD
-9 files, 27818 bytes uncompressed, 8359 bytes compressed:  70.0%
+-rw-rw-r--  2.0 unx     2991 b- defN 18-Sep-28 01:46 blinkpy/helpers/util.py
+-rw-rw-r--  2.0 unx        8 b- defN 18-Sep-28 01:52 blinkpy-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx       92 b- defN 18-Sep-28 01:52 blinkpy-0.9.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     5227 b- defN 18-Sep-28 01:52 blinkpy-0.9.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx      939 b- defN 18-Sep-28 01:52 blinkpy-0.9.0.dist-info/RECORD
+12 files, 34802 bytes uncompressed, 11295 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
 Filename: blinkpy/__init__.py
 Comment: 
 
 Filename: blinkpy/blinkpy.py
 Comment: 
 
+Filename: blinkpy/camera.py
+Comment: 
+
+Filename: blinkpy/sync_module.py
+Comment: 
+
 Filename: blinkpy/helpers/__init__.py
 Comment: 
 
 Filename: blinkpy/helpers/constants.py
 Comment: 
 
 Filename: blinkpy/helpers/errors.py
 Comment: 
 
-Filename: blinkpy-0.8.3.dist-info/top_level.txt
+Filename: blinkpy/helpers/util.py
+Comment: 
+
+Filename: blinkpy-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: blinkpy-0.8.3.dist-info/WHEEL
+Filename: blinkpy-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: blinkpy-0.8.3.dist-info/METADATA
+Filename: blinkpy-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: blinkpy-0.8.3.dist-info/RECORD
+Filename: blinkpy-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## blinkpy/blinkpy.py

```diff
@@ -1,487 +1,94 @@
-#!/usr/bin/python
+
 # -*- coding: utf-8 -*-
 """
 blinkpy by Kevin Fronczak - A Blink camera Python library.
 
 https://github.com/fronzbot/blinkpy
 Original protocol hacking by MattTW :
 https://github.com/MattTW/BlinkMonitorProtocol
 Published under the MIT license - See LICENSE file for more details.
 "Blink Wire-Free HS Home Monitoring & Alert Systems" is a trademark
 owned by Immedia Inc., see www.blinkforhome.com for more information.
 I am in no way affiliated with Blink, nor Immedia Inc.
 """
 
+import time
 import json
 import getpass
-from shutil import copyfileobj
 import logging
-import requests
-from requests.structures import CaseInsensitiveDict
 import blinkpy.helpers.errors as ERROR
+from blinkpy.sync_module import BlinkSyncModule
+from blinkpy.helpers.util import (
+    http_req, create_session, BlinkURLHandler,
+    BlinkException, BlinkAuthenticationException)
 from blinkpy.helpers.constants import (
-    BLINK_URL, LOGIN_URL, LOGIN_BACKUP_URL,
-    DEFAULT_URL, ONLINE
-)
-
-_LOGGER = logging.getLogger('blinkpy')
-
-MAX_CLIPS = 5
-
-
-def _attempt_reauthorization(blink):
-    """Attempt to refresh auth token and links."""
-    _LOGGER.debug("Auth token expired, attempting reauthorization.")
-    headers = blink.get_auth_token()
-    blink.set_links()
-    return headers
-
-
-def _request(blink, url='http://google.com', data=None, headers=None,
-             reqtype='get', stream=False, json_resp=True, is_retry=False):
-    """Perform server requests and check if reauthorization neccessary."""
-    if reqtype == 'post':
-        response = requests.post(url, headers=headers,
-                                 data=data)
-    elif reqtype == 'get':
-        response = requests.get(url, headers=headers,
-                                stream=stream)
-    else:
-        raise BlinkException(ERROR.REQUEST)
-
-    if json_resp and 'code' in response.json():
-        if is_retry:
-            raise BlinkAuthenticationException(
-                (response.json()['code'], response.json()['message']))
-        else:
-            headers = _attempt_reauthorization(blink)
-            return _request(blink, url=url, data=data, headers=headers,
-                            reqtype=reqtype, stream=stream,
-                            json_resp=json_resp, is_retry=True)
-    # pylint: disable=no-else-return
-    if json_resp:
-        return response.json()
-    else:
-        return response
-
-
-# pylint: disable=super-init-not-called
-class BlinkException(Exception):
-    """Class to throw general blink exception."""
-
-    def __init__(self, errcode):
-        """Initialize BlinkException."""
-        self.errid = errcode[0]
-        self.message = errcode[1]
-
-
-class BlinkAuthenticationException(BlinkException):
-    """Class to throw authentication exception."""
-
-    pass
-
-
-class BlinkURLHandler():
-    """Class that handles Blink URLS."""
-
-    def __init__(self, region_id):
-        """Initialize the urls."""
-        self.base_url = "https://rest.{}.{}".format(region_id, BLINK_URL)
-        self.home_url = "{}/homescreen".format(self.base_url)
-        self.event_url = "{}/events/network".format(self.base_url)
-        self.network_url = "{}/network".format(self.base_url)
-        self.networks_url = "{}/networks".format(self.base_url)
-        self.video_url = "{}/api/v2/videos".format(self.base_url)
-        _LOGGER.debug("Setting base url to %s.", self.base_url)
-
-
-class BlinkCamera():
-    """Class to initialize individual camera."""
-
-    def __init__(self, config, blink):
-        """Initiailize BlinkCamera."""
-        self.blink = blink
-        self.urls = self.blink.urls
-        self.id = str(config['device_id'])  # pylint: disable=invalid-name
-        self.name = config['name']
-        self._status = config['active']
-        self.thumbnail = "{}{}.jpg".format(self.urls.base_url,
-                                           config['thumbnail'])
-        self.clip = "{}{}".format(self.urls.base_url, config['video'])
-        self.temperature = config['temp']
-        self._battery_string = config['battery']
-        self.notifications = config['notifications']
-        self.motion = dict()
-        self.header = None
-        self.image_link = None
-        self.arm_link = None
-        self.region_id = config['region_id']
-        self.battery_voltage = -180
-        self.motion_detected = None
-        self.wifi_strength = None
-        self.camera_config = dict()
-        self.motion_enabled = None
-        self.last_record = list()
-
-    @property
-    def attributes(self):
-        """Return dictionary of all camera attributes."""
-        attributes = {
-            'name': self.name,
-            'device_id': self.id,
-            'status': self._status,
-            'armed': self.armed,
-            'temperature': self.temperature,
-            'temperature_c': self.temperature_c,
-            'battery': self.battery,
-            'thumbnail': self.thumbnail,
-            'video': self.clip,
-            'motion_enabled': self.motion_enabled,
-            'notifications': self.notifications,
-            'motion_detected': self.motion_detected,
-            'wifi_strength': self.wifi_strength,
-            'network_id': self.blink.network_id,
-            'last_record': self.last_record
-        }
-        return attributes
+    DEFAULT_URL, BLINK_URL, LOGIN_URL, LOGIN_BACKUP_URL)
 
-    @property
-    def status(self):
-        """Return camera status."""
-        return self._status
-
-    @property
-    def armed(self):
-        """Return camera arm status."""
-        return True if self._status == 'armed' else False
-
-    @property
-    def battery(self):
-        """Return battery level as percentage."""
-        return round(self.battery_voltage / 180 * 100)
+REFRESH_RATE = 30
 
-    @property
-    def battery_string(self):
-        """Return string indicating battery status."""
-        status = "Unknown"
-        if self._battery_string > 1 and self._battery_string <= 3:
-            status = "OK"
-        elif self._battery_string >= 0:
-            status = "Low"
-        return status
-
-    @property
-    def temperature_c(self):
-        """Return temperature in celcius."""
-        return round((self.temperature - 32) / 9.0 * 5.0, 1)
-
-    def snap_picture(self):
-        """Take a picture with camera to create a new thumbnail."""
-        _request(self.blink, url=self.image_link,
-                 headers=self.header, reqtype='post')
-
-    def set_motion_detect(self, enable):
-        """Set motion detection."""
-        url = self.arm_link
-        if enable:
-            _request(self.blink, url=url + 'enable',
-                     headers=self.header, reqtype='post')
-        else:
-            _request(self.blink, url=url + 'disable',
-                     headers=self.header, reqtype='post')
-
-    def update(self, values):
-        """Update camera information."""
-        self.name = values['name']
-        self._status = values['active']
-        self.clip = "{}{}".format(
-            self.urls.base_url, values['video'])
-        self.thumbnail = "{}{}.jpg".format(
-            self.urls.base_url, values['thumbnail'])
-        self._battery_string = values['battery']
-        self.notifications = values['notifications']
-
-        try:
-            cfg = self.blink.camera_config_request(self.id)
-            self.camera_config = cfg
-        except requests.exceptions.RequestException as err:
-            _LOGGER.warning("Could not get config for %s with id %s",
-                            self.name, self.id)
-            _LOGGER.warning("Exception raised: %s", err)
-
-        try:
-            self.battery_voltage = cfg['camera'][0]['battery_voltage']
-            self.motion_enabled = cfg['camera'][0]['motion_alert']
-            self.wifi_strength = cfg['camera'][0]['wifi_strength']
-            self.temperature = cfg['camera'][0]['temperature']
-        except KeyError:
-            _LOGGER.warning("Problem extracting config for camera %s",
-                            self.name)
-
-        # Check if the most recent clip is included in the last_record list
-        # and that the last_record list is populated
-        try:
-            records = sorted(self.blink.record_dates[self.name])
-            new_clip = records.pop()
-            if new_clip not in self.last_record and self.last_record:
-                self.motion_detected = True
-                self.last_record.insert(0, new_clip)
-                if len(self.last_record) > MAX_CLIPS:
-                    self.last_record.pop()
-            elif not self.last_record:
-                self.last_record.insert(0, new_clip)
-                self.motion_detected = False
-            else:
-                self.motion_detected = False
-        except KeyError:
-            _LOGGER.warning("Could not extract clip info from camera %s",
-                            self.name)
-
-    def image_refresh(self):
-        """Refresh current thumbnail."""
-        url = self.urls.home_url
-        response = _request(self.blink, url=url, headers=self.header,
-                            reqtype='get')['devices']
-        for element in response:
-            try:
-                if str(element['device_id']) == self.id:
-                    self.thumbnail = (
-                        "{}{}.jpg".format(
-                            self.urls.base_url, element['thumbnail'])
-                    )
-                    return self.thumbnail
-            except KeyError:
-                pass
-        return None
-
-    def image_to_file(self, path):
-        """Write image to file."""
-        _LOGGER.debug("Writing image from %s to %s", self.name, path)
-        thumb = self.image_refresh()
-        if not thumb:
-            thumb = self.thumbnail
-        response = _request(self.blink, url=thumb, headers=self.header,
-                            reqtype='get', stream=True, json_resp=False)
-        if response.status_code == 200:
-            with open(path, 'wb') as imgfile:
-                copyfileobj(response.raw, imgfile)
-        else:
-            print(response)
-
-    def video_to_file(self, path):
-        """Write video to file."""
-        _LOGGER.debug("Writing video from %s to %s", self.name, path)
-        response = _request(self.blink, url=self.clip, headers=self.header,
-                            reqtype='get', stream=True, json_resp=False)
-        with open(path, 'wb') as vidfile:
-            copyfileobj(response.raw, vidfile)
+_LOGGER = logging.getLogger('blinkpy')
 
 
 class Blink():
-    """Class to initialize communication and sync module."""
+    """Class to initialize communication."""
+
+    def __init__(self, username=None, password=None,
+                 refresh_rate=REFRESH_RATE):
+        """
+        Initialize Blink system.
 
-    def __init__(self, username=None, password=None):
-        """Initialize Blink system."""
+        :param username: Blink username (usually email address)
+        :param password: Blink password
+        :param refresh_rate: Refresh rate of blink information.
+                             Defaults to 15 (seconds)
+        """
         self._username = username
         self._password = password
         self._token = None
         self._auth_header = None
+        self._host = None
+        self._events = []
+        self._last_summary = None
+        self._last_events = None
         self.network_id = None
         self.account_id = None
+        self.urls = None
+        self.sync = None
         self.region = None
         self.region_id = None
-        self._host = None
-        self._events = []
-        self.cameras = CaseInsensitiveDict({})
-        self._idlookup = {}
-        self.urls = None
-        self._video_count = 0
-        self._all_videos = {}
-        self._summary = None
-        self.record_dates = dict()
-
-    @property
-    def camera_thumbs(self):
-        """Return camera thumbnails."""
-        self.refresh()
-        data = {}
-        for name, camera in self.cameras.items():
-            data[name] = camera.thumbnail
-
-        return data
-
-    @property
-    def id_table(self):
-        """Return id/camera pairs."""
-        return self._idlookup
-
-    @property
-    def video_count(self):
-        """Return number of videos on server."""
-        url = "{}/count".format(self.urls.video_url)
-        headers = self._auth_header
-        self._video_count = _request(self, url=url, headers=headers,
-                                     reqtype='get')['count']
-        return self._video_count
+        self.last_refresh = None
+        self.refresh_rate = refresh_rate
+        self.session = None
+        self._login_url = LOGIN_URL
 
     @property
     def events(self):
         """Get all events on server."""
         return self._events
 
-    @property
-    def online(self):
-        """Return boolean system online status."""
-        return ONLINE[self._status_request()['syncmodule']['status']]
-
-    @property
-    def videos(self):
-        """Return video list."""
-        return self._all_videos
-
-    @property
-    def summary(self):
-        """Get a full summary of device information."""
-        return self._summary
-
-    @property
-    def arm(self):
-        """Return status of sync module: armed/disarmed."""
-        return self.summary['network']['armed']
-
-    @arm.setter
-    def arm(self, value):
-        """Arm or disarm system."""
-        if value:
-            value_to_append = 'arm'
-        else:
-            value_to_append = 'disarm'
-        url = "{}/{}/{}".format(self.urls.network_url,
-                                self.network_id,
-                                value_to_append)
-        _request(self, url=url, headers=self._auth_header, reqtype='post')
-
-    def refresh(self):
-        """Get all blink cameras and pulls their most recent status."""
-        _LOGGER.debug("Attempting refresh of cameras.")
-        self._summary = self._summary_request()
-        self._events = self._events_request()
-        response = self.summary['devices']
-        self.get_videos()
-        for name in self.cameras:
-            camera = self.cameras[name]
-            for element in response:
-                try:
-                    if str(element['device_id']) == camera.id:
-                        element['video'] = self.videos[name][0]['clip']
-                        element['thumbnail'] = self.videos[name][0]['thumb']
-                        camera.update(element)
-                except KeyError:
-                    pass
-
-    def get_videos(self, start_page=0, end_page=1):
-        """Retrieve last recorded videos per camera."""
-        videos = list()
-        all_dates = dict()
-        for page_num in range(start_page, end_page + 1):
-            this_page = self._video_request(page_num)
-            if not this_page:
-                break
-            videos.append(this_page)
-
-        for page in videos:
-            _LOGGER.debug("Retrieved video page %s", page)
-            for entry in page:
-                camera_name = entry['camera_name']
-                clip_addr = entry['address']
-                thumb_addr = entry['thumbnail']
-                clip_date = clip_addr.split('_')[-6:]
-                clip_date = '_'.join(clip_date)
-                clip_date = clip_date.split('.')[0]
-                if camera_name not in all_dates:
-                    all_dates[camera_name] = list()
-                all_dates[camera_name].append(clip_date)
-                try:
-                    self._all_videos[camera_name].append(
-                        {
-                            'clip': clip_addr,
-                            'thumb': thumb_addr,
-                        }
-                    )
-                except KeyError:
-                    self._all_videos[camera_name] = [
-                        {
-                            'clip': clip_addr,
-                            'thumb': thumb_addr,
-                        }
-                    ]
-        self.record_dates = all_dates
-
-    def get_cameras(self):
-        """Find and creates cameras."""
-        self._summary = self._summary_request()
-        response = self.summary['devices']
-        for element in response:
-            if ('device_type' in element and
-                    element['device_type'] == 'camera'):
-                # Add region to config
-                element['region_id'] = self.region_id
-                try:
-                    name = element['name']
-                    element['video'] = self.videos[name][0]['clip']
-                    element['thumbnail'] = self.videos[name][0]['thumb']
-                except KeyError:
-                    element['video'] = None
-                    element['thumbnail'] = None
-                device = BlinkCamera(element, self)
-                self.cameras[device.name] = device
-                self._idlookup[device.id] = device.name
-        self.refresh()
-
-    def set_links(self):
-        """Set access links and required headers for each camera in system."""
-        for name in self.cameras:
-            camera = self.cameras[name]
-            network_id_url = "{}/{}".format(self.urls.network_url,
-                                            self.network_id)
-            image_url = "{}/camera/{}/thumbnail".format(network_id_url,
-                                                        camera.id)
-            arm_url = "{}/camera/{}/".format(network_id_url,
-                                             camera.id)
-            camera.image_link = image_url
-            camera.arm_link = arm_url
-            camera.header = self._auth_header
-
-    def setup_system(self):
-        """Legacy method support."""
-        _LOGGER.warning(
-            ("Blink.setup_system() will be deprecated in future release. "
-             "Please use Blink.start() instead.")
-        )
-        self.start()
-
     def start(self):
         """
         Perform full system setup.
 
         Method logs in and sets auth token, urls, and ids for future requests.
         Essentially this is just a wrapper function for ease of use.
         """
         if self._username is None or self._password is None:
             self.login()
         else:
             self.get_auth_token()
 
         self.get_ids()
-        self.get_videos()
-        if self.video_count > 0:
-            self.get_cameras()
-        self.set_links()
-        self._events = self._events_request()
+        self.sync = BlinkSyncModule(self, self._auth_header)
+        self.sync.get_videos()
+        if self.sync.video_count > 0:
+            self.sync.get_cameras()
+        self.sync.set_links()
+        self._events = self.events_request()
 
     def login(self):
         """Prompt user for username and password."""
         self._username = input("Username:")
         self._password = getpass.getpass("Password:")
         if self.get_auth_token():
             _LOGGER.info("Login successful!")
@@ -499,26 +106,28 @@
         headers = {'Host': DEFAULT_URL,
                    'Content-Type': 'application/json'}
         data = json.dumps({
             "email": self._username,
             "password": self._password,
             "client_specifier": "iPhone 9.2 | 2.2 | 222"
         })
-        response = _request(self, url=LOGIN_URL, headers=headers,
+        self.session = create_session()
+        response = http_req(self, url=self._login_url, headers=headers,
                             data=data, json_resp=False, reqtype='post')
         if response.status_code == 200:
             response = response.json()
             (self.region_id, self.region), = response['region'].items()
         else:
             _LOGGER.debug(
                 ("Received response code %s "
                  "when authenticating, "
                  "trying new url"), response.status_code
             )
-            response = _request(self, url=LOGIN_BACKUP_URL, headers=headers,
+            self._login_url = LOGIN_BACKUP_URL
+            response = http_req(self, url=self._login_url, headers=headers,
                                 data=data, reqtype='post')
             self.region_id = 'piri'
             self.region = "UNKNOWN"
 
         self._host = "{}.{}".format(self.region_id, BLINK_URL)
         self._token = response['authtoken']['authtoken']
 
@@ -531,49 +140,58 @@
 
     def get_ids(self):
         """Set the network ID and Account ID."""
         response = self._network_request()
         self.network_id = str(response['networks'][0]['id'])
         self.account_id = str(response['networks'][0]['account_id'])
 
-    def _video_request(self, page=0):
-        """Perform a request for videos."""
-        url = "{}/page/{}".format(self.urls.video_url, page)
-        headers = self._auth_header
-        return _request(self, url=url, headers=headers, reqtype='get')
-
-    def _summary_request(self):
-        """Get blink summary."""
-        url = self.urls.home_url
-        headers = self._auth_header
-        if headers is None:
-            raise BlinkException(ERROR.AUTH_TOKEN)
-        return _request(self, url=url, headers=headers, reqtype='get')
-
     def _network_request(self):
         """Get network and account information."""
         url = self.urls.networks_url
         headers = self._auth_header
         if headers is None:
             raise BlinkException(ERROR.AUTH_TOKEN)
-        return _request(self, url=url, headers=headers, reqtype='get')
+        return http_req(self, url=url, headers=headers, reqtype='get')
 
-    def _events_request(self):
+    def events_request(self, skip_throttle=False):
         """Get events on server."""
         url = "{}/{}".format(self.urls.event_url, self.network_id)
         headers = self._auth_header
-        return _request(self, url=url, headers=headers, reqtype='get')
+        if self.check_if_ok_to_update() or skip_throttle:
+            self._last_events = http_req(self, url=url,
+                                         headers=headers,
+                                         reqtype='get')
+        return self._last_events
 
-    def _status_request(self):
-        """Get syncmodule status."""
-        url = "{}/{}/syncmodules".format(self.urls.network_url,
-                                         self.network_id)
+    def summary_request(self, skip_throttle=False):
+        """Get blink summary."""
+        url = self.urls.home_url
         headers = self._auth_header
-        return _request(self, url=url, headers=headers, reqtype='get')
+        if headers is None:
+            raise BlinkException(ERROR.AUTH_TOKEN)
+        if self.check_if_ok_to_update() or skip_throttle:
+            self._last_summary = http_req(
+                self, url=url, headers=headers, reqtype='get')
+        return self._last_summary
 
-    def camera_config_request(self, camera_id):
-        """Retrieve more info about Blink config."""
-        url = "{}/network/{}/camera/{}/config".format(self.urls.base_url,
-                                                      self.network_id,
-                                                      str(camera_id))
-        headers = self._auth_header
-        return _request(self, url=url, headers=headers, reqtype='get')
+    def refresh(self, force_cache=False):
+        """
+        Perform a system refresh.
+
+        :param force_cache: Force an update of the camera cache
+        """
+        if self.check_if_ok_to_update() or force_cache:
+            _LOGGER.debug("Attempting refresh of cameras.")
+            self._last_events = self.events_request(skip_throttle=True)
+            self._last_summary = self.summary_request(skip_throttle=True)
+            self.sync.refresh(force_cache=force_cache)
+
+    def check_if_ok_to_update(self):
+        """Check if it is ok to perform an http request."""
+        current_time = int(time.time())
+        last_refresh = self.last_refresh
+        if last_refresh is None:
+            last_refresh = 0
+        if current_time >= (last_refresh + self.refresh_rate):
+            self.last_refresh = current_time
+            return True
+        return False
```

## blinkpy/helpers/constants.py

```diff
@@ -1,14 +1,14 @@
 """Generates constants for use in blinkpy."""
 
 import os
 
 MAJOR_VERSION = 0
-MINOR_VERSION = 8
-PATCH_VERSION = 3
+MINOR_VERSION = 9
+PATCH_VERSION = 0
 
 __version__ = '{}.{}.{}'.format(MAJOR_VERSION, MINOR_VERSION, PATCH_VERSION)
 
 REQUIRED_PYTHON_VER = (3, 4, 2)
 
 PROJECT_NAME = 'blinkpy'
 PROJECT_PACKAGE_NAME = 'blinkpy'
```

## Comparing `blinkpy-0.8.3.dist-info/RECORD` & `blinkpy-0.9.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 blinkpy/__init__.py,sha256=o_u9nvwhMMDpoZWiB5upFSPCAS_CG0HxgqijkNXrGEo,29
-blinkpy/blinkpy.py,sha256=XA8F3O3R695th6zF2e709MqassFiuTGLUwREO0D9n4w,21090
+blinkpy/blinkpy.py,sha256=H4W0e3-sdI8CLtY0m0r_LqBvp-MwqHu5NtSCb-gRKpE,6999
+blinkpy/camera.py,sha256=5CHZ7v71owpULmfdsuMPTmLN5sBSQsSQLkyzM9jd4As,7740
+blinkpy/sync_module.py,sha256=G8lidZGK-nMh5vci3dRDn41bGkbXSy3-IABh8ZH-A8k,8661
 blinkpy/helpers/__init__.py,sha256=6U0cOJ-gmsKG07TKpkfDzkDaVFFXA6LaQh9jZ0YvRO8,47
-blinkpy/helpers/constants.py,sha256=-zBGzIRyuS7fDOXxOubeFONBdAJmGXYzQ_2-br_N3V0,1660
+blinkpy/helpers/constants.py,sha256=lDpTNRMGqy_0cmBVqnI_XTv2RD-B6X_BRHf-QAooKAw,1660
 blinkpy/helpers/errors.py,sha256=GufEl8IH2RoTNsFuSxcorc9eHPsJFkLqg1HAT2W8qUA,409
-blinkpy-0.8.3.dist-info/METADATA,sha256=ogOz2SXLKxGdl1XG-cZ_Kb0yyS-23FK5KO9qCzuUj4o,3779
-blinkpy-0.8.3.dist-info/RECORD,,
-blinkpy-0.8.3.dist-info/WHEEL,sha256=NzFAKnL7g-U64xnS1s5e3mJnxKpOTeOtlXdFwS9yNXI,92
-blinkpy-0.8.3.dist-info/top_level.txt,sha256=tNE6jcSsEnqvabMMI9EZmnpNtYd54KBiYFZFVTXmPB0,8
+blinkpy/helpers/util.py,sha256=zQArVcxBAdw09CLp_djtcvRxMfRvS6aviLJUfkEIm08,2991
+blinkpy-0.9.0.dist-info/METADATA,sha256=vucfixAEyw2-ae5yTUs5SOXkKI_wdWhTE34GXBLpMAw,5227
+blinkpy-0.9.0.dist-info/RECORD,,
+blinkpy-0.9.0.dist-info/WHEEL,sha256=NzFAKnL7g-U64xnS1s5e3mJnxKpOTeOtlXdFwS9yNXI,92
+blinkpy-0.9.0.dist-info/top_level.txt,sha256=tNE6jcSsEnqvabMMI9EZmnpNtYd54KBiYFZFVTXmPB0,8
```

