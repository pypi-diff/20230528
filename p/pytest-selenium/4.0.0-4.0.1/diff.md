# Comparing `tmp/pytest-selenium-4.0.0.tar.gz` & `tmp/pytest_selenium-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-selenium-4.0.0.tar", max compression
+gzip compressed data, last modified: Sun May 28 01:03:31 2023, max compression
```

## Comparing `pytest-selenium-4.0.0.tar` & `pytest_selenium-4.0.1.tar`

### file list

```diff
@@ -1,51 +1,56 @@
--rw-r--r--   0        0        0      193 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/LICENSE
--rw-r--r--   0        0        0     1474 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/README.rst
--rw-r--r--   0        0        0        7 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/.gitignore
--rw-r--r--   0        0        0     7445 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/Makefile
--rw-r--r--   0        0        0     9465 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/conf.py
--rw-r--r--   0        0        0     3177 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/development.rst
--rw-r--r--   0        0        0      261 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/index.rst
--rw-r--r--   0        0        0      531 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/installing.rst
--rw-r--r--   0        0        0     7262 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/make.bat
--rw-r--r--   0        0        0    10824 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/news.rst
--rw-r--r--   0        0        0    23309 2022-09-21 20:41:42.616585 pytest-selenium-4.0.0/docs/user_guide.rst
--rw-r--r--   0        0        0     2335 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/pyproject.toml
--rw-r--r--   0        0        0       39 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/__init__.py
--rw-r--r--   0        0        0       47 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/__init__.py
--rw-r--r--   0        0        0      566 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/appium.py
--rw-r--r--   0        0        0     3964 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/browserstack.py
--rw-r--r--   0        0        0     1010 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/chrome.py
--rw-r--r--   0        0        0     1746 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/cloud.py
--rw-r--r--   0        0        0     3972 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/crossbrowsertesting.py
--rw-r--r--   0        0        0      992 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/edge.py
--rw-r--r--   0        0        0     1892 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/firefox.py
--rw-r--r--   0        0        0      755 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/internet_explorer.py
--rw-r--r--   0        0        0      593 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/remote.py
--rw-r--r--   0        0        0      407 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/safari.py
--rw-r--r--   0        0        0     7197 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/saucelabs.py
--rw-r--r--   0        0        0     4248 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/drivers/testingbot.py
--rw-r--r--   0        0        0      962 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/exceptions.py
--rw-r--r--   0        0        0      446 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/hooks.py
--rw-r--r--   0        0        0    16798 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/pytest_selenium.py
--rw-r--r--   0        0        0     2931 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/safety.py
--rw-r--r--   0        0        0     2343 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/src/pytest_selenium/utils.py
--rw-r--r--   0        0        0        0 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/__init__.py
--rw-r--r--   0        0        0     2381 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/conftest.py
--rw-r--r--   0        0        0      534 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/empty.xpi
--rw-r--r--   0        0        0     6655 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_browserstack.py
--rw-r--r--   0        0        0     2168 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_capabilities.py
--rw-r--r--   0        0        0     1726 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_chrome.py
--rw-r--r--   0        0        0     1734 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_crossbrowsertesting.py
--rw-r--r--   0        0        0     2957 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_destructive.py
--rw-r--r--   0        0        0     8145 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_driver.py
--rw-r--r--   0        0        0     2099 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_driver_log.py
--rw-r--r--   0        0        0     1691 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_edge.py
--rw-r--r--   0        0        0     5099 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_firefox.py
--rw-r--r--   0        0        0     1526 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_metadata.py
--rw-r--r--   0        0        0     6000 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_report.py
--rw-r--r--   0        0        0      644 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_safari.py
--rw-r--r--   0        0        0     9159 2022-09-21 20:41:42.620586 pytest-selenium-4.0.0/testing/test_saucelabs.py
--rw-r--r--   0        0        0     3679 2022-09-21 20:41:42.624585 pytest-selenium-4.0.0/testing/test_testingbot.py
--rw-r--r--   0        0        0     1175 2022-09-21 20:41:42.624585 pytest-selenium-4.0.0/testing/test_webdriver.py
--rw-r--r--   0        0        0     3492 1970-01-01 00:00:00.000000 pytest-selenium-4.0.0/setup.py
--rw-r--r--   0        0        0     2985 1970-01-01 00:00:00.000000 pytest-selenium-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0      448 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1538 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/tox.ini
+-rw-r--r--   0        0        0        7 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/.gitignore
+-rw-r--r--   0        0        0     7445 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/Makefile
+-rw-r--r--   0        0        0     9465 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/conf.py
+-rw-r--r--   0        0        0     2834 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/development.rst
+-rw-r--r--   0        0        0      261 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/index.rst
+-rw-r--r--   0        0        0      531 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/installing.rst
+-rw-r--r--   0        0        0     7262 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/make.bat
+-rw-r--r--   0        0        0    10914 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/news.rst
+-rw-r--r--   0        0        0    23309 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/docs/user_guide.rst
+-rwxr-xr-x   0        0        0      605 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/installation/chromedriver.sh
+-rwxr-xr-x   0        0        0      840 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/installation/geckodriver.sh
+-rw-r--r--   0        0        0       39 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/__init__.py
+-rw-r--r--   0        0        0      160 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/__version.py
+-rw-r--r--   0        0        0      962 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/exceptions.py
+-rw-r--r--   0        0        0      446 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/hooks.py
+-rw-r--r--   0        0        0    16109 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/pytest_selenium.py
+-rw-r--r--   0        0        0     2931 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/safety.py
+-rw-r--r--   0        0        0     2343 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/utils.py
+-rw-r--r--   0        0        0       47 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/__init__.py
+-rw-r--r--   0        0        0      566 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/appium.py
+-rw-r--r--   0        0        0     3974 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/browserstack.py
+-rw-r--r--   0        0        0      751 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/chrome.py
+-rw-r--r--   0        0        0     1746 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/cloud.py
+-rw-r--r--   0        0        0     3992 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/crossbrowsertesting.py
+-rw-r--r--   0        0        0      670 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/edge.py
+-rw-r--r--   0        0        0     1892 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/firefox.py
+-rw-r--r--   0        0        0      482 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/internet_explorer.py
+-rw-r--r--   0        0        0      593 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/remote.py
+-rw-r--r--   0        0        0      407 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/safari.py
+-rw-r--r--   0        0        0     7217 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/saucelabs.py
+-rw-r--r--   0        0        0     4268 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/src/pytest_selenium/drivers/testingbot.py
+-rw-r--r--   0        0        0        0 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/__init__.py
+-rw-r--r--   0        0        0     2381 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/conftest.py
+-rw-r--r--   0        0        0      534 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/empty.xpi
+-rw-r--r--   0        0        0     6655 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_browserstack.py
+-rw-r--r--   0        0        0     2168 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_capabilities.py
+-rw-r--r--   0        0        0     1726 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_chrome.py
+-rw-r--r--   0        0        0     1734 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_crossbrowsertesting.py
+-rw-r--r--   0        0        0     2957 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_destructive.py
+-rw-r--r--   0        0        0     7784 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_driver.py
+-rw-r--r--   0        0        0     2099 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_driver_log.py
+-rw-r--r--   0        0        0     1462 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_edge.py
+-rw-r--r--   0        0        0     5099 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_firefox.py
+-rw-r--r--   0        0        0     1164 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_metadata.py
+-rw-r--r--   0        0        0     5647 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_report.py
+-rw-r--r--   0        0        0      644 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_safari.py
+-rw-r--r--   0        0        0     9200 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_saucelabs.py
+-rw-r--r--   0        0        0     3679 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_testingbot.py
+-rw-r--r--   0        0        0     1175 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/testing/test_webdriver.py
+-rw-r--r--   0        0        0      124 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/.gitignore
+-rw-r--r--   0        0        0      193 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/LICENSE
+-rw-r--r--   0        0        0     1323 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/README.rst
+-rw-r--r--   0        0        0     2874 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3476 2023-05-28 01:03:31.000000 pytest_selenium-4.0.1/PKG-INFO
```

### Comparing `pytest-selenium-4.0.0/README.rst` & `pytest_selenium-4.0.1/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -6,22 +6,19 @@
 
 .. image:: https://img.shields.io/badge/license-MPL%202.0-blue.svg
    :target: https://github.com/pytest-dev/pytest-selenium/blob/master/LICENSE
    :alt: License
 .. image:: https://img.shields.io/pypi/v/pytest-selenium.svg
    :target: https://pypi.python.org/pypi/pytest-selenium/
    :alt: PyPI
