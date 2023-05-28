# Comparing `tmp/spotify_recommender_api-4.1.0-py3-none-any.whl.zip` & `tmp/spotify_recommender_api-4.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 36930 bytes, number of entries: 13
--rw-rw-r--  2.0 unx       21 b- defN 23-Apr-23 15:35 spotify_recommender_api/__init__.py
--rw-rw-r--  2.0 unx      636 b- defN 23-Apr-23 15:34 spotify_recommender_api/authentication.py
--rw-rw-r--  2.0 unx    14242 b- defN 23-Apr-23 15:35 spotify_recommender_api/core.py
--rw-rw-r--  2.0 unx     1966 b- defN 23-Apr-22 18:22 spotify_recommender_api/error.py
--rw-rw-r--  2.0 unx    95320 b- defN 23-Apr-23 15:38 spotify_recommender_api/recommender.py
--rw-rw-r--  2.0 unx     5866 b- defN 23-Apr-22 18:22 spotify_recommender_api/request_handler.py
+Zip file size: 37935 bytes, number of entries: 13
+-rw-rw-r--  2.0 unx       21 b- defN 23-May-28 16:03 spotify_recommender_api/__init__.py
+-rw-rw-r--  2.0 unx      636 b- defN 23-May-28 16:02 spotify_recommender_api/authentication.py
+-rw-rw-r--  2.0 unx    14264 b- defN 23-May-28 16:03 spotify_recommender_api/core.py
+-rw-rw-r--  2.0 unx     1966 b- defN 23-May-28 16:02 spotify_recommender_api/error.py
+-rw-rw-r--  2.0 unx    98800 b- defN 23-May-28 16:02 spotify_recommender_api/recommender.py
+-rw-rw-r--  2.0 unx     5933 b- defN 23-May-28 16:02 spotify_recommender_api/request_handler.py
 -rw-rw-r--  2.0 unx       99 b- defN 22-Jun-25 22:21 spotify_recommender_api/sensitive.py
--rw-rw-r--  2.0 unx     6661 b- defN 23-Apr-23 15:34 spotify_recommender_api/server.py
--rw-rw-r--  2.0 unx     9226 b- defN 23-Apr-23 15:38 spotify_recommender_api/util.py
--rw-rw-r--  2.0 unx    20363 b- defN 23-Apr-23 15:43 spotify_recommender_api-4.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-23 15:43 spotify_recommender_api-4.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       24 b- defN 23-Apr-23 15:43 spotify_recommender_api-4.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1192 b- defN 23-Apr-23 15:43 spotify_recommender_api-4.1.0.dist-info/RECORD
-13 files, 155708 bytes uncompressed, 34898 bytes compressed:  77.6%
+-rw-rw-r--  2.0 unx     6661 b- defN 23-May-28 16:03 spotify_recommender_api/server.py
+-rw-rw-r--  2.0 unx     9304 b- defN 23-May-28 16:02 spotify_recommender_api/util.py
+-rw-rw-r--  2.0 unx    21022 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       24 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1192 b- defN 23-May-28 16:25 spotify_recommender_api-4.2.0.dist-info/RECORD
+13 files, 160014 bytes uncompressed, 35903 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: spotify_recommender_api/server.py
 Comment: 
 
 Filename: spotify_recommender_api/util.py
 Comment: 
 
-Filename: spotify_recommender_api-4.1.0.dist-info/METADATA
+Filename: spotify_recommender_api-4.2.0.dist-info/METADATA
 Comment: 
 
-Filename: spotify_recommender_api-4.1.0.dist-info/WHEEL
+Filename: spotify_recommender_api-4.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: spotify_recommender_api-4.1.0.dist-info/top_level.txt
+Filename: spotify_recommender_api-4.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: spotify_recommender_api-4.1.0.dist-info/RECORD
+Filename: spotify_recommender_api-4.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotify_recommender_api/__init__.py

```diff
@@ -1 +1 @@
-__version__ = '4.1.0'
+__version__ = '4.2.0'
```

## spotify_recommender_api/core.py

```diff
@@ -1,8 +1,9 @@
 import pytz
+import logging
 import datetime
 import pandas as pd
 import seaborn as sns
 import matplotlib.pyplot as plt
 import spotify_recommender_api.util as util
 import spotify_recommender_api.request_handler as requests
 sns.set()
@@ -283,15 +284,15 @@
         chart_title (str, optional): label of the chart. Defaults to None
         top (int, optional): numbers of values to be in the chart. Defaults to 10
     """
 
     if plot_max:
         df = df[df['name'] != ''][:top + 1]
     else:
-        print(f'Total number of songs: {df["number of songs"][0]}')
+        logging.info(f'Total number of songs: {df["number of songs"][0]}')
         df = df[df['name'] != ''][1:top + 1]
 
     plt.figure(figsize=(15, 10))
 
     sns.color_palette('bright')
 
     sns.barplot(x='name', y='number of songs', data=df, label=chart_title)
```

## spotify_recommender_api/error.py

```diff
@@ -28,22 +28,22 @@
         super().__init__(f'{message}{err_code}')
 
 class TooManyRequestsError(HTTPRequestError):
     """Generic exception for HTTP Request Exceptions
         It can receive the function name and the function arguments, besides the message, to better help debugging the error
     """
     def __init__(self, func_name=None, message=None, *args, **kwargs):
-        super().__init__(err_code='429 Too Many Requests', func_name=func_name, message=message, *args, **kwargs)
+        super().__init__(*args, err_code='429 Too Many Requests', func_name=func_name, message=message, **kwargs)
 
 class AccessTokenExpiredError(HTTPRequestError):
     """Exception raised when the SpofifyAPI access token has expired
         It can receive the function name and the function arguments, besides the message, to better help debugging the error
     """
     func: Callable
     args: list
     kwargs: 'dict[str,]'
 
     def __init__(self, func_name: str = None, func: Callable = None, message: str = None, *args, **kwargs):
-        super().__init__(err_code='401 Access Token Expired', func_name=func_name, message=message, *args, **kwargs)
+        super().__init__(*args, err_code='401 Access Token Expired', func_name=func_name, message=message, **kwargs)
         self.func = func
         self.args = args
         self.kwargs = kwargs
```

## spotify_recommender_api/recommender.py

```diff
@@ -1,9 +1,10 @@
 import os
 import re
+import logging
 import operator
 import pandas as pd
 import spotify_recommender_api.util as util
 import spotify_recommender_api.core as core
 import spotify_recommender_api.authentication as auth
 import spotify_recommender_api.request_handler as requests
 from functools import reduce
@@ -22,26 +23,22 @@
     def __get_playlist_from_csv(self):
         """
         Function that creates the playlist variable from a CSV file previously created by this same package
 
         """
 
         try:
-            df = pd.read_parquet(
-                f'./.spotify-recommender-util/{self.__base_playlist_name}.parquet')
+            df = pd.read_parquet(f'./.spotify-recommender-util/{self.__base_playlist_name}.parquet')
         except FileNotFoundError as e:
             try:
-                df = pd.read_parquet(
-                    './.spotify-recommender-util/util.parquet')
-                print(f'The playlist {self.__base_playlist_name} does not exist in the CSV format, but ever since the version 3.5.0 the csv file and the util file created, have the same name as the playlist, but there is only a generic file on your machine.')
-                response = input(
-                    'Therefore, do you want to rename the generic files to the new format, and therefore having the playlist name (y/n)? ')
+                df = pd.read_parquet('./.spotify-recommender-util/util.parquet')
+                logging.warning(f'The playlist {self.__base_playlist_name} does not exist in the CSV format, but ever since the version 3.5.0 the csv file and the util file created, have the same name as the playlist, but there is only a generic file on your machine.')
+                response = input('Therefore, do you want to rename the generic files to the new format, and therefore having the playlist name (y/n)? ')
                 while response not in ['y', 'n']:
-                    response = input(
-                        'Select a valid option.\n Do you want to rename the generic files to the new format, and therefore having the playlist name (y/n)? ')
+                    response = input('Select a valid option.\n Do you want to rename the generic files to the new format, and therefore having the playlist name (y/n)? ')
 
                 if response == 'n':
                     raise FileNotFoundError(
                         'The playlist with the specified ID does not exist in the CSV format, try again but selecting the "web" option, as the source for the playlist') from e
 
                 else:
                     self.__update_created_files = True
@@ -59,16 +56,15 @@
             self.__playlist = pd.read_csv(f'{self.__base_playlist_name}.csv')
 
     def __get_playlist(self):
         """
         General purpose function to get the playlist, either from CSV or web requests
 
         """
-        answer = input(
-            'Do you want to get the playlist data via CSV saved previously or read from spotify, *which will take a few minutes* depending on the playlist size (csv/web)? ')
+        answer = input('Do you want to get the playlist data via CSV saved previously or read from spotify, *which will take a few minutes* depending on the playlist size (csv/web)? ')
         while answer.lower() not in ['csv', 'web']:  # , 'parquet'
             answer = input("Please select a valid response: ")
 
         self.__update_created_files = False
         if answer.lower() == 'csv':
             self.__get_playlist_from_csv()
             return False
@@ -87,23 +83,22 @@
         """
         genres = []
         song_artists = song["track"]["artists"] if 'track' in list(
             song.keys()) else song["artists"]
         for artist in song_artists:
             artist_id = artist["id"]
             if artist_id not in self.__artists:
-                artist_genres_res = requests.get_request(
-                    url=f'https://api.spotify.com/v1/artists/{artist_id}', headers=self.__headers)
+                artist_genres_res = requests.get_request(url=f'https://api.spotify.com/v1/artists/{artist_id}', headers=self.__headers)
                 try:
                     artist_genres = artist_genres_res.json()["genres"]
+                    genres += artist_genres
+                    self.__artists[artist["name"]] = artist_genres
                 except Exception as e:
-                    print(f'{e = }')
-                    print(artist_genres_res.json())
-                genres += artist_genres
-                self.__artists[artist["name"]] = artist_genres
+                    logging.error(f'{e = }')
+                    logging.debug(artist_genres_res.json())
             else:
                 genres += self.__artists[artist_id]
 
         return list(set(genres))
 
     def __get_playlist_items(self):
         """
@@ -113,15 +108,15 @@
         Ran automatically but can last as long as 2.5 seconds for each song (can be worse depending on the network connection) inside of the playlist, not because it is compute demanding but because it needs to do a up to a handful of http requests per song, which can take a while
 
         """
         self.__all_genres = []
         try:
             total_song_count = util.get_total_song_count(playlist_id=self.__playlist_id, headers=self.__headers)
             for offset in range(0, total_song_count, 100):
-                print(f'Songs mapped: {offset}/{total_song_count}')
+                logging.info(f'Songs mapped: {offset}/{total_song_count}')
                 all_genres_res = requests.get_request(
                     headers=self.__headers,
                     url=f'https://api.spotify.com/v1/playlists/{self.__playlist_id}/tracks?limit=100&{offset=!s}'
                 )
                 for song in all_genres_res.json()["items"]:
                     (id, name, popularity, artist, added_at), song_genres = util.song_data(
                         song=song), self.__get_song_genres(song)
@@ -155,63 +150,68 @@
         Function that gets the items (songs) inside the user's liked songs
 
         # Note
         Ran automatically but can last as long as 2.5 seconds for each song (can be worse depending on the network connection) inside of the playlist, not because it is compute demanding but because it needs to do a up to a handful of http requests per song, which can take a while
 
         """
         self.__all_genres = []
-        try:
-            total_song_count = requests.get_request(
-                headers=self.__headers, url='https://api.spotify.com/v1/me/tracks').json()['total']
-            for offset in range(0, total_song_count, 50):
-                print(f'Songs mapped: {offset}/{total_song_count}')
-                all_genres_res = requests.get_request(
-                    headers=self.__headers,
-                    url=f'https://api.spotify.com/v1/me/tracks?limit=50&{offset=!s}'
-                )
-                for song in all_genres_res.json()["items"]:
-                    (id, name, popularity, artist, added_at), song_genres = util.song_data(
-                        song=song), self.__get_song_genres(song)
-                    song['id'] = id
-                    danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
-                        song=song, headers=self.__headers)
-                    self.__songs.append({
-                        "id": id,
-                        "name": name,
-                        "artists": artist,
-                        "popularity": popularity,
-                        "genres": song_genres,
-                        "added_at": added_at,
-                        "danceability": danceability,
-                        "energy": energy,
-                        "instrumentalness": instrumentalness,
-                        "tempo": tempo,
-                        "valence": valence
-                    })
-                    self.__all_genres += song_genres
+        for _ in range(2):
+            try:
+                total_song_count = requests.get_request(headers=self.__headers, url='https://api.spotify.com/v1/me/tracks').json()['total']
 
-            print(
-                f'Songs mapping complete: {total_song_count}/{total_song_count}')
+                for offset in range(0, total_song_count, 50):
+                    logging.info(f'Songs mapped: {offset}/{total_song_count}')
+                    all_genres_res = requests.get_request(
+                        headers=self.__headers,
+                        url=f'https://api.spotify.com/v1/me/tracks?limit=50&{offset=!s}'
+                    )
+                    for song in all_genres_res.json()["items"]:
+                        (id, name, popularity, artist, added_at), song_genres = util.song_data(
+                            song=song), self.__get_song_genres(song)
+                        song['id'] = id
+                        danceability, energy, instrumentalness, tempo, valence = util.query_audio_features(
+                            song=song, headers=self.__headers)
+                        self.__songs.append({
+                            "id": id,
+                            "name": name,
+                            "artists": artist,
+                            "popularity": popularity,
+                            "genres": song_genres,
+                            "added_at": added_at,
+                            "danceability": danceability,
+                            "energy": energy,
+                            "instrumentalness": instrumentalness,
+                            "tempo": tempo,
+                            "valence": valence
+                        })
+                        self.__all_genres += song_genres
 
-        except KeyError as e:
-            raise ValueError(
-                'Invalid Auth Token, try again with a valid one') from e
+                logging.info(f'Songs mapping complete: {total_song_count}/{total_song_count}')
 
-        else:
-            self.__all_genres = list(set(self.__all_genres))
+                self.__all_genres = list(set(self.__all_genres))
+
+            except AccessTokenExpiredError as e:
+                logging.warning('Error due to the access token expiration')
+                auth_token = auth.get_auth()
+
+                self.__auth_token = auth_token
+
+                self.__headers['Authorization'] = f'Bearer {auth_token}'
+            else:
+                break
 
     def __playlist_adjustments(self):
         """
         Function that does a bunch of adjustments to the overall formatting of the playlist, before making it visible
 
         """
         try:
             songs = self.__songs[-util.get_total_song_count(playlist_id=self.__playlist_id, headers=self.__headers):]
         except KeyError as e:
-            raise ValueError('Invalid Auth Token, try again with a valid one') from e
+            raise AccessTokenExpiredError('Invalid Auth Token, try again with a valid one') from e
 
         self.__all_artists = list(self.__artists.keys())
         playlist = pd.DataFrame(data=list(songs))
 
         playlist["genres_indexed"] = [
             util.item_list_indexed(
                 all_items=self.__all_genres,
@@ -232,44 +232,75 @@
         playlist['danceability'] = playlist["danceability"].astype(float)
         playlist['energy'] = playlist["energy"].astype(float)
         playlist['instrumentalness'] = playlist["instrumentalness"].astype(float)
         playlist['tempo'] = playlist["tempo"].astype(float)
         playlist['valence'] = playlist["valence"].astype(float)
         self.__playlist = playlist
 
-    def __init__(self, auth_token: str, user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False, prepare_favorites: bool = False):
-        """Spotify API is the Class that provides access to the playlists recommendations
+    def playlist_to_csv(self):
+        """
+        Function to convert playlist to CSV format
+        Really useful if the package is being used in a .py file since it is not worth it to use it directly through web requests everytime even more when the playlist has not changed since last package usage
+        """
+        if not os.path.exists('./.spotify-recommender-util'):
+            os.mkdir('./.spotify-recommender-util')
 
-        Note:
-            It will trigger most of the API functions and can take a good while to complete
+        df = pd.DataFrame(
+            columns=['artists', 'songs', 'all_genres'],
+            data=[
+                {
+                    'songs': self.__songs,
+                    'artists': self.__artists,
+                    'all_genres': self.__all_genres
+                }
+            ],
+        )
 
+        df.to_parquet(
+            f'./.spotify-recommender-util/{self.__base_playlist_name}.parquet')
 
-        Args:
-            auth_token (str): The authentication token for the Spotify API, base64 encoded string that allows the use of the API's functionalities
-            user_id (str): The user ID, visible in the Spotify profile account settings
-            playlist_id (str, optional): The playlist ID hash in Spotify. Defaults to None.
-            playlist_url (str, optional): The url used while sharing the playlist. Defaults to None.
+        playlist = self.__playlist[
+            [
+                'id',
+                'name',
+                'artists',
+                'genres',
+                'popularity',
+                'added_at',
+                'danceability',
+                'energy',
+                'instrumentalness',
+                'tempo',
+                'valence'
+            ]
+        ]
+
+        playlist.to_csv(f'{self.__base_playlist_name}.csv')
+
+    def select_playlist(
+            self,
+            user_id: str,
+            playlist_id: str = None,
+            playlist_url: str = None,
+            liked_songs: bool = False,
+            prepare_favorites: bool = False
+        ) -> None:
+        """Function to select a playlist to be mapped and be available on all the playlist related recommendation functions
+
+        Args:
+            user_id (str): Spotify User ID
+            playlist_id (str, optional): Playlist ID. Defaults to None.
+            playlist_url (str, optional): Playlist Share URL (contains the ID, and it's easier to get). Defaults to None.
+            liked_songs (bool, optional): Flag to use the user 'Liked songs' as the playlist. Defaults to False.
+            prepare_favorites (bool, optional): Flag to prepare the deprecated functions for mid-term and short term favorites. Defaults to False.
 
-        Raises:
-            ValueError: auth_token is required
-            ValueError: Either the playlist url or its id must be specified
         """
-        if not auth_token:
-            raise ValueError('auth_token is required')
-        self.__user_id = user_id
-        self.__auth_token = auth_token
-        self.__headers = {
-            "Accept": "application/json",
-            "Content-Type": "application/json",
-            "Authorization": self.__auth_token
-        }
         self.__artists = {}
         self.__songs = []
         self.__deny_favorites = False
-
         if liked_songs:
             self.__playlist_id = 'liked_songs'
 
             self.__base_playlist_name = f'{user_id} Liked Songs'
 
         else:
             if playlist_id:
@@ -277,77 +308,88 @@
             else:
                 if not playlist_url:
                     raise ValueError(
                         'Either the playlist url or its id must be specified')
                 self.__playlist_id = util.playlist_url_to_id(url=playlist_url)
                 self.__playlist_url = playlist_url
 
-            self.__base_playlist_name = util.get_base_playlist_name(
-                playlist_id=self.__playlist_id, headers=self.__headers)
+            for _ in range(2):
+                try:
+                    self.__base_playlist_name = util.get_base_playlist_name(
+                        headers=self.__headers,
+                        playlist_id=self.__playlist_id,
+                    )
+                except AccessTokenExpiredError as e:
+                    logging.warning('Error due to the access token expiration')
+                    auth_token = auth.get_auth()
+
+                    self.__auth_token = auth_token
+
+                    self.__headers['Authorization'] = f'Bearer {auth_token}'
+                else:
+                    break
 
-        print('Mapping playlist items')
+
+        logging.info('Mapping playlist items')
 
         if self.__get_playlist():
             if liked_songs:
                 self.__get_liked_songs()
             else:
                 self.__get_playlist_items()
 
-        print('Setting up some operations with the playlist')
+        logging.info('Setting up some operations with the playlist')
 
         self.__playlist_adjustments()
 
         self.__song_dict = core.knn_prepared_data(playlist=self.__playlist)
         if prepare_favorites:
             self.__prepare_favorites_playlist()
 
         if self.__update_created_files:
             self.playlist_to_csv()
 
         self.__top_genres = self.__top_artists = self.__top_tracks = None
 
-    def playlist_to_csv(self):
-        """
-        Function to convert playlist to CSV format
-        Really useful if the package is being used in a .py file since it is not worth it to use it directly through web requests everytime even more when the playlist has not changed since last package usage
-        """
-        if not os.path.exists('./.spotify-recommender-util'):
-            os.mkdir('./.spotify-recommender-util')
 
-        df = pd.DataFrame(
-            columns=['artists', 'songs', 'all_genres'],
-            data=[
-                {
-                    'songs': self.__songs,
-                    'artists': self.__artists,
-                    'all_genres': self.__all_genres
-                }
-            ],
-        )
 
-        df.to_parquet(
-            f'./.spotify-recommender-util/{self.__base_playlist_name}.parquet')
+    def __init__(self, auth_token: str, user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False, prepare_favorites: bool = False):
+        """Spotify API is the Class that provides access to the playlists recommendations
 
-        playlist = self.__playlist[
-            [
-                'id',
-                'name',
-                'artists',
-                'genres',
-                'popularity',
-                'added_at',
-                'danceability',
-                'energy',
-                'instrumentalness',
-                'tempo',
-                'valence'
-            ]
-        ]
+        Note:
+            It will trigger most of the API functions and can take a good while to complete
 
-        playlist.to_csv(f'{self.__base_playlist_name}.csv')
+
+        Args:
+            auth_token (str): The authentication token for the Spotify API, base64 encoded string that allows the use of the API's functionalities
+            user_id (str): The user ID, visible in the Spotify profile account settings
+            playlist_id (str, optional): The playlist ID hash in Spotify. Defaults to None.
+            playlist_url (str, optional): The url used while sharing the playlist. Defaults to None.
+
+        Raises:
+            ValueError: auth_token is required
+            ValueError: Either the playlist url or its id must be specified
+        """
+        if not auth_token:
+            raise ValueError('auth_token is required')
+        self.__user_id = user_id
+        self.__auth_token = auth_token
+        self.__headers = {
+            "Accept": "application/json",
+            "Content-Type": "application/json",
+            "Authorization": self.__auth_token
+        }
+
+        self.select_playlist(
+            user_id=user_id,
+            liked_songs=liked_songs,
+            playlist_id=playlist_id,
+            playlist_url=playlist_url,
+            prepare_favorites=prepare_favorites
+        )
 
     def __get_neighbors(self, song: str, K: int, song_dict: list, type: str = None) -> list:
         """Function thats using the distance calculated above, returns the K nearest neighbors for a given song
 
         Args:
             song (str): song's index in the songs list
             K (int): desired number K of neighbors to be returned
@@ -471,15 +513,15 @@
             additional_info (Any, optional): the song name when the type is 'song'. Defaults to None.
 
         Raises:
             ValueError: Value for K must be between 1 and 1500
             ValueError: Invalid type
         """
         if K > 1500:
-            print('K limit exceded. Maximum value for K is 1500')
+            logging.warning('K limit exceded. Maximum value for K is 1500')
             K = 1500
         elif K < 1:
             raise ValueError(
                 f'Value for K must be between 1 and 1500 on creation of {type} playlist. {additional_info=!r}')
         uris = ''
         if type == 'song':
             index = self.__get_index_for_song(additional_info)
@@ -540,51 +582,51 @@
         try:
             if not (1 < K <= 1500):
                 raise ValueError(
                     f'Value for K must be between 1 and 1500 on creation of recommendation for the song {song}')
 
             self.__song_name = song
 
-            for _ in range(2):
-                try:
+            df = self.__get_recommendations('song', song, K)
+            playlist_name = f'{song} Related'
 
-                    df = self.__get_recommendations('song', song, K)
-                    playlist_name = f'{song} Related'
+            if print_base_caracteristics:
+                index = self.__get_index_for_song(song)
+                caracteristics = self.__song_dict[index]
+                name, genres, artists, popularity, _, danceability, energy, instrumentalness, tempo, valence = list(
+                    caracteristics.values())[1:11]
+                util.print_base_caracteristics(
+                    name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
 
-                    if print_base_caracteristics:
-                        index = self.__get_index_for_song(song)
-                        caracteristics = self.__song_dict[index]
-                        name, genres, artists, popularity, _, danceability, energy, instrumentalness, tempo, valence = list(
-                            caracteristics.values())[1:11]
-                        util.print_base_caracteristics(
-                            name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+            if generate_csv:
+                df.to_csv(f'{playlist_name}.csv')
 
-                    if generate_csv:
-                        df.to_csv(f'{playlist_name}.csv')
+            if generate_parquet:
+                df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
 
-                    if generate_parquet:
-                        df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
+            for _ in range(2):
+                try:
 
                     if build_playlist:
                         self.__write_playlist('song', K, additional_info=song)
 
                 except AccessTokenExpiredError as e:
-                    print('Error due to the access token expiration')
+                    logging.warning('Error due to the access token expiration')
                     auth_token = auth.get_auth()
 
                     self.__auth_token = auth_token
 
                     self.__headers['Authorization'] = f'Bearer {auth_token}'
                 else:
                     break
 
             return df if with_distance else df.drop(columns=['distance'])
 
         except ValueError as e:
-            print(e)
+            logging.error(e)
 
     def __get_desired_dict_fields(self, index: int, song_dict: list = None) -> 'list[str]':
         """Function that returns the usual fields for a given song
 
         Args:
             index (int): The index of the song inside the song list
             song_dict (list, optional): song dictionary. Defaults to None.
@@ -853,15 +895,15 @@
             build_playlist (bool, optional): Whether to generate a parquet file containing the recommended playlist. Defaults to False.
             generate_parquet (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
 
         Returns:
             pd.DataFrame: Short term favorites DataFrame
         """
         if self.__deny_favorites:
-            print("The chosen playlist does not contain the user's favorite songs")
+            logging.error("The chosen playlist does not contain the user's favorite songs")
             return
         df = self.__short_fav
         playlist_name = 'Latest Favorites'
         if generate_csv:
             df.to_csv(f'{playlist_name}.csv')
         if generate_parquet:
             df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
@@ -885,15 +927,15 @@
             generate_parquet (bool, optional): Whether to generate a parquet file containing the recommended playlist. Defaults to False.
             build_playlist (bool, optional): Whether to build the playlist to the user's library. Defaults to False.
 
         Returns:
             pd.DataFrame: Medium term favorites DataFrame
         """
         if self.__deny_favorites:
-            print("The chosen playlist does not contain the user's favorite songs")
+            logging.error("The chosen playlist does not contain the user's favorite songs")
             return
         df = self.__medium_fav
         playlist_name = 'Recent-ish Favorites'
         if generate_csv:
             df.to_csv(f'{playlist_name}.csv')
         if generate_parquet:
             df.to_parquet(f'{playlist_name}.parquet', compression='snappy')
@@ -936,87 +978,86 @@
             raise ValueError(
                 'time_range must be long, medium or short')
 
         if not (1 < K <= 1500):
             raise ValueError(
                 f'Value for K must be between 1 and 1500: {time_range} term most listened')
 
-        for _ in range(2):
-            try:
+        top = requests.get_request(
+            url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
 
-                top = requests.get_request(
-                    url=f'https://api.spotify.com/v1/me/top/tracks?{time_range=!s}_term&limit={K}', headers=self.__headers).json()
+        top_songs = list(map(lambda song: {'id': song['id'], 'name': song['name'], 'genres': self.__get_song_genres(song), 'artists': list(map(
+            lambda artist: artist['name'], song['artists'])), 'popularity': song['popularity']}, top['items']))
 
-                top_songs = list(map(lambda song: {'id': song['id'], 'name': song['name'], 'genres': self.__get_song_genres(song), 'artists': list(map(
-                    lambda artist: artist['name'], song['artists'])), 'popularity': song['popularity']}, top['items']))
+        for _ in range(2):
+            try:
 
                 if build_playlist:
                     self.__write_playlist(
                         f'most-listened-{time_range}', K, additional_info=list(map(lambda x: x['id'], top_songs)))
 
             except AccessTokenExpiredError as e:
-                print('Error due to the access token expiration')
+                logging.warning('Error due to the access token expiration')
                 auth_token = auth.get_auth()
 
                 self.__auth_token = auth_token
 
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
         return pd.DataFrame(data=list(map(lambda x: {'name': x['name'], 'genres': x['genres'], 'artists': x['artists'], 'popularity': x['popularity']}, top_songs)), columns=['name', 'artists', 'genres', 'popularity'])
 
-    def update_all_generated_playlists(self, K: int = None):
+    def update_all_generated_playlists(self, *, K: int = None, playlist_types_to_update: 'list[str]' = None):
         """Update all package generated playlists in batch
 
         Note:
             It is NOT recommended to use the K parameter in this function, unless 100% on purpose, since it will make all the playlists have the same number of songs in them
 
-        Args:
+        Keyword Arguments:
             K (int, optional): Number of songs in the new playlists, if not set, defaults to the number of songs already in the playlist. Defaults to None.
+            playlist_types_to_update (list[str], optional): List of playlist types to update. For example, if you only want to update song-related playlists use this argument as ['song-related']. Defaults to all - ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation'].
         """
-        total_playlist_count = requests.get_request(
-            url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
+        if playlist_types_to_update is None:
+            playlist_types_to_update = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation']
+
+        total_playlist_count = requests.get_request(url='https://api.spotify.com/v1/me/playlists?limit=0', headers=self.__headers).json()['total']
 
         playlists = []
 
         for offset in range(0, total_playlist_count, 50):
-            request = requests.get_request(
-                url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=self.__headers).json()
+            request = requests.get_request(url=f'https://api.spotify.com/v1/me/playlists?limit=50&{offset=!s}',  headers=self.__headers).json()
 
-            playlists += list(map(lambda playlist: (playlist['id'], playlist['name'],
-                              playlist['description'], playlist['tracks']['total']), request['items']))
+            playlists += list(map(lambda playlist: (playlist['id'], playlist['name'], playlist['description'], playlist['tracks']['total']), request['items']))
 
-        for id, name, description, total_tracks in playlists:
+        for _, name, description, total_tracks in playlists:
             try:
                 if K is not None:
                     total_tracks = K
-                if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'}:
-                    self.get_most_listened(time_range=name.split(
-                        " ")[0].lower(), K=total_tracks, build_playlist=True)
+                if name in {'Long Term Most-listened Tracks', 'Medium Term Most-listened Tracks', 'Short Term Most-listened Tracks'} and 'most-listened-tracks' in playlist_types_to_update:
+                    self.get_most_listened(time_range=name.split(" ")[0].lower(), K=total_tracks, build_playlist=True)
 
                 elif f', within the playlist {self.__base_playlist_name}' in description or self.__update_created_files:
-                    if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)):
+                    if (re.match(r"\'(.*?)\' Related", name) or re.match(r'\"(.*?)\" Related', name)) and 'song-related' in playlist_types_to_update:
                         song_name = name.replace(" Related", '')[1:-1]
                         self.__song_name = song_name
-                        self.__write_playlist(
-                            type='song', K=total_tracks - 1, additional_info=song_name)
+                        self.__write_playlist(type='song', K=total_tracks - 1, additional_info=song_name)
 
-                    elif (re.match(r"\'(.*?)\' Mix", name) or re.match(r'\"(.*?)\" Mix', name)):
+                    elif (re.match(r"\'(.*?)\' Mix", name) or re.match(r'\"(.*?)\" Mix', name)) and 'artist-mix' in playlist_types_to_update:
                         artist_name = name.replace(" Mix", '')[1:-1]
                         self.__artist_name = artist_name
                         self.artist_specific_playlist(
                             K=total_tracks,
                             build_playlist=True,
                             artist_name=artist_name,
                             complete_with_similar=True,
                             _auto=True
                         )
 
-                    elif (re.match(r"This once was \'(.*?)\'", name) or re.match(r'This once was \"(.*?)\"', name)):
+                    elif (re.match(r"This once was \'(.*?)\'", name) or re.match(r'This once was \"(.*?)\"', name)) and 'artist-full' in playlist_types_to_update:
                         artist_name = name.replace("This once was ", '')[1:-1]
                         self.__artist_name = artist_name
                         self.artist_specific_playlist(
                             K=total_tracks,
                             build_playlist=True,
                             artist_name=artist_name,
                             complete_with_similar=False,
@@ -1026,40 +1067,42 @@
 
                     # elif name == 'Recent-ish Favorites':
                     #     self.__write_playlist(type='medium', K=total_tracks)
 
                     # elif name == 'Latest Favorites':
                     #     self.__write_playlist(type='short', K=total_tracks)
 
-                    elif 'Playlist Recommendation' in name and ' - 20' not in name:
+                    elif 'Playlist Recommendation' in name and ' - 20' not in name and 'playlist-recommendation' in playlist_types_to_update:
                         criteria = name.split('(')[1].split(')')[0]
                         if ',' in criteria:
                             criteria = 'mixed'
 
                         time_range = 'all_time' if 'for all_time' in name else name.split(
                             'for the last')[-1].split('(')[0].strip()
 
                         self.get_playlist_recommendation(
                             K=total_tracks,
                             build_playlist=True,
                             time_range=time_range,
                             main_criteria=criteria,
                         )
 
-                elif 'Profile Recommendation' in name and ' - 20' not in name:
+                elif 'Profile Recommendation' in name and ' - 20' not in name and 'profile-recommendation' in playlist_types_to_update:
                     criteria = name.split('(')[1].split(')')[0]
                     if ',' in criteria:
                         criteria = 'mixed'
 
                     self.get_profile_recommendation(
-                        K=total_tracks, main_criteria=criteria, build_playlist=True)
+                        K=total_tracks,
+                        build_playlist=True,
+                        main_criteria=criteria,
+                    )
 
             except ValueError as e:
-                print(
-                    f"Unfortunately we couldn't update a playlist because\n {e}")
+                logging.error(f"Unfortunately we couldn't update a playlist because\n {e}")
 
     def get_playlist_trending_genres(self, time_range: str = 'all_time', plot_top: 'int|bool' = False) -> pd.DataFrame:
         """Calculates the amount of times each genre was spotted in the playlist, and can plot a bar chart to represent this information
 
         Args:
             time_range (str, optional): Time range that represents how much of the playlist will be considered for the trend. Can be one of the following: 'all_time', 'month', 'trimester', 'semester', 'year'. Defaults to 'all_time'.
             plot_top(int|bool , optional): the number of top genres to be plotted. Must be 5, 10, 15 or False. No chart will be plotted if set to False. Defaults to False.
@@ -1079,16 +1122,15 @@
             raise ValueError(
                 'plot_top must be either an int smaller than 30 or False')
 
         playlist = self.__playlist[self.__playlist['added_at'] >
                                    util.get_datetime_by_time_range(time_range=time_range)]
 
         if not len(playlist):
-            print(
-                f"No songs added to the playlist in the time range {time_range} ")
+            logging.warning(f"No songs added to the playlist in the time range {time_range} ")
             return None
 
         genres = list(reduce(lambda x, y: list(
             x) + list(y), playlist['genres'], []))
 
         genres_dict = dict(
             reduce(lambda x, y: util.list_to_count_dict(dictionary=x, item=y), genres, {}))
@@ -1138,16 +1180,15 @@
             raise ValueError(
                 'plot_top must be either an int smaller than 30 or False')
 
         playlist = self.__playlist[self.__playlist['added_at'] >
                                    util.get_datetime_by_time_range(time_range=time_range)]
 
         if not len(playlist):
-            print(
-                f"No songs added to the playlist in the time range {time_range} ")
+            logging.warning(f"No songs added to the playlist in the time range {time_range} ")
             return None
 
         artists = list(reduce(lambda x, y: list(
             x) + list(y), playlist['artists'], []))
 
         artists_dict = dict(reduce(lambda x, y: util.list_to_count_dict(
             dictionary=x, item=y), artists, {}))
@@ -1217,75 +1258,103 @@
                 f'{artist_name = } does not exist in the playlist')
 
         self.__artist_name = artist_name
 
         columns = ['id', 'name', 'artists', 'genres', 'popularity', 'added_at',
                    'danceability', 'energy', 'instrumentalness', 'tempo', 'valence']
 
-        if len(artist_songs) < K:
-            if complete_with_similar:
-                artist_songs_record_song_dict = list(map(lambda x: {'id': '', 'name': x['name'], 'artists': x['artists'], 'genres': x['genres'], 'artists_indexed': x['artists_indexed'], 'genres_indexed': x['genres_indexed'], 'popularity': x['popularity'], 'added_at': x[
-                                                     'added_at'], 'danceability': x['danceability'], 'energy': x['energy'], 'instrumentalness': x['instrumentalness'], 'tempo': x['tempo'], 'valence': x['valence']}, list(filter(lambda x: artist_name in x['artists'], self.__song_dict))))
-                artist_songs_record = self.__find_recommendations_to_songs(
-                    base_songs=artist_songs_record_song_dict, subset_name=f"{artist_name} Mix")
+        if complete_with_similar:
+            artist_songs_record_song_dict = list(map(
+                lambda x: {
+                    'id': '',
+                    'name': x['name'],
+                    'artists': x['artists'],
+                    'genres': x['genres'],
+                    'artists_indexed': x['artists_indexed'],
+                    'genres_indexed': x['genres_indexed'],
+                    'popularity': x['popularity'],
+                    'added_at': x['added_at'],
+                    'danceability': x['danceability'],
+                    'energy': x['energy'],
+                    'instrumentalness': x['instrumentalness'],
+                    'tempo': x['tempo'],
+                    'valence': x['valence']
+                },
+                list(filter(lambda x: artist_name in x['artists'], self.__song_dict))
+            ))
 
-                song_dict = list(map(lambda x: {'id': x['id'], 'name': x['name'], 'artists': x['artists'], 'genres': x['genres'], 'artists_indexed': x['artists_indexed'], 'genres_indexed': x['genres_indexed'], 'popularity': x['popularity'], 'added_at': x['added_at'],
-                                 'danceability': x['danceability'], 'energy': x['energy'], 'instrumentalness': x['instrumentalness'], 'tempo': x['tempo'], 'valence': x['valence']}, list(filter(lambda x: artist_name not in x['artists'], self.__song_dict))))
-                song_dict.append(artist_songs_record)
+            artist_songs_record = self.__find_recommendations_to_songs(base_songs=artist_songs_record_song_dict, subset_name=f"{artist_name} Mix")
 
-                mix_songs = self.__get_recommendations(
-                    'artist-related', song_dict, K=K-len(artist_songs))
+            song_dict = list(map(
+                lambda x: {
+                    'id': x['id'],
+                    'name': x['name'],
+                    'artists': x['artists'],
+                    'genres': x['genres'],
+                    'artists_indexed': x['artists_indexed'],
+                    'genres_indexed': x['genres_indexed'],
+                    'popularity': x['popularity'],
+                    'added_at': x['added_at'],
+                    'danceability': x['danceability'],
+                    'energy': x['energy'],
+                    'instrumentalness': x['instrumentalness'],
+                    'tempo': x['tempo'],
+                    'valence': x['valence']
+                },
+                list(filter(lambda x: artist_name not in x['artists'], self.__song_dict))
+            ))
 
-                ids = pd.concat([artist_songs['id'], mix_songs['id']])
+            song_dict.append(artist_songs_record)
 
-                if with_distance:
-                    df = artist_songs[columns]
+            mix_songs = self.__get_recommendations('artist-related', song_dict, K=K-len(artist_songs) if len(artist_songs) < K else len(artist_songs) // 3)
 
-                    columns.append('distance')
+            ids = pd.concat([artist_songs['id'], mix_songs['id']])
 
-                    df['distance'] = pd.to_numeric(0)
+            if with_distance:
+                df = artist_songs[columns]
 
-                    df = pd.concat([df[columns], mix_songs[columns]])
+                columns.append('distance')
 
-                else:
-                    df = pd.concat([artist_songs[columns], mix_songs[columns]])
+                df['distance'] = pd.to_numeric(0)
 
-                if print_base_caracteristics and not _auto:
-                    name = artist_songs_record['name']
-                    genres = artist_songs_record['genres']
-                    artists = artist_songs_record['artists']
-                    popularity = artist_songs_record['popularity']
-                    danceability = artist_songs_record['danceability']
-                    energy = artist_songs_record['energy']
-                    instrumentalness = artist_songs_record['instrumentalness']
-                    tempo = artist_songs_record['tempo']
-                    valence = artist_songs_record['valence']
-                    util.print_base_caracteristics(
-                        name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+                df = pd.concat([df[columns], mix_songs[columns]])
 
             else:
-                if not _auto:
-                    print(f'Playlist has only {len(artist_songs)} songs')
-                    print(
-                        f'To fill the {K = } number of songs, consider using the flag complete_with_similar')
-                ids = artist_songs['id']
-                df = artist_songs[columns]
+                df = pd.concat([artist_songs[columns], mix_songs[columns]])
+
+            if print_base_caracteristics and not _auto:
+                name = artist_songs_record['name']
+                genres = artist_songs_record['genres']
+                artists = artist_songs_record['artists']
+                popularity = artist_songs_record['popularity']
+                danceability = artist_songs_record['danceability']
+                energy = artist_songs_record['energy']
+                instrumentalness = artist_songs_record['instrumentalness']
+                tempo = artist_songs_record['tempo']
+                valence = artist_songs_record['valence']
+                util.print_base_caracteristics(name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence)
+
+        elif not _auto and len(artist_songs) < K:
+            logging.info(f'Playlist has only {len(artist_songs)} songs')
+            logging.info(f'To fill the {K = } number of songs, consider using the flag complete_with_similar')
+            ids = artist_songs['id']
+            df = artist_songs[columns]
 
         elif ensure_all_artist_songs:
             ids = artist_songs['id']
             df = artist_songs[columns]
 
         else:
             ids = artist_songs['id'][:K]
             df = artist_songs[columns][:K]
 
         if build_playlist:
             self.__write_playlist(
                 K=K,
-                type=f'artist{"-related" if len(artist_songs) < K and complete_with_similar else "-full" if ensure_all_artist_songs else ""}',
+                type=f'artist{"-related" if complete_with_similar else "-full" if ensure_all_artist_songs else ""}',
                 additional_info=ids
             )
 
         return df.reset_index(drop=True)
 
     def audio_features_extraordinary_songs(self) -> 'dict[str, dict]':
         """Returns a dictionary with the maximum and minimum values for each audio feature used in the package
@@ -1531,14 +1600,18 @@
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
             raise ValueError(
                 "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
 
+        tracks = None
+        genres = None
+        artists = None
+
         for _ in range(2):
             try:
 
                 if main_criteria != 'tracks':
                     if self.__top_genres or self.__top_artists:
                         genres = self.__top_genres
                         artists = self.__top_artists
@@ -1548,40 +1621,40 @@
                             url='https://api.spotify.com/v1/me/top/artists?time_range=short_term&limit=5', headers=self.__headers).json()['items']
 
                         artists = list(map(lambda x: x['id'], top_artists_req))
                         genres = list(set(reduce(
                             lambda x, y: x + y, list(map(lambda x: x['genres'], top_artists_req)), [])))[:5]
                         self.__top_genres = genres
                         self.__top_artists = artists
+
                 if main_criteria not in ['artists']:
                     if self.__top_tracks:
                         tracks = self.__top_tracks
 
                     else:
                         tracks = list(map(lambda x: x['id'], requests.get_request(
                             url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
 
                         self.__top_tracks = tracks
+
                 url = f'https://api.spotify.com/v1/recommendations?limit={K}'
 
                 if main_criteria == 'artists':
                     url += f'&seed_artists={",".join(artists)}'
                 elif main_criteria == 'genres':
                     url += f'&seed_genres={",".join(genres[:4])}&seed_tracks={",".join(tracks[:1])}'
                 elif main_criteria == 'mixed':
                     url += f'&seed_tracks={",".join(tracks[:2])}&seed_artists={",".join(artists[:1])}&seed_genres={",".join(genres[:2])}'
                 elif main_criteria == 'tracks':
                     url += f'&seed_tracks={",".join(tracks)}'
 
-                recommendations = requests.get_request(
-                    url=url, headers=self.__headers).json()
+                recommendations = requests.get_request(url=url, headers=self.__headers).json()
 
                 if not recommendations.get("tracks"):
-                    print(
-                        f'There was a problem creating the profile recommendations based on {main_criteria}')
+                    logging.error(f'There was a problem creating the profile recommendations based on {main_criteria}')
                     return
 
                 songs = []
 
                 for song in recommendations["tracks"]:
                     (id, name, popularity, artist), song_genres = util.song_data(
                         song=song, added_at=False), self.__get_song_genres(song)
@@ -1611,26 +1684,26 @@
 
                     self.__write_playlist(
                         K=K,
                         type='profile-recommendation',
                         additional_info=ids
                     )
 
+                return recommendations_playlist
+
             except AccessTokenExpiredError as e:
-                print('Error due to the access token expiration')
+                logging.warning('Error due to the access token expiration')
                 auth_token = auth.get_auth()
 
                 self.__auth_token = auth_token
 
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
-        return recommendations_playlist
-
     def get_playlist_recommendation(
         self,
         K: int = 50,
         time_range: str = 'all_time',
         main_criteria: str = 'mixed',
         save_with_date: bool = False,
         build_playlist: bool = False,
@@ -1655,14 +1728,18 @@
         if not (1 < K <= 100):
             raise ValueError('K must be between 1 and 100')
 
         if main_criteria not in ['mixed', 'artists', 'tracks', 'genres']:
             raise ValueError(
                 "main_criteria must be one of the following: 'mixed', 'artists', 'tracks', 'genres'")
 
+        tracks = None
+        genres = None
+        artists = None
+
 
         for _ in range(2):
             try:
                 audio_statistics = self.audio_features_statistics()
 
                 if main_criteria not in ['genres', 'tracks']:
                     top_artists_names = self.get_playlist_trending_artists(time_range=time_range)[
@@ -1671,21 +1748,19 @@
                         url=f'https://api.spotify.com/v1/search?q={x}&type=artist&limit=1', headers=self.__headers).json()['artists']['items'][0]['id'], top_artists_names))
 
                 if main_criteria not in ['artists']:
                     if self.__top_tracks:
                         tracks = self.__top_tracks
 
                     else:
-                        tracks = list(map(lambda x: x['id'], requests.get_request(
-                            url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
+                        tracks = list(map(lambda x: x['id'], requests.get_request(url='https://api.spotify.com/v1/me/top/tracks?time_range=short_term&limit=5', headers=self.__headers).json()['items']))
 
                         self.__top_tracks = tracks
                 if main_criteria != 'artists':
-                    genres = self.get_playlist_trending_genres(time_range=time_range)[
-                        'name'][1:6].tolist()[:5]
+                    genres = self.get_playlist_trending_genres(time_range=time_range)['name'][1:6].tolist()[:5]
 
                 min_tempo = audio_statistics['min_tempo'] * 0.8
                 max_tempo = audio_statistics['max_tempo'] * 1.2
                 target_tempo = audio_statistics['mean_tempo']
                 min_energy = audio_statistics['min_energy'] * 0.8
                 max_energy = audio_statistics['max_energy'] * 1.2
                 target_energy = audio_statistics['mean_energy']
@@ -1747,26 +1822,26 @@
 
                     self.__write_playlist(
                         K=K,
                         type='playlist-recommendation',
                         additional_info=ids
                     )
 
+                return recommendations_playlist
+
             except AccessTokenExpiredError as e:
-                print('Error due to the access token expiration')
+                logging.warning('Error due to the access token expiration')
                 auth_token = auth.get_auth()
 
                 self.__auth_token = auth_token
 
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
-        return recommendations_playlist
-
     def get_general_recommendation(
         self,
         K: int = 50,
         genres_info: 'list[str]' = [],
         artists_info: 'list[str]' = [],
         build_playlist: bool = False,
         use_main_playlist_audio_features: bool = False,
@@ -1947,28 +2022,29 @@
                     self.__general_recommendation_description_types = types
 
                     self.__write_playlist(
                         K=K,
                         type='general-recommendation',
                         additional_info=ids
                     )
+
+                return recommendations_playlist
+
             except AccessTokenExpiredError as e:
-                print('Error due to the access token expiration')
+                logging.warning('Error due to the access token expiration')
                 auth_token = auth.get_auth()
 
                 self.__auth_token = auth_token
 
                 self.__headers['Authorization'] = f'Bearer {auth_token}'
             else:
                 break
 
-        return recommendations_playlist
-
 
-def start_api(user_id: str, *, playlist_url: str = False, playlist_id: str = False, liked_songs: bool = False, prepare_favorites: bool = False):
+def start_api(user_id: str, *, playlist_url: str = False, playlist_id: str = False, liked_songs: bool = False, log_level: str = 'INFO', prepare_favorites: bool = False):
     """Function that prepares for and initializes the API
 
     Note:
         Internet Connection is required
 
     Args:
         user_id(str): the id of user, present in the user account profile
@@ -1986,20 +2062,28 @@
 
     Returns:
         SpotifyAPI: The instance of the SpotifyAPI class
 
     Note:
     Although both the playlist_url and playlist_id are optional, informing at least one of them is required, though the choice is up to you
     """
+    if log_level.upper() not in ['DEBUG', 'INFO', 'WARNING', 'ERROR']:
+        raise ValueError("log_level must be one of the following: 'DEBUG', 'INFO', 'WARNING', 'ERROR'")
+
+    logging.basicConfig(
+        level=log_level.upper(),
+        datefmt='%Y-%m-%d %H:%M:%S',
+        format='%(asctime)s.%(msecs)03d - %(levelname)s: %(message)s',
+    )
 
     if not playlist_url and not playlist_id and not liked_songs:
         raise ValueError(
             'It is necessary to specify a playlist either with playlist id or playlist url or flag the liked_songs as True')
     if (playlist_url or playlist_id) and liked_songs:
         raise ValueError(
             'It is necessary to specify only one of the following parameters: playlist_id or playlist_url or liked_songs')
 
-    print('Retrieving Authentication token')
+    logging.info('Retrieving Authentication token')
 
     auth_token = f'Bearer {auth.get_auth()}'
 
     return SpotifyAPI(auth_token=auth_token, playlist_id=playlist_id, user_id=user_id, playlist_url=playlist_url, liked_songs=liked_songs, prepare_favorites=prepare_favorites)
```