-.. image:: https://img.shields.io/travis/pytest-dev/pytest-selenium.svg
-   :target: https://travis-ci.org/pytest-dev/pytest-selenium/
-   :alt: Travis
 .. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
    :target: http://pytest-selenium.readthedocs.io/en/latest/
    :alt: Read the Docs
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/ambv/black
+   :target: https://github.com/ambv/black
 .. image:: https://img.shields.io/github/issues-raw/pytest-dev/pytest-selenium.svg
    :target: https://github.com/pytest-dev/pytest-selenium/issues
    :alt: Issues
 .. image:: https://img.shields.io/requires/github/pytest-dev/pytest-selenium.svg
    :target: https://requires.io/github/pytest-dev/pytest-selenium/requirements/?branch=master
    :alt: Requirements
```

### Comparing `pytest-selenium-4.0.0/docs/Makefile` & `pytest_selenium-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/docs/conf.py` & `pytest_selenium-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/docs/development.rst` & `pytest_selenium-4.0.1/docs/development.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,56 +1,46 @@
 Development
 ===========
 
-To contribute to `pytest-selenium` you can use `Pipenv`_ to manage
+To contribute to `pytest-selenium` you can use `Hatch`_ to manage
 a python virtual environment and `pre-commit <https://pre-commit.com/>`_ to help you with
 styling and formatting.
 
 To setup the virtual environment and pre-commit, run:
 
 .. code-block:: bash
 
-  $ pipenv install --dev
-  $ pipenv run pre-commit install
+  $ hatch -e test run pre-commit install
 
-If you're not using `Pipenv`_, to install `pre-commit`, run:
+If you're not using `Hatch`_, to install `pre-commit`, run:
 
 .. code-block:: bash
 
   $ pip install pre-commit
   $ pre-commit install
 
 
 Automated Testing
 -----------------
 
-All pull requests and merges are tested in `Travis CI <https://travis-ci.org/>`_
-based on the ``.travis.yml`` file.
-
-Usually, a link to your specific travis build appears in pull requests, but if
-not, you can find it on the
-`pull requests page <https://travis-ci.org/pytest-dev/pytest-selenium/pull_requests>`_
-
-The only way to trigger Travis CI to run again for a pull request, is to submit
-another change to the pull branch.
-
-You can do this with `git commit --allow-empty`
+All pull requests and merges are tested in `GitHub Actions <https://docs.github.com/en/actions>`_
+based on the workflows defined in ``.github/workflows``.
 
 Running Tests
 -------------
 
 You will need `Tox <http://tox.testrun.org/>`_ installed to run the tests
-against the supported Python versions. If you're using `Pipenv`_ it will be
+against the supported Python versions. If you're using `Hatch`_ it will be
 installed for you.
 
-With `Pipenv`_, run:
+With `Hatch`_, run:
 
 .. code-block:: bash
 
-  $ pipenv run tox
+  $ hatch -e test run tox
 
 Otherwise, to install and run, do:
 
 .. code-block:: bash
 
   $ pip install tox
   $ tox
@@ -97,12 +87,12 @@
 Follow these steps to release a new version of the project:
 
 1. Update your local master with the upstream master (``git pull --rebase upstream master``)
 2. Create a new branch and update ``news.rst`` with the new version, today's date, and all changes/new features
 3. Commit and push the new branch and then create a new pull request
 4. Wait for tests and reviews and then merge the branch
 5. Once merged, update your local master again (``git pull --rebase upstream master``)
-6. Tag the release with the new release version (``git tag v<new tag>``)
+6. Tag the release with the new release version (``git tag <new tag>``)
 7. Push the tag (``git push upstream --tags``)
 8. Done. You can monitor the progress on `Travis <https://travis-ci.org/pytest-dev/pytest-selenium/>`_
 
-.. _Pipenv: https://docs.pipenv.org/en/latest/
+.. _Hatch: https://hatch.pypa.io/latest/
```

### Comparing `pytest-selenium-4.0.0/docs/installing.rst` & `pytest_selenium-4.0.1/docs/installing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Installation
 ============
 
 Requirements
 ------------
 
-pytest-selenium will work with Python >=3.6.
+pytest-selenium will work with Python >=3.7.
 
 Install pytest-selenium
 -----------------------
 
 To install pytest-selenium using `pip <https://pip.pypa.io/>`_:
 
 .. code-block:: bash