## spotify_recommender_api/request_handler.py

```diff
@@ -1,9 +1,10 @@
 import json
 import time
+import logging
 from requests import get, post, delete, put
 from spotify_recommender_api.error import HTTPRequestError, TooManyRequestsError, AccessTokenExpiredError
 
 
 def exponential_backoff(func, retries: int = 5, *args, **kwargs):
     """Exponential backoff strategy (https://en.wikipedia.org/wiki/Exponential_backoff)
     in order to retry certain function after exponetially increasing delay, to overcome "429: Too Many Requests" error
@@ -16,14 +17,15 @@
         Exception: Error raised in the function after {retries} attempts
 
     Returns:
         Any: specified function return
     """
     x = 0
     while x <= retries:
+        response = None
         try:
             response = func(*args, **kwargs)
             try:
                 response.json()
             except Exception as e: # this error happens when there is a 204 response and the response.json() cannot be decoded properly regardless of the request being successful
                 pass
             else:
@@ -31,30 +33,30 @@
                     raise HTTPRequestError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs)
             return response
         except Exception as e:
             if any(errorCode in f'{e}' for errorCode in ['404', '50']):
                 continue
 
             if '401' in f'{e}':
-                print('Access Token Expired')
+                logging.error('Access Token Expired')
                 raise AccessTokenExpiredError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs) from e
 
             if '429' not in f'{e}':
                 raise HTTPRequestError(func_name=func.__name__, err_code=f"{response.json()['error']['status']}: {response.json()['error']['message']}", message=None, *args, **kwargs) from e
 
             if x == 0:
-                print('\nExponential backoff triggered: ')
+                logging.warning('\nExponential backoff triggered: ')
 
             x += 1
 
             if x >= retries:
                 raise TooManyRequestsError(func_name=func.__name__, message=f'After {retries} attempts, the execution of the function failed with the 429 exception', *args, **kwargs) from e
 
             sleep = 2 ** x
-            print(f'\tError raised: sleeping {sleep} seconds')
+            logging.warning(f'\tError raised: sleeping {sleep} seconds')
             time.sleep(sleep)
 
 
 def get_request(url: str, headers: dict = None, retries: int = 10) -> dict:
     """GET request with integrated exponential backoff retry strategy
 
     Args:
```

## spotify_recommender_api/util.py

```diff
@@ -1,7 +1,8 @@
+import logging
 import warnings
 import datetime
 import functools
 import pandas as pd
 import spotify_recommender_api.request_handler as requests
 from dateutil import tz
 
@@ -209,23 +210,23 @@
         instrumentalness (float): song's instrumentalness
         tempo (float): song's tempo
         valence (float): song's valence
 
     """
     name, genres, artists, popularity, danceability, energy, instrumentalness, tempo, valence = args
 
-    print(f'{name = }')
-    print(f'{artists = }')
-    print(f'{genres = }')
-    print(f'{popularity = }')
-    print(f'{danceability = }')
-    print(f'{energy = }')
-    print(f'{instrumentalness = }')
-    print(f'{tempo = }')
-    print(f'{valence = }')
+    logging.info(f'{name = }')
+    logging.info(f'{artists = }')
+    logging.info(f'{genres = }')
+    logging.info(f'{popularity = }')
+    logging.info(f'{danceability = }')
+    logging.info(f'{energy = }')
+    logging.info(f'{instrumentalness = }')
+    logging.info(f'{tempo = }')
+    logging.info(f'{valence = }')
 
 
 def get_base_playlist_name(playlist_id: str, headers: dict) -> str:
     """Returns the base playlist name given the playlist id
 
     Args:
         playlist_id (str): The Spotify playlist id
```