```

### Comparing `pytest-selenium-4.0.0/docs/make.bat` & `pytest_selenium-4.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/docs/news.rst` & `pytest_selenium-4.0.1/docs/news.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Release Notes
 =============
 
+4.0.1 (2023-05-28)
+------------------
+
+* Switch to Hatch
+
+* Relax dependency constraints
+
 4.0.0 (2022-09-15)
 ------------------
 
 * Selenium 4 support
 
 * Drop support for python 3.6
```

### Comparing `pytest-selenium-4.0.0/docs/user_guide.rst` & `pytest_selenium-4.0.1/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/appium.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/appium.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/browserstack.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/browserstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
             )
         except MissingCloudSettingError:
             field = "browser_url"
 
         return field
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_runtest_makereport(item, report, summary, extra):
     provider = BrowserStack()
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     passed = report.passed or (report.failed and hasattr(report, "wasxfail"))
     session_id = item._driver.session_id
```

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/cloud.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/cloud.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/crossbrowsertesting.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/crossbrowsertesting.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     @property
     def key(self):
         return self.get_credential(
             "key", ["CROSSBROWSERTESTING_AUTH_KEY", "CROSSBROWSERTESTING_PSW"]
         )
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_capture_debug(item, report, extra):
     provider = CrossBrowserTesting()
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     # lazy import requests for projects that don't need requests
     import requests
@@ -53,15 +53,15 @@
     )
 
     if videos and len(videos) > 0:
         pytest_html = item.config.pluginmanager.getplugin("html")
         extra.append(pytest_html.extras.html(_video_html(videos[0])))
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_runtest_makereport(item, report, summary, extra):
     provider = CrossBrowserTesting()
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     passed = report.passed or (report.failed and hasattr(report, "wasxfail"))
```

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/edge.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/edge.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
-from packaging.version import Version
-
 import pytest
-from selenium import __version__ as SELENIUM_VERSION
 from selenium.webdriver.edge.options import Options
 
 
 def driver_kwargs(capabilities, driver_log, driver_path, edge_options, **kwargs):
 
-    # Selenium 3.14.0 deprecated log_path in favour of service_log_path
-    if Version(SELENIUM_VERSION) < Version("3.14.0"):
-        kwargs = {"log_path": driver_log}
-    else:
-        kwargs = {"service_log_path": driver_log}
-
-    if Version(SELENIUM_VERSION) >= Version("4.0.0"):
-        kwargs["options"] = edge_options
+    kwargs = {
+        "service_log_path": driver_log,
+        "options": edge_options,
+    }
 
     if capabilities:
         kwargs["capabilities"] = capabilities
     if driver_path is not None:
         kwargs["executable_path"] = driver_path
 
     return kwargs
```

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/firefox.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/firefox.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/remote.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/remote.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/saucelabs.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/saucelabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,25 +48,25 @@
             "key", ["SAUCELABS_API_KEY", "SAUCELABS_PSW", "SAUCE_ACCESS_KEY"]
         )
 
     def uses_driver(self, driver):
         return driver.lower() == self.name.lower()
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_capture_debug(item, report, extra):
     provider = SauceLabs(item.config.getini("saucelabs_data_center"))
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     pytest_html = item.config.pluginmanager.getplugin("html")
     extra.append(pytest_html.extras.html(_video_html(item._driver.session_id)))
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_runtest_makereport(item, report, summary, extra):
     provider = SauceLabs(item.config.getini("saucelabs_data_center"))
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     passed = report.passed or (report.failed and hasattr(report, "wasxfail"))
     session_id = item._driver.session_id
```

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/drivers/testingbot.py` & `pytest_selenium-4.0.1/src/pytest_selenium/drivers/testingbot.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,29 +38,29 @@
         return self.get_credential("key", ["TESTINGBOT_KEY", "TESTINGBOT_USR"])
 
     @property
     def secret(self):
         return self.get_credential("secret", ["TESTINGBOT_SECRET", "TESTINGBOT_PSW"])
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_capture_debug(item, report, extra):
     provider = TestingBot()
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     session_id = item._driver.session_id
     auth_url = get_auth_url(
         "https://testingbot.com/tests/{}.mp4".format(session_id), provider, session_id
     )
     pytest_html = item.config.pluginmanager.getplugin("html")
     extra.append(pytest_html.extras.html(_video_html(auth_url, session_id)))
 
 
-@pytest.mark.optionalhook
+@pytest.hookimpl(optionalhook=True)
 def pytest_selenium_runtest_makereport(item, report, summary, extra):
     provider = TestingBot()
     if not provider.uses_driver(item.config.getoption("driver")):
         return
 
     passed = report.passed or (report.failed and hasattr(report, "wasxfail"))
     session_id = item._driver.session_id
```

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/exceptions.py` & `pytest_selenium-4.0.1/src/pytest_selenium/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/pytest_selenium.py` & `pytest_selenium-4.0.1/src/pytest_selenium/pytest_selenium.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from selenium.webdriver.common.desired_capabilities import DesiredCapabilities
 from selenium.webdriver.support.event_firing_webdriver import EventFiringWebDriver
 from tenacity import Retrying, stop_after_attempt, wait_exponential
 
 from .utils import CaseInsensitiveDict
 from . import drivers
 
-import warnings
 
 LOGGER = logging.getLogger(__name__)
 
 SUPPORTED_DRIVERS = CaseInsensitiveDict(
     {
         "BrowserStack": webdriver.Remote,
         "CrossBrowserTesting": webdriver.Remote,
@@ -224,57 +223,53 @@
 @pytest.fixture
 def selenium(driver):
     yield driver
 
 
 @pytest.hookimpl(trylast=True)
 def pytest_configure(config):
-    if config.getoption("host"):
-        warnings.warn(
-            "--host has been deprecated and will be removed in a "
-            "future release. Please use --selenium-host instead.",
-            DeprecationWarning,
-        )
-        config.option.selenium_host = config.getoption("host")
-
-    if config.getoption("port"):
-        warnings.warn(
-            "--port has been deprecated and will be removed in a "
-            "future release. Please use --selenium-port instead.",
-            DeprecationWarning,
-        )
-        config.option.selenium_port = config.getoption("port")
+    try:
+        capabilities = config._variables.get("capabilities", {})
+    except AttributeError:
+        from pytest_variables.plugin import variables_key
 
-    capabilities = config._variables.get("capabilities", {})
+        capabilities = config.stash[variables_key].get("capabilities", {})
     capabilities.update({k: v for k, v in config.getoption("capabilities")})
     config.addinivalue_line(
         "markers",
         "capabilities(kwargs): add or change existing "
         "capabilities. specify capabilities as keyword arguments, for example "
         "capabilities(foo="
         "bar"
         ")",
     )
-    if hasattr(config, "_metadata"):
-        config._metadata["Driver"] = config.getoption("driver")
-        config._metadata["Capabilities"] = capabilities
+    metadata = config.pluginmanager.getplugin("metadata")
+    if metadata:
+        try:
+            metadata = config._metadata
+        except AttributeError:
+            from pytest_metadata.plugin import metadata_key
+
+            metadata = config.stash[metadata_key]
+        metadata["Driver"] = config.getoption("driver")
+        metadata["Capabilities"] = capabilities
         if all((config.option.selenium_host, config.option.selenium_port)):
-            config._metadata["Server"] = "{0}:{1}".format(
+            metadata["Server"] = "{0}:{1}".format(
                 config.option.selenium_host, config.option.selenium_port
             )
     config._capabilities = capabilities
 
 
 def pytest_report_header(config, startdir):
     driver = config.getoption("driver")
     if driver is not None:
         return "driver: {0}".format(driver)
 
 
-@pytest.mark.hookwrapper
+@pytest.hookimpl(hookwrapper=True)
 def pytest_runtest_makereport(item, call):
     outcome = yield
     report = outcome.get_result()
     summary = []
     extra = getattr(report, "extra", [])
     driver = getattr(item, "_driver", None)
     xfail = hasattr(report, "wasxfail")
@@ -476,29 +471,14 @@
     group._addoption(
         "--event-listener",
         metavar="str",
         help="selenium eventlistener class, e.g. "
         "package.module.EventListenerClassName.",
     )
     group._addoption(
-        "--host",
-        metavar="str",
-        help="DEPRECATED host that the selenium server is listening on, "
-        "which will default to the cloud provider default "
-        "or localhost.",
-    )
-    group._addoption(
-        "--port",
-        type=int,
-        metavar="num",
-        help="DEPRECATED port that the selenium server is listening on, "
-        "which will default to the cloud provider default "
-        "or localhost.",
-    )
-    group._addoption(
         "--selenium-host",
         metavar="str",
         help="host that the selenium server is listening on, "
         "which will default to the cloud provider default "
         "or localhost.",
     )
     group._addoption(
```

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/safety.py` & `pytest_selenium-4.0.1/src/pytest_selenium/safety.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/src/pytest_selenium/utils.py` & `pytest_selenium-4.0.1/src/pytest_selenium/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/conftest.py` & `pytest_selenium-4.0.1/testing/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/empty.xpi` & `pytest_selenium-4.0.1/testing/empty.xpi`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_browserstack.py` & `pytest_selenium-4.0.1/testing/test_browserstack.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_capabilities.py` & `pytest_selenium-4.0.1/testing/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_chrome.py` & `pytest_selenium-4.0.1/testing/test_chrome.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_crossbrowsertesting.py` & `pytest_selenium-4.0.1/testing/test_crossbrowsertesting.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_destructive.py` & `pytest_selenium-4.0.1/testing/test_destructive.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_driver.py` & `pytest_selenium-4.0.1/testing/test_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from contextlib import ExitStack as does_not_raise
 from functools import partial
 
 import pytest_selenium
 import pytest
 
 from pytest_selenium.utils import CaseInsensitiveDict
 
@@ -134,45 +133,38 @@
         "--selenium-port",
         "4444",
         filetest,
         passed=1,
     )
 
 
-@pytest.mark.parametrize(
-    ("host_arg_name", "port_arg_name", "context"),
-    [
-        ("--selenium-host", "--selenium-port", does_not_raise()),
-        ("--host", "--port", pytest.warns(DeprecationWarning)),
-    ],
-)
-def test_arguments_order(testdir, host_arg_name, port_arg_name, context):
+def test_arguments_order(testdir):
     host = "notlocalhost"
     port = "4441"
     file_test = testdir.makepyfile(
         """
         import pytest
         @pytest.mark.nondestructive
         def test_pass(driver_kwargs):
             assert driver_kwargs['command_executor'] == 'http://{}:{}/wd/hub'
     """.format(
             host, port
         )
     )
-    with context:
-        testdir.quick_qa(
-            "--driver",
-            "Remote",
-            host_arg_name,
-            host,
-            port_arg_name,
-            port,
-            file_test,
-            passed=1,
-        )
+
+    testdir.quick_qa(
+        "--driver",
+        "Remote",
+        "--selenium-host",
+        host,
+        "--selenium-port",
+        port,
+        file_test,
+        passed=1,
+    )
 
 
 def test_arguments_order_random(testdir):
     host = "notlocalhost"
     port = "4441"
     file_test = testdir.makepyfile(
         """
```