## Comparing `spotify_recommender_api-4.1.0.dist-info/METADATA` & `spotify_recommender_api-4.2.0.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-recommender-api
-Version: 4.1.0
+Version: 4.2.0
 Summary: Python package which takes the songs of a greater playlist as starting point to make recommendations of groups of songs that might bond well within that same playlist, using K-Nearest-Neighbors Technique
 Home-page: https://github.com/nikolas-virionis/spotify-api
 Author: Nikolas B Virionis
 Author-email: nikolas.virionis@bandtec.com.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -83,28 +83,29 @@
 
   --- Playlist URL: The playlist url is available when right clicking the playlist name / or going to the three dots that represent the playlist options <br>
   --- Playlist ID: The playlist id is available the hash string between the last '/' in and the '?' in the playlist url<br>
   <img src='./readme-pictures/Playlist Configs.png' width='25%'><br>
   --- User ID: The user id is available when clicking the account, and accessing its information, on Spotify's website<br>
   <img src='./readme-pictures/Account.png' width='25%'><br>
   --- Liked Songs: A flag to pass in case the playlist you want to use is your profile Liked Songs <br>
+  --- Log level: the logging package log level. Defaults to INFO, but can be DEBUG, INFO, WARNING and ERROR
 
   - Calling the function:
 ~~~python
 api = start_api(playlist_url='<PLAYLIST_URL>', user_id='<USER_ID>')
 ~~~
 Or
 ~~~python
 api = start_api(playlist_id='<PLAYLIST_ID>', user_id='<USER_ID>')
 ~~~
 Or
 ~~~python
-api = start_api(liked_songs=True, user_id='<USER_ID>')
+api = start_api(liked_songs=True, user_id='<USER_ID>', log_level='DEBUG')
 ~~~
-Though, to be honest, it is easier and more convenient to use the playlist URL
+Though, to be honest, it is easier and more convenient to use the playlist URL or the liked_songs flag
 
   - Getting the Auth Token:
   It is a hash token that expires 60 minutes after it is generated, and after April 22nd 2023 it has been fully refactored, due to a change in the Spotify API Authentication methods, which invalidated the previous way. Now As soon as you call the start_api function a fastapi server will be lauched in port 8000.<br>
   The also there will be a web browser opened so that the user can click on the button Authorize, the log in with their spotify account, and then, the authentication is completed for that usage of the package.
 
 
 ## Methods
@@ -150,23 +151,22 @@
 # No parameters are mandatory but the default values should be noted
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~
  - update_all_generated_playlists
 ### WILL CHANGE THE USER'S LIBRARY DRASTICALLY
 ~~~python
 # Parameters
-update_all_generated_playlists(K: int = None)
+update_all_generated_playlists(K: int = None, playlist_types_to_update: list[str] = ['most-listened-tracks', 'song-related', 'artist-mix', 'artist-full', 'playlist-recommendation', 'profile-recommendation'])
 # Method Use Example
 api.update_all_generated_playlists()