### Comparing `pytest-selenium-4.0.0/testing/test_driver_log.py` & `pytest_selenium-4.0.1/testing/test_driver_log.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_edge.py` & `pytest_selenium-4.0.1/testing/test_edge.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import pytest
 import sys
-from packaging.version import Version
-from selenium import __version__ as SELENIUM_VERSION
 
 
 pytestmark = pytest.mark.nondestructive
 
 
 @pytest.mark.skipif(sys.platform != "win32", reason="Edge only runs on Windows")
 @pytest.mark.edge
@@ -23,18 +21,14 @@
             assert webtext == u'Success!'
     """
     )
     testdir.quick_qa("--driver", "Edge", file_test, passed=1)
 
 
 @pytest.mark.skipif(sys.platform != "win32", reason="Edge only runs on Windows")
-@pytest.mark.skipif(
-    Version(SELENIUM_VERSION) < Version("4.0.0"),
-    reason="Edge chromium only supported for selenium >= 4.0.0",
-)
 @pytest.mark.edge
 @pytest.mark.parametrize("use_chromium", [True, False], ids=["chromium", "legacy"])
 def test_launch(use_chromium, testdir, httpserver):
     httpserver.serve_content(content="<h1>Success!</h1>")
     file_test = testdir.makepyfile(
         """
         import pytest
```

### Comparing `pytest-selenium-4.0.0/testing/test_firefox.py` & `pytest_selenium-4.0.1/testing/test_firefox.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_metadata.py` & `pytest_selenium-4.0.1/testing/test_metadata.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-from contextlib import ExitStack as does_not_raise
-
 import pytest
 
 pytestmark = pytest.mark.nondestructive
 
 
 def test_metadata_default_host_port(testdir):
     host = "localhost"
@@ -21,38 +19,31 @@
     """.format(
             host, port
         )
     )
     testdir.quick_qa("--driver", "Remote", file_test, passed=1)
 
 
-@pytest.mark.parametrize(
-    ("host_arg_name", "port_arg_name", "context"),
-    [
-        ("--selenium-host", "--selenium-port", does_not_raise()),
-        ("--host", "--port", pytest.warns(DeprecationWarning)),
-    ],
-)
-def test_metadata_host_port(testdir, host_arg_name, port_arg_name, context):
+def test_metadata_host_port(testdir):
     host = "notlocalhost"
     port = "4441"
     file_test = testdir.makepyfile(
         """
         import pytest
         @pytest.mark.nondestructive
         def test_pass(metadata):
             assert metadata['Server'] == '{}:{}'
     """.format(
             host, port
         )
     )
-    with context:
-        testdir.quick_qa(
-            "--driver",
-            "Remote",
-            host_arg_name,
-            host,
-            port_arg_name,
-            port,
-            file_test,
-            passed=1,
-        )
+
+    testdir.quick_qa(
+        "--driver",
+        "Remote",
+        "--selenium-host",
+        host,
+        "--selenium-port",
+        port,
+        file_test,
+        passed=1,
+    )
```

### Comparing `pytest-selenium-4.0.0/testing/test_report.py` & `pytest_selenium-4.0.1/testing/test_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 # -*- encoding: utf-8 -*-
 
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import re
-from packaging.version import Version
 
 import pytest
-from pytest_html import __version__ as PYTEST_HTML_VERSION
+
 
 pytestmark = pytest.mark.nondestructive
 
 URL_LINK = '<a class="url" href="{0}/" target="_blank">URL</a>'
 
-if Version(PYTEST_HTML_VERSION) < Version("2.0.0"):
-    SCREENSHOT_LINK_REGEX = '<a class="image" href=".*" target="_blank">Screenshot</a>'
-    SCREENSHOT_REGEX = '<div class="image"><a href=".*"><img src=".*"/></a></div>'
-else:
-    SCREENSHOT_LINK_REGEX = (
-        '<a class="image" href=".*" target="_blank"><img src=".*"/></a>'
-    )
-    SCREENSHOT_REGEX = '<div class="image"><a class="image" href=".*" target="_blank">'
-    '<img src=".*"/></a></div>'
+SCREENSHOT_LINK_REGEX = '<a class="image" href=".*" target="_blank"><img src=".*"/></a>'
+SCREENSHOT_REGEX = '<div class="image"><a class="image" href=".*" target="_blank">'
+'<img src=".*"/></a></div>'
 
 LOGS_REGEX = '<a class="text" href=".*" target="_blank">.* Log</a>'
 HTML_REGEX = '<a class="text" href=".*" target="_blank">HTML</a>'
 
 
 def run(testdir, *args):
     testdir.makepyfile(
```

### Comparing `pytest-selenium-4.0.0/testing/test_safari.py` & `pytest_selenium-4.0.1/testing/test_safari.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_saucelabs.py` & `pytest_selenium-4.0.1/testing/test_saucelabs.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,20 @@
 
     capabilities = {"browserName": "chrome"}
     variables = testdir.makefile(
         ".json", '{{"capabilities": {}}}'.format(json.dumps(capabilities))
     )
 
     testdir.quick_qa(
-        "--driver", "saucelabs", "--variables", variables, file_test, passed=1
+        "--driver",
+        "saucelabs",
+        "--variables",
+        variables,
+        file_test,
+        passed=1,
     )
 
 
 def test_empty_sauce_options(monkeypatch, testdir):
     capabilities = {"browserName": "chrome"}
     expected = {"name": "test_empty_sauce_options.test_sauce_capabilities"}
     run_w3c_sauce_test(capabilities, expected, monkeypatch, testdir)
```

### Comparing `pytest-selenium-4.0.0/testing/test_testingbot.py` & `pytest_selenium-4.0.1/testing/test_testingbot.py`

 * *Files identical despite different names*

### Comparing `pytest-selenium-4.0.0/testing/test_webdriver.py` & `pytest_selenium-4.0.1/testing/test_webdriver.py`

 * *Files identical despite different names*