+# or for example api.update_all_generated_playlists(playlist_types_to_update=['playlist-recommendation'])
 # Function updates all the playlists once generated by this package in batch
 # Note that if only a few updates are preferred, the methods above are a better fit
 # No parameters are mandatory but the default values should be noted, and if a value for K
-# is not specified, it takes as default the already existing playlist total song count,
-# or in the case of the playlist being one of the "This is" type, and was created with the
-# ensure_all_artist_songs Flag set to True, then the Flag will continue to take effect
+# is not specified, it takes as default the already existing playlist total song count which is recommended,
 ~~~
  - get_playlist_trending_genres
 ~~~python
 # Parameters
 get_playlist_trending_genres(time_range: str = 'all_time', plot_top: int|bool = False)
 # Method Use Example
 api.get_playlist_trending_genres()
@@ -247,14 +247,23 @@
 # Method Use Example
 api.get_general_recommendation(build_playlist=True, artists_info=['NF', 'Logic'], use_main_playlist_audio_features=True)
 # Function that returns a pandas DataFrame with artists, genres, and/or tracks based recommendations, and create it in the users account
 # genres_info, artists_info and tracks_info are the lists of information that the recommendation would be based on
 # use_main_playlist_audio_features is the flag to indicate if the playlist provided audio features will be used as target for a better recommendation
 # BUILD_PLAYLIST WILL CHANGE THE USER'S LIBRARY IF SET TO TRUE
 ~~~~~~
+ - select_playlist
+~~~python
+# Parameters
+select_playlist(user_id: str, playlist_id: str = None, playlist_url: str = None, liked_songs: bool = False)
+# Method Use Example
+api.select_playlist(user_id='USER_ID', liked_songs=True)
+# Function to select a playlist to be mapped and be available on all the playlist related recommendation
+# functions on an already existing authorization context
+~~~~~~
  - get_medium_term_favorites_playlist - DEPRECATED
 ~~~python
 # Parameters
 get_medium_term_favorites_playlist(with_distance: bool, generate_csv: bool,
                         generate_parquet: bool, build_playlist: bool)
 # Method Use Example
 api.get_medium_term_favorites_playlist(generate_csv=True, build_playlist=True)
```

