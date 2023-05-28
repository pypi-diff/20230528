# Comparing `tmp/poeblix-0.8.1.tar.gz` & `tmp/poeblix-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poeblix-0.8.1.tar", max compression
+gzip compressed data, was "poeblix-0.9.tar", max compression
```

## Comparing `poeblix-0.8.1.tar` & `poeblix-0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rwxr-xr-x   0        0        0     1084 2022-08-03 17:49:48.499327 poeblix-0.8.1/LICENSE
--rwxr-xr-x   0        0        0     7293 2023-03-06 04:28:09.224214 poeblix-0.8.1/README.md
--rwxr-xr-x   0        0        0     1839 2023-03-21 16:26:21.803907 poeblix-0.8.1/pyproject.toml
--rwxr-xr-x   0        0        0        0 2022-07-18 19:58:54.454254 poeblix-0.8.1/src/poeblix/__init__.py
--rwxr-xr-x   0        0        0    12813 2022-12-10 17:55:43.625877 poeblix-0.8.1/src/poeblix/plugins.py
--rwxr-xr-x   0        0        0        0 2022-07-18 19:58:54.455254 poeblix-0.8.1/src/poeblix/util/__init__.py
--rwxr-xr-x   0        0        0     2741 2023-03-06 04:23:43.126561 poeblix-0.8.1/src/poeblix/util/util.py
--rwxr-xr-x   0        0        0     4365 2023-03-21 16:25:04.421609 poeblix-0.8.1/src/poeblix/validatedocker.py
--rwxr-xr-x   0        0        0     9021 2023-03-21 16:24:41.702416 poeblix-0.8.1/src/poeblix/validatewheel.py
--rw-r--r--   0        0        0     8206 1970-01-01 00:00:00.000000 poeblix-0.8.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1063 2023-05-28 19:54:30.665847 poeblix-0.9/LICENSE
+-rwxr-xr-x   0        0        0     7098 2023-05-28 19:54:30.665847 poeblix-0.9/README.md
+-rwxr-xr-x   0        0        0     1835 2023-05-28 20:19:20.881322 poeblix-0.9/pyproject.toml
+-rwxr-xr-x   0        0        0        0 2022-07-18 19:58:54.454254 poeblix-0.9/src/poeblix/__init__.py
+-rwxr-xr-x   0        0        0    12545 2023-05-28 19:54:30.666846 poeblix-0.9/src/poeblix/plugins.py
+-rwxr-xr-x   0        0        0        0 2022-07-18 19:58:54.455254 poeblix-0.9/src/poeblix/util/__init__.py
+-rwxr-xr-x   0        0        0     2678 2023-05-28 19:54:30.667846 poeblix-0.9/src/poeblix/util/util.py
+-rwxr-xr-x   0        0        0     4259 2023-05-28 19:54:30.667846 poeblix-0.9/src/poeblix/validatedocker.py
+-rwxr-xr-x   0        0        0     9033 2023-05-28 19:54:30.668846 poeblix-0.9/src/poeblix/validatewheel.py
+-rw-r--r--   0        0        0     8056 1970-01-01 00:00:00.000000 poeblix-0.9/PKG-INFO
```

### Comparing `poeblix-0.8.1/LICENSE` & `poeblix-0.9/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 spoorn
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 spoorn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `poeblix-0.8.1/README.md` & `poeblix-0.9/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,195 +1,217 @@
-# poeblix
-Poetry Plugin that adds various features that extend the `poetry` command such as building wheel files with locked dependencies, and validations of wheel/docker containers.
-
-Supports poetry versions `1.2+`
-
-# Overview
-These contain custom poetry plugins that enable functionality not available in the official distribution of poetry.  These include:
-
-1. Using the Lock file to build a wheel file with pinned dependencies
-2. Support for data_files (like with setup.py) such as jupyter extensions or font files
-3. Validating a wheel file is consistent with dependencies specified in pyproject.toml/poetry.lock
-4. Validating a docker container's `pip freeze` contains dependencies as specified in pyproject.toml/poetry.lock
-
-These are not supported in Poetry due to debate in the community: https://github.com/python-poetry/poetry/issues/890, https://github.com/python-poetry/poetry/issues/4013, https://github.com/python-poetry/poetry/issues/2778
-
-## Deterministic builds and environments
-
-Poetry guarantees deterministic installations and environments thanks
-to the `poetry.lock` file, which is where it stores the exact versions
-of all the dependencies needed to install a package. However, this doesn't
-occurs when wheel or package artifacts are build using `poetry build`
-command.
-
-To build a package, poetry uses the direct dependencies set in the
-`pyproject.toml` and not all the other dependencies required to install
-a package. For example, if `pyproject.toml` defines `pandas = "1.4.2"`
-as dependency but `poetry.lock` also says that `pandas` requires of
-`numpy-1.22.4`, poetry will build a package with `pandas` as dependency
-but not with `numpy`.
-
-Another problem that exists is that `pyproject.toml` can contain dependencies
-with ranges of versions while `poetry.lock` has pinned versions. For instance,
-if `pyproject.toml` has as dependency `pandas = ">=1.3"` but `poetry.lock`
-sets `pandas-1.4.2`, poetry will build a package with the dependency
-`Requires-Dist: pandas (>=0.1.3,<0.2.0)`. When the package is installed,
-the resolver will install the newest package of `pandas` which its version
-number is greater than or equal to `0.1.3` and lower than `0.2.0`.
-
-Summing this up, the same python package created with `poetry build` and
-installed several times won't install the same dependencies, making impossible
-to have deterministic installations.
-
-This plugin solves these problems building python packages that use the
-dependencies defined in the `poetry.lock`.
-
-
-# How to Use
-
-### Prerequisite
-
-Poetry Plugins are only supported in 1.2.0+ which, at the moment (5/29/22), can only be installed when using the [new poetry installer](https://python-poetry.org/docs/#installation)
-
-```commandline
-# You can update poetry using
-poetry self update
-```
-
-## Installation
-
-You can add the plugin via poetry's CLI:
-
-```commandline
-poetry self add poeblix
-```
-
-_For <= 1.2_:
-
-```commandline
-poetry plugin add poeblix
-```
-
-Or install directly from source/wheel, then add with the same above command using the absolute path to the built dist
-
-To update the plugin:
-
-```commandline
-# Update to latest
-poetry self add poeblix@latest
-
-# Update to specific version
-poetry self add poeblix==<version>
-```
-
-You should now see the blix* commands if you run `poetry list`
-
-## Usage
-
-1. To build a wheel from your package (pyproject.toml dependencies have precedence over poetry.lock ones, by default)
-
-```commandline
-poetry blixbuild
-
-# Note: Options below are also available as part of the `blixvalidatewheel` and `blixvalidatedocker` commands
-
-# To disable using lock file for building wheel and only use pyproject.toml
-poetry blixbuild --no-lock
-
-# Uses lock dependencies only which are pinned to exact versions, instead of pyproject.toml
-poetry blixbuild --only-lock
-
-# Specify additional dependency groups to include as Requires-Dist in the wheel
-poetry blixbuild --with-groups=dev,integ,etc.
-```
-
-
-2. Validate a wheel file has consistent dependencies and data_files as specified in pyproject.toml/poetry.lock
-
-```commandline
-poetry blixvalidatewheel <path-to-wheel>
-
-# Disable using lock file for validation
-poetry blixvalidatewheel --no-lock <path-to-wheel>
-```
-
-_Note: this validates consistency in both directions_
-
-3. Validate a docker container contains dependencies in a `pip freeze` as specified in pyproject.toml/poetry.lock
-
-```commandline
-poetry blixvalidatedocker <docker-container-ID>
-
-# Disable using lock file for validation
-poetry blixvalidatedocker --no-lock <docker-container-ID>
-```
-
-_Note: this only validates the docker container contains dependencies in the project, but not the other direction_
-
-Here's an example series of commands to start up a temporary docker container using its tag, validate it, then stop the temporary container
-
-```
-# This will output the newly running container id
-docker run --entrypoint=bash -it -d <docker-image-tag>
-
-# Then validate the running docker container, and stop it when done
-poetry blixvalidatedocker <container-id>
-docker stop <container-id>
-```
-
-4. Adding data_files to pyproject.toml to mimic data_files in setup.py:
-
-```yaml
-...
-
-[tool.blix.data]
-data_files = [
-    { destination = "share/data/", from = [ "data_files/test.txt", "data_files/anotherfile" ] },
-    { destination = "share/data/threes", from = [ "data_files/athirdfile" ] }
-]
-
-...
-```
-
-data_files should be under the `[tool.blix.data]` category and is a list of objects, each containing the `destination` data folder, and a `from` list of files to add to the destination data folder.
-
-_Note: the destination is a relative path that installs data to relative to the [installation prefix](https://docs.python.org/3/distutils/setupscript.html#installing-additional-files)_
-
-Example: https://github.com/spoorn/poeblix/blob/main/test/positive_cases/happy_case_example/pyproject.toml
-
-5. For more help on each command, use the --help argument
-
-```commandline
-poetry blixbuild --help
-poetry blixvalidatewheel --help
-poetry blixvalidatedocker --help
-```
-
-# Development
-
-```bash
-# Make a virtual environment on Python 3.9
-# If using virtualenvwrapper, run `mkvirtualenv -p python3.9 venv`
-virtualenv -p python3.9 venv
-
-# Or activate existing virtualenv
-# If using virtualenvwrapper, run `workon venv`
-source venv/bin/activate
-
-# installs the plugin in editable mode for easier testing via `poetry install`
-./devtool bootstrap
-
-# Lint checks
-./devtool lint
-
-# Tests
-./devtool test
-
-# Run all checks and tests
-./devtool all
-```
-
-**plugins.py** : contains our plugin that adds the `poetry blixbuild` command for building our wheel file
-
-**validatewheel.py**: adds a `poetry blixvalidatewheel` command that validates a wheel file contains the Required Dist as specified in pyproject.toml/poetry.lock
-
-**validatedocker.py** : adds a command that validates a docker file contains dependencies as specified in pyproject.toml and poetry.lock.  This does *NOT* validate that they are exactly matching, but rather that all dependencies in pyproject.toml/poetry.lock exist in the docker container on the correct versions.  The docker image may contain more extra dependencies
+Metadata-Version: 2.1
+Name: poeblix
+Version: 0.9
+Summary: Poetry plugin that adds support for building wheel files using the poetry.lock file, and data_files just like in setup.py
+Home-page: https://github.com/spoorn/poeblix
+Keywords: poeblix,utility,poetry,plugin,poetry-plugin,wheel,distribution,data_files
+Author: spoorn
+Author-email: spookump@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: poetry (>=1.2.0rc1,<2.0)
+Project-URL: Repository, https://github.com/spoorn/poeblix
+Description-Content-Type: text/markdown
+
+# poeblix
+Poetry Plugin that adds various features that extend the `poetry` command such as building wheel files with locked dependencies, and validations of wheel/docker containers.
+
+Supports poetry versions `1.2+`
+
+# Overview
+These contain custom poetry plugins that enable functionality not available in the official distribution of poetry.  These include:
+
+1. Using the Lock file to build a wheel file with pinned dependencies
+2. Support for data_files (like with setup.py) such as jupyter extensions or font files
+3. Validating a wheel file is consistent with dependencies specified in pyproject.toml/poetry.lock
+4. Validating a docker container's `pip freeze` contains dependencies as specified in pyproject.toml/poetry.lock
+
+These are not supported in Poetry due to debate in the community: https://github.com/python-poetry/poetry/issues/890, https://github.com/python-poetry/poetry/issues/4013, https://github.com/python-poetry/poetry/issues/2778
+
+## Deterministic builds and environments
+
+Poetry guarantees deterministic installations and environments thanks
+to the `poetry.lock` file, which is where it stores the exact versions
+of all the dependencies needed to install a package. However, this doesn't
+occurs when wheel or package artifacts are build using `poetry build`
+command.
+
+To build a package, poetry uses the direct dependencies set in the
+`pyproject.toml` and not all the other dependencies required to install
+a package. For example, if `pyproject.toml` defines `pandas = "1.4.2"`
+as dependency but `poetry.lock` also says that `pandas` requires of
+`numpy-1.22.4`, poetry will build a package with `pandas` as dependency
+but not with `numpy`.
+
+Another problem that exists is that `pyproject.toml` can contain dependencies
+with ranges of versions while `poetry.lock` has pinned versions. For instance,
+if `pyproject.toml` has as dependency `pandas = ">=1.3"` but `poetry.lock`
+sets `pandas-1.4.2`, poetry will build a package with the dependency
+`Requires-Dist: pandas (>=0.1.3,<0.2.0)`. When the package is installed,
+the resolver will install the newest package of `pandas` which its version
+number is greater than or equal to `0.1.3` and lower than `0.2.0`.
+
+Summing this up, the same python package created with `poetry build` and
+installed several times won't install the same dependencies, making impossible
+to have deterministic installations.
+
+This plugin solves these problems building python packages that use the
+dependencies defined in the `poetry.lock`.
+
+
+# How to Use
+
+### Prerequisite
+
+Poetry Plugins are only supported in 1.2.0+ which, at the moment (5/29/22), can only be installed when using the [new poetry installer](https://python-poetry.org/docs/#installation)
+
+```commandline
+# You can update poetry using
+poetry self update
+```
+
+## Installation
+
+You can add the plugin via poetry's CLI:
+
+```commandline
+poetry self add poeblix
+```
+
+_For <= 1.2_:
+
+```commandline
+poetry plugin add poeblix
+```
+
+Or install directly from source/wheel, then add with the same above command using the absolute path to the built dist
+
+To update the plugin:
+
+```commandline
+# Update to latest
+poetry self add poeblix@latest
+
+# Update to specific version
+poetry self add poeblix==<version>
+```
+
+You should now see the blix* commands if you run `poetry list`
+
+## Usage
+
+1. To build a wheel from your package (pyproject.toml dependencies have precedence over poetry.lock ones, by default)
+
+```commandline
+poetry blixbuild
+
+# Note: Options below are also available as part of the `blixvalidatewheel` and `blixvalidatedocker` commands
+
+# To disable using lock file for building wheel and only use pyproject.toml
+poetry blixbuild --no-lock
+
+# Uses lock dependencies only which are pinned to exact versions, instead of pyproject.toml
+poetry blixbuild --only-lock
+
+# Specify additional dependency groups to include as Requires-Dist in the wheel
+poetry blixbuild --with-groups=dev,integ,etc.
+```
+
+
+2. Validate a wheel file has consistent dependencies and data_files as specified in pyproject.toml/poetry.lock
+
+```commandline
+poetry blixvalidatewheel <path-to-wheel>
+
+# Disable using lock file for validation
+poetry blixvalidatewheel --no-lock <path-to-wheel>
+```
+
+_Note: this validates consistency in both directions_
+
+3. Validate a docker container contains dependencies in a `pip freeze` as specified in pyproject.toml/poetry.lock
+
+```commandline
+poetry blixvalidatedocker <docker-container-ID>
+
+# Disable using lock file for validation
+poetry blixvalidatedocker --no-lock <docker-container-ID>
+```
+
+_Note: this only validates the docker container contains dependencies in the project, but not the other direction_
+
+Here's an example series of commands to start up a temporary docker container using its tag, validate it, then stop the temporary container
+
+```
+# This will output the newly running container id
+docker run --entrypoint=bash -it -d <docker-image-tag>
+
+# Then validate the running docker container, and stop it when done
+poetry blixvalidatedocker <container-id>
+docker stop <container-id>
+```
+
+4. Adding data_files to pyproject.toml to mimic data_files in setup.py:
+
+```yaml
+...
+
+[tool.blix.data]
+data_files = [
+    { destination = "share/data/", from = [ "data_files/test.txt", "data_files/anotherfile" ] },
+    { destination = "share/data/threes", from = [ "data_files/athirdfile" ] }
+]
+
+...
+```
+
+data_files should be under the `[tool.blix.data]` category and is a list of objects, each containing the `destination` data folder, and a `from` list of files to add to the destination data folder.
+
+_Note: the destination is a relative path that installs data to relative to the [installation prefix](https://docs.python.org/3/distutils/setupscript.html#installing-additional-files)_
+
+Example: https://github.com/spoorn/poeblix/blob/main/test/positive_cases/happy_case_example/pyproject.toml
+
+5. For more help on each command, use the --help argument
+
+```commandline
+poetry blixbuild --help
+poetry blixvalidatewheel --help
+poetry blixvalidatedocker --help
+```
+
+# Development
+
+```bash
+# Make a virtual environment on Python 3.9
+# If using virtualenvwrapper, run `mkvirtualenv -p python3.9 venv`
+virtualenv -p python3.9 venv
+
+# Or activate existing virtualenv
+# If using virtualenvwrapper, run `workon venv`
+source venv/bin/activate
+
+# installs the plugin in editable mode for easier testing via `poetry install`
+./devtool bootstrap
+
+# Lint checks
+./devtool lint
+
+# Tests
+./devtool test
+
+# Run all checks and tests
+./devtool all
+```
+
+**plugins.py** : contains our plugin that adds the `poetry blixbuild` command for building our wheel file
+
+**validatewheel.py**: adds a `poetry blixvalidatewheel` command that validates a wheel file contains the Required Dist as specified in pyproject.toml/poetry.lock
+
+**validatedocker.py** : adds a command that validates a docker file contains dependencies as specified in pyproject.toml and poetry.lock.  This does *NOT* validate that they are exactly matching, but rather that all dependencies in pyproject.toml/poetry.lock exist in the docker container on the correct versions.  The docker image may contain more extra dependencies
+
```

### Comparing `poeblix-0.8.1/src/poeblix/plugins.py` & `poeblix-0.9/src/poeblix/plugins.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,284 +1,284 @@
-from __future__ import annotations
-
-import os
-import shutil
-import zipfile
-from pathlib import Path
-from typing import Optional, List, Dict, cast
-
-from cleo.helpers import option
-from cleo.io.inputs.option import Option
-
-# For fixing https://github.com/python-poetry/poetry/issues/5216
-from packaging.tags import sys_tags  # noqa
-from poetry.console.application import Application
-from poetry.console.commands.env_command import EnvCommand
-from poetry.core.masonry.builders.wheel import WheelBuilder, logger
-from poetry.core.poetry import Poetry
-from poetry.packages import Locker
-from poetry.plugins.application_plugin import ApplicationPlugin
-from poetry.utils.env import Env
-
-from poeblix.util import util
-
-"""
-This Plugin introduces a new command `poetry blix` that extends upon the regular `poetry build` command,
-but allows for building the wheel file using the poetry.lock file and supports adding data_files just like in setup.py:
-https://docs.python.org/3/distutils/setupscript.html#installing-additional-files
-"""
-
-
-class BlixWheelBuilder(WheelBuilder):
-    """
-    This extends on Poetry's wheel builder which is invoked via `poetry build -f wheel`.  Adds features such as
-    supporting data_files in the wheel archive, and using the lock file to pin dependencies in the wheel.
-
-    These features are not supported in the official Poetry commands as they have either been deemed by the community
-    as not commonly necessary, or not yet implemented.
-
-    For example, data_files are deprecated even in setup.py: https://github.com/python-poetry/poetry/issues/890
-    Using lock file to build the wheel: https://github.com/python-poetry/poetry/issues/2778
-    """
-
-    def __init__(
-        self,
-        poetry: "Poetry",
-        env: Env,
-        locker: Locker,
-        executable: str | Path | None = None,
-        data_files: Optional[List[Dict]] = None,
-        no_lock: bool = False,
-        only_lock: bool = False,
-        with_groups: Optional[List[str]] = None,
-    ) -> None:
-        super().__init__(poetry, executable=executable)  # type: ignore
-        self._env = env
-        self._locker = locker
-        self._data_files = data_files
-        self._no_lock = no_lock
-        self._only_lock = only_lock
-        self._with_groups = with_groups
-
-    def _get_abs_path(self, rel_path: str) -> Path:
-        """Transform a relative path to absolute path"""
-        abs_path = Path.joinpath(self._path, rel_path)
-
-        if not abs_path.exists():
-            raise RuntimeError(f"{abs_path} in data_files is not found.")
-
-        if not abs_path.is_file():
-            raise RuntimeError(f"{abs_path} in data_files is not a file.")
-
-        return abs_path
-
-    # Hijack _copy_dist_info and also write data folder that we wrote in prepare_metadata()
-    def _copy_dist_info(self, wheel: zipfile.ZipFile, source: Path) -> None:
-        super()._copy_dist_info(wheel, source)
-        source = source.parent / self.wheel_data_folder
-        wheel_data = Path(self.wheel_data_folder)
-        for file in source.glob("**/*"):
-            if not file.is_file():
-                continue
-
-            rel_path = file.relative_to(source)
-            target = wheel_data / rel_path
-            print(f"Copying file from {file} to wheel relative {target}")
-            self._add_file(wheel, file, target)
-
-    def prepare_metadata(self, metadata_directory: Path) -> Path:
-        """
-        The below code before super().prepare_metadata() takes locked dependencies from poetry.lock to add as
-        requirements in the wheel file we will build.
-
-        This can be removed if poetry supports https://github.com/python-poetry/poetry/issues/2778.
-        """
-        dist_info = metadata_directory / self.dist_info
-
-        if self._no_lock:
-            logger.info("Excluding lock dependencies from wheel as --no-lock was specified")
-        else:
-
-            logger.info("Adding dependencies from lock file to wheel build")
-            # There is currently a bug with poetry 1.2.0b1 where the `category` field in poetry.lock all gets set to
-            # "dev" for all packages.  As per https://github.com/python-poetry/poetry/issues/5702 and
-            # https://github.com/python-poetry/poetry/issues/2280, the `category` field is not accurate and will be
-            # removed.  Instead, we will read ALL packages from the locked repo, then during resolve_dependencies,
-            # filter based on dependency group which should be used going forward 1.2.0+
-            locked_repository = self._locker.locked_repository()
-            # logger.info(f"locked repo {locked_repository.packages}")
-            # for package in locked_repository.packages:
-            #     logger.info(f"Package {package.__dict__}")
-            logger.info("Resolving dependencies using poetry's solver to get rid of unneeded packages")
-            ops = util.resolve_dependencies(self._poetry, self._env, locked_repository, self._with_groups)
-
-            # logger.info(f"dependency groups: {self._poetry.package._dependency_groups}")
-
-            logger.info("Adding resolved dependencies to wheel METADATA")
-
-            # By default, 'pyproject.toml' dependencies have priority over
-            # 'poetry.lock' ones.
-            #
-            # When 'only-lock' is set, pyproject dependencies are removed
-            # using fixed versions from the lock file only.
-            #
-            # However, poetry requires that the packages listed on the
-            # 'pyproject.toml' are also on the 'poetry.lock' file,
-            # so no direct dependencies will be missed when the wheel
-            # is built. Only package versions may vary.
-
-            in_extras = {}
-            if self._only_lock:
-                # in_extras is backfilled in factory.py:
-                # https://github.com/python-poetry/poetry-core/blob/8097f67d0760bad5989219483c59339e1eed549c/src/poetry/core/factory.py#L176-L187
-                # keep a record of these so if we are building with only_lock enabled, we preserve the in_extras
-                for p in self._poetry.package.requires:
-                    in_extras[p.pretty_name] = p.in_extras
-                self._meta.requires_dist = []
-
-            requires_dist = self._meta.requires_dist
-            required_packages_names = [p.pretty_name for p in self._poetry.package.requires]
-            logger.debug(f"Adding to Wheel Requires Dist: {ops}")
-            for op in ops:
-                dep_pack = op.package
-                name = dep_pack.pretty_name
-                # Exclude python version constraints from the wheel file Required-Dist as default
-                # otherwise, most of the deps will have a verbose python version constraint with it
-                dep_pack.python_versions = "*"
-                dependency = dep_pack.to_dependency()
-                # Backfill in_extras
-                if self._only_lock and name in in_extras:
-                    dependency.in_extras.extend(in_extras[name])
-                dep = dependency.to_pep_508()
-                if self._only_lock or name not in required_packages_names:
-                    requires_dist.append(dep)
-
-        super().prepare_metadata(metadata_directory)
-
-        # After writing the metadata, also write our custom data files to the wheel data folder
-        if self._data_files:
-            logger.info("Adding data_files to WHEEL data folder")
-            for data_file in self._data_files:
-                destination = data_file["destination"]
-                sources = data_file["from"]
-
-                if Path(destination).is_absolute():
-                    raise ValueError(
-                        f"Destination path in data_files [{destination}] is absolute.  "
-                        f"Please change it to a relative path"
-                    )
-
-                # TODO: Use OS specific separator
-                if destination[-1] != "/":
-                    destination += "/"
-
-                # Note: this assumes destination is suffixed with the directory separator "/"
-                for src in sources:
-                    abs_path = self._get_abs_path(src)
-                    dest = Path.joinpath(
-                        metadata_directory, Path(self.wheel_data_folder), "data", destination + abs_path.name
-                    )
-                    print(f"Copying data files from {abs_path} to {dest}")
-                    os.makedirs(dest.parent, exist_ok=True)
-                    shutil.copy(abs_path, dest)
-
-        return dist_info
-
-
-class BlixBuildCommand(EnvCommand):
-    """
-    Our custom build command to use with the poetry CLI via `poetry blix`.
-    """
-
-    name = "blixbuild"
-    description = (
-        "Builds a wheel package with custom data files mimicking data_files in setup.py, and uses the lock file"
-    )
-
-    options: List[Option] = [
-        option(
-            "no-lock",
-            None,
-            "Disables building wheel file with lock dependencies.",
-        ),
-        option(
-            "only-lock",
-            None,
-            "Uses lock dependencies only which are pinned to exact versions, instead of pyproject.toml",
-        ),
-        option(
-            "with-groups",
-            None,
-            "Specify which dependency groups to use to build the wheel file, on top of required groups from "
-            "pyproject.toml.  Can be specified multiple times or as a comma delimited list.",
-            flag=False,
-            multiple=True,
-        ),
-    ]
-
-    # Pick up Poetry's WheelBuilder logger
-    loggers = ["poetry.core.masonry.builders.wheel"]
-
-    def handle(self) -> int:
-        util.validate_options_mutually_exclusive(self.option, "no-lock", "only-lock")
-        with_groups = []
-        for group in self.option("with-groups"):
-            with_groups.extend(group.split(","))
-
-        package = self.poetry.package
-        self.line(f"Building <c1>{package.pretty_name}</c1> (<c2>{package.version}</c2>)")
-
-        # Parse data_files
-        from tomlkit.exceptions import NonExistentKey
-
-        data_files = None
-        try:
-            """
-            Cast to dict to avoid these errors after upgrading poetry to 1.2.0b2.  It should be a dict anyways:
-
-            src/poeblix/plugins.py:169:16: error: Unsupported right operand type for in ("Union[Any, Item, Container]")
-            src/poeblix/plugins.py:170:30: error: Value of type "Union[Any, Item, Container]" is not indexable
-            src/poeblix/plugins.py:181:24: error: Argument "data_files" to "BlixWheelBuilder" has incompatible type
-                "Union[Any, Item, Container, None]"; expected "Optional[List[Dict[Any, Any]]]"
-            """
-            data_files_config = cast(dict, self.poetry.pyproject.data["tool"]["blix"]["data"])  # type: ignore
-            if "data_files" in data_files_config:
-                data_files = data_files_config["data_files"]
-                """
-                List out the data_files when printing as __str__ for tomlkit seems to have a breaking change where
-                it tries to call v.value.value for each item in the Toml Array, but the item may be a string such as
-                the "\r\n" character which will run into an error as there is no value() method on strings.
-                """
-                self.line(f"Adding data_files={[v for v in data_files]}")
-        except NonExistentKey:
-            self.line(f"[tool.blix.data] section not found in {self.poetry.file}, no data_files to process")
-
-        # Create our custom wheel builder
-        builder = BlixWheelBuilder(
-            self.poetry,
-            env=self.env,
-            locker=self.poetry.locker,
-            executable=self.env.python,
-            data_files=data_files,
-            no_lock=self.option("no-lock"),
-            only_lock=self.option("only-lock"),
-            with_groups=with_groups,
-        )
-        builder.build()
-
-        return 0
-
-
-class BlixPlugin(ApplicationPlugin):
-    def activate(self, application: Application) -> None:
-        # Custom build command via `poetry blix`
-        application.command_loader.register_factory(BlixBuildCommand.name, lambda: BlixBuildCommand())
-
-        # Validate Wheel plugin
-        from .validatewheel import ValidateWheelPlugin
-
-        application.command_loader.register_factory(ValidateWheelPlugin.name, lambda: ValidateWheelPlugin())
-
-        # Validate Docker plugin
-        from .validatedocker import ValidateDockerPlugin
-
-        application.command_loader.register_factory(ValidateDockerPlugin.name, lambda: ValidateDockerPlugin())
+from __future__ import annotations
+
+import os
+import shutil
+import zipfile
+from pathlib import Path
+from typing import Optional, List, Dict, cast
+
+from cleo.helpers import option
+from cleo.io.inputs.option import Option
+
+# For fixing https://github.com/python-poetry/poetry/issues/5216
+from packaging.tags import sys_tags  # noqa
+from poetry.console.application import Application
+from poetry.console.commands.env_command import EnvCommand
+from poetry.core.masonry.builders.wheel import WheelBuilder, logger
+from poetry.core.poetry import Poetry
+from poetry.packages import Locker
+from poetry.plugins.application_plugin import ApplicationPlugin
+from poetry.utils.env import Env
+
+from poeblix.util import util
+
+"""
+This Plugin introduces a new command `poetry blix` that extends upon the regular `poetry build` command,
+but allows for building the wheel file using the poetry.lock file and supports adding data_files just like in setup.py:
+https://docs.python.org/3/distutils/setupscript.html#installing-additional-files
+"""
+
+
+class BlixWheelBuilder(WheelBuilder):
+    """
+    This extends on Poetry's wheel builder which is invoked via `poetry build -f wheel`.  Adds features such as
+    supporting data_files in the wheel archive, and using the lock file to pin dependencies in the wheel.
+
+    These features are not supported in the official Poetry commands as they have either been deemed by the community
+    as not commonly necessary, or not yet implemented.
+
+    For example, data_files are deprecated even in setup.py: https://github.com/python-poetry/poetry/issues/890
+    Using lock file to build the wheel: https://github.com/python-poetry/poetry/issues/2778
+    """
+
+    def __init__(
+        self,
+        poetry: "Poetry",
+        env: Env,
+        locker: Locker,
+        executable: str | Path | None = None,
+        data_files: Optional[List[Dict]] = None,
+        no_lock: bool = False,
+        only_lock: bool = False,
+        with_groups: Optional[List[str]] = None,
+    ) -> None:
+        super().__init__(poetry, executable=executable)  # type: ignore
+        self._env = env
+        self._locker = locker
+        self._data_files = data_files
+        self._no_lock = no_lock
+        self._only_lock = only_lock
+        self._with_groups = with_groups
+
+    def _get_abs_path(self, rel_path: str) -> Path:
+        """Transform a relative path to absolute path"""
+        abs_path = Path.joinpath(self._path, rel_path)
+
+        if not abs_path.exists():
+            raise RuntimeError(f"{abs_path} in data_files is not found.")
+
+        if not abs_path.is_file():
+            raise RuntimeError(f"{abs_path} in data_files is not a file.")
+
+        return abs_path
+
+    # Hijack _copy_dist_info and also write data folder that we wrote in prepare_metadata()
+    def _copy_dist_info(self, wheel: zipfile.ZipFile, source: Path) -> None:
+        super()._copy_dist_info(wheel, source)
+        source = source.parent / self.wheel_data_folder
+        wheel_data = Path(self.wheel_data_folder)
+        for file in source.glob("**/*"):
+            if not file.is_file():
+                continue
+
+            rel_path = file.relative_to(source)
+            target = wheel_data / rel_path
+            print(f"Copying file from {file} to wheel relative {target}")
+            self._add_file(wheel, file, target)
+
+    def prepare_metadata(self, metadata_directory: Path) -> Path:
+        """
+        The below code before super().prepare_metadata() takes locked dependencies from poetry.lock to add as
+        requirements in the wheel file we will build.
+
+        This can be removed if poetry supports https://github.com/python-poetry/poetry/issues/2778.
+        """
+        dist_info = metadata_directory / self.dist_info
+
+        if self._no_lock:
+            logger.info("Excluding lock dependencies from wheel as --no-lock was specified")
+        else:
+
+            logger.info("Adding dependencies from lock file to wheel build")
+            # There is currently a bug with poetry 1.2.0b1 where the `category` field in poetry.lock all gets set to
+            # "dev" for all packages.  As per https://github.com/python-poetry/poetry/issues/5702 and
+            # https://github.com/python-poetry/poetry/issues/2280, the `category` field is not accurate and will be
+            # removed.  Instead, we will read ALL packages from the locked repo, then during resolve_dependencies,
+            # filter based on dependency group which should be used going forward 1.2.0+
+            locked_repository = self._locker.locked_repository()
+            # logger.info(f"locked repo {locked_repository.packages}")
+            # for package in locked_repository.packages:
+            #     logger.info(f"Package {package.__dict__}")
+            logger.info("Resolving dependencies using poetry's solver to get rid of unneeded packages")
+            ops = util.resolve_dependencies(self._poetry, self._env, locked_repository, self._with_groups)
+
+            # logger.info(f"dependency groups: {self._poetry.package._dependency_groups}")
+
+            logger.info("Adding resolved dependencies to wheel METADATA")
+
+            # By default, 'pyproject.toml' dependencies have priority over
+            # 'poetry.lock' ones.
+            #
+            # When 'only-lock' is set, pyproject dependencies are removed
+            # using fixed versions from the lock file only.
+            #
+            # However, poetry requires that the packages listed on the
+            # 'pyproject.toml' are also on the 'poetry.lock' file,
+            # so no direct dependencies will be missed when the wheel
+            # is built. Only package versions may vary.
+
+            in_extras = {}
+            if self._only_lock:
+                # in_extras is backfilled in factory.py:
+                # https://github.com/python-poetry/poetry-core/blob/8097f67d0760bad5989219483c59339e1eed549c/src/poetry/core/factory.py#L176-L187
+                # keep a record of these so if we are building with only_lock enabled, we preserve the in_extras
+                for p in self._poetry.package.requires:
+                    in_extras[p.pretty_name] = p.in_extras
+                self._meta.requires_dist = []
+
+            requires_dist = self._meta.requires_dist
+            required_packages_names = [p.pretty_name.lower() for p in self._poetry.package.requires]
+            logger.debug(f"Adding to Wheel Requires Dist: {ops}")
+            for op in ops:
+                dep_pack = op.package
+                name = dep_pack.pretty_name
+                # Exclude python version constraints from the wheel file Required-Dist as default
+                # otherwise, most of the deps will have a verbose python version constraint with it
+                dep_pack.python_versions = "*"
+                dependency = dep_pack.to_dependency()
+                # Backfill in_extras
+                if self._only_lock and name in in_extras:
+                    dependency.in_extras.extend(in_extras[name])
+                dep = dependency.to_pep_508()
+                if self._only_lock or name.lower() not in required_packages_names:
+                    requires_dist.append(dep)
+
+        super().prepare_metadata(metadata_directory)
+
+        # After writing the metadata, also write our custom data files to the wheel data folder
+        if self._data_files:
+            logger.info("Adding data_files to WHEEL data folder")
+            for data_file in self._data_files:
+                destination = data_file["destination"]
+                sources = data_file["from"]
+
+                if Path(destination).is_absolute():
+                    raise ValueError(
+                        f"Destination path in data_files [{destination}] is absolute.  "
+                        f"Please change it to a relative path"
+                    )
+
+                # TODO: Use OS specific separator
+                if destination[-1] != "/":
+                    destination += "/"
+
+                # Note: this assumes destination is suffixed with the directory separator "/"
+                for src in sources:
+                    abs_path = self._get_abs_path(src)
+                    dest = Path.joinpath(
+                        metadata_directory, Path(self.wheel_data_folder), "data", destination + abs_path.name
+                    )
+                    print(f"Copying data files from {abs_path} to {dest}")
+                    os.makedirs(dest.parent, exist_ok=True)
+                    shutil.copy(abs_path, dest)
+
+        return dist_info
+
+
+class BlixBuildCommand(EnvCommand):
+    """
+    Our custom build command to use with the poetry CLI via `poetry blix`.
+    """
+
+    name = "blixbuild"
+    description = (
+        "Builds a wheel package with custom data files mimicking data_files in setup.py, and uses the lock file"
+    )
+
+    options: List[Option] = [
+        option(
+            "no-lock",
+            None,
+            "Disables building wheel file with lock dependencies.",
+        ),
+        option(
+            "only-lock",
+            None,
+            "Uses lock dependencies only which are pinned to exact versions, instead of pyproject.toml",
+        ),
+        option(
+            "with-groups",
+            None,
+            "Specify which dependency groups to use to build the wheel file, on top of required groups from "
+            "pyproject.toml.  Can be specified multiple times or as a comma delimited list.",
+            flag=False,
+            multiple=True,
+        ),
+    ]
+
+    # Pick up Poetry's WheelBuilder logger
+    loggers = ["poetry.core.masonry.builders.wheel"]
+
+    def handle(self) -> int:
+        util.validate_options_mutually_exclusive(self.option, "no-lock", "only-lock")
+        with_groups = []
+        for group in self.option("with-groups"):
+            with_groups.extend(group.split(","))
+
+        package = self.poetry.package
+        self.line(f"Building <c1>{package.pretty_name}</c1> (<c2>{package.version}</c2>)")
+
+        # Parse data_files
+        from tomlkit.exceptions import NonExistentKey
+
+        data_files = None
+        try:
+            """
+            Cast to dict to avoid these errors after upgrading poetry to 1.2.0b2.  It should be a dict anyways:
+
+            src/poeblix/plugins.py:169:16: error: Unsupported right operand type for in ("Union[Any, Item, Container]")
+            src/poeblix/plugins.py:170:30: error: Value of type "Union[Any, Item, Container]" is not indexable
+            src/poeblix/plugins.py:181:24: error: Argument "data_files" to "BlixWheelBuilder" has incompatible type
+                "Union[Any, Item, Container, None]"; expected "Optional[List[Dict[Any, Any]]]"
+            """
+            data_files_config = cast(dict, self.poetry.pyproject.data["tool"]["blix"]["data"])  # type: ignore
+            if "data_files" in data_files_config:
+                data_files = data_files_config["data_files"]
+                """
+                List out the data_files when printing as __str__ for tomlkit seems to have a breaking change where
+                it tries to call v.value.value for each item in the Toml Array, but the item may be a string such as
+                the "\r\n" character which will run into an error as there is no value() method on strings.
+                """
+                self.line(f"Adding data_files={[v for v in data_files]}")
+        except NonExistentKey:
+            self.line(f"[tool.blix.data] section not found in {self.poetry.file}, no data_files to process")
+
+        # Create our custom wheel builder
+        builder = BlixWheelBuilder(
+            self.poetry,
+            env=self.env,
+            locker=self.poetry.locker,
+            executable=self.env.python,
+            data_files=data_files,
+            no_lock=self.option("no-lock"),
+            only_lock=self.option("only-lock"),
+            with_groups=with_groups,
+        )
+        builder.build()
+
+        return 0
+
+
+class BlixPlugin(ApplicationPlugin):
+    def activate(self, application: Application) -> None:
+        # Custom build command via `poetry blix`
+        application.command_loader.register_factory(BlixBuildCommand.name, lambda: BlixBuildCommand())
+
+        # Validate Wheel plugin
+        from .validatewheel import ValidateWheelPlugin
+
+        application.command_loader.register_factory(ValidateWheelPlugin.name, lambda: ValidateWheelPlugin())
+
+        # Validate Docker plugin
+        from .validatedocker import ValidateDockerPlugin
+
+        application.command_loader.register_factory(ValidateDockerPlugin.name, lambda: ValidateDockerPlugin())
```

### Comparing `poeblix-0.8.1/src/poeblix/util/util.py` & `poeblix-0.9/src/poeblix/util/util.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-from typing import Sequence, Callable, List, Optional
-
-from cleo.io.null_io import NullIO
-
-# For fixing https://github.com/python-poetry/poetry/issues/5216
-from packaging.tags import sys_tags  # noqa
-from poetry.core.poetry import Poetry
-from poetry.installation.operations.operation import Operation
-from poetry.puzzle import Solver
-from poetry.repositories import RepositoryPool
-from poetry.repositories import Repository
-from poetry.repositories.installed_repository import InstalledRepository
-from poetry.utils.env import Env
-
-
-def resolve_dependencies(
-    poetry: "Poetry", env: Env, locked_repository: Repository, with_groups: Optional[List[str]] = None
-) -> Sequence[Operation]:
-    """
-    This uses poetry's solver to resolve dependencies and filters out packages from the lock file which are not
-    needed, such as packages that are not for our OS environment using markers (e.g. pywin32 is for Windows).
-    """
-    # Making a new repo containing the packages
-    # newly resolved and the ones from the current lock file
-    repo = Repository(name="poetry-locked")
-    for package in locked_repository.packages:
-        if not package.is_direct_origin() and not repo.has_package(package):
-            repo.add_package(package)
-
-    pool = RepositoryPool(ignore_repository_names=True)
-    pool.add_repository(repo)
-
-    # Run through poetry's dependency resolver.  Only uses the default/main `dependencies` in pyproject.toml, not
-    # dev dependencies or other groups.  If we want to support more groups in the wheel file, we can expand on the
-    # CLI with more options.
-    # See https://github.com/python-poetry/poetry/blob/master/src/poetry/installation/installer.py#L34 for poetry's
-    # usage of this
-    # TODO: Add support for adding more groups
-    groups = set(["default", "main"] + (with_groups if with_groups else []))
-
-    solver = Solver(
-        poetry.package.with_dependency_groups(groups=groups, only=True),
-        pool,
-        InstalledRepository.load(env).packages,
-        locked_repository.packages,
-        NullIO(),
-    )
-
-    # Everything is resolved at this point, so we no longer need
-    # to load deferred dependencies (i.e. VCS, URL and path dependencies)
-    solver.provider.load_deferred(False)
-
-    with solver.use_environment(env):
-        ops = solver.solve(use_latest=[]).calculate_operations(
-            with_uninstalls=False,
-            synchronize=False,
-        )
-    return ops
-
-
-def validate_options_mutually_exclusive(option_func: Callable, option1: str, option2: str) -> None:
-    if option_func(option1) and option_func(option2):
-        raise RuntimeError(f"'{option1}' and '{option2}' options are incompatible")
+from typing import Sequence, Callable, List, Optional
+
+from cleo.io.null_io import NullIO
+
+# For fixing https://github.com/python-poetry/poetry/issues/5216
+from packaging.tags import sys_tags  # noqa
+from poetry.core.poetry import Poetry
+from poetry.installation.operations.operation import Operation
+from poetry.puzzle import Solver
+from poetry.repositories import RepositoryPool
+from poetry.repositories import Repository
+from poetry.repositories.installed_repository import InstalledRepository
+from poetry.utils.env import Env
+
+
+def resolve_dependencies(
+    poetry: "Poetry", env: Env, locked_repository: Repository, with_groups: Optional[List[str]] = None
+) -> Sequence[Operation]:
+    """
+    This uses poetry's solver to resolve dependencies and filters out packages from the lock file which are not
+    needed, such as packages that are not for our OS environment using markers (e.g. pywin32 is for Windows).
+    """
+    # Making a new repo containing the packages
+    # newly resolved and the ones from the current lock file
+    repo = Repository(name="poetry-locked")
+    for package in locked_repository.packages:
+        if not package.is_direct_origin() and not repo.has_package(package):
+            repo.add_package(package)
+
+    pool = RepositoryPool(ignore_repository_names=True)
+    pool.add_repository(repo)
+
+    # Run through poetry's dependency resolver.  Only uses the default/main `dependencies` in pyproject.toml, not
+    # dev dependencies or other groups.  If we want to support more groups in the wheel file, we can expand on the
+    # CLI with more options.
+    # See https://github.com/python-poetry/poetry/blob/master/src/poetry/installation/installer.py#L34 for poetry's
+    # usage of this
+    # TODO: Add support for adding more groups
+    groups = set(["default", "main"] + (with_groups if with_groups else []))
+
+    solver = Solver(
+        poetry.package.with_dependency_groups(groups=groups, only=True),
+        pool,
+        InstalledRepository.load(env).packages,
+        locked_repository.packages,
+        NullIO(),
+    )
+
+    # Everything is resolved at this point, so we no longer need
+    # to load deferred dependencies (i.e. VCS, URL and path dependencies)
+    solver.provider.load_deferred(False)
+
+    with solver.use_environment(env):
+        ops = solver.solve(use_latest=[]).calculate_operations(
+            with_uninstalls=False,
+            synchronize=False,
+        )
+    return ops
+
+
+def validate_options_mutually_exclusive(option_func: Callable, option1: str, option2: str) -> None:
+    if option_func(option1) and option_func(option2):
+        raise RuntimeError(f"'{option1}' and '{option2}' options are incompatible")
```

### Comparing `poeblix-0.8.1/src/poeblix/validatedocker.py` & `poeblix-0.9/src/poeblix/validatedocker.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-import subprocess
-from typing import List
-
-from cleo.helpers import argument, option
-from cleo.io.inputs.option import Option
-
-# For fixing https://github.com/python-poetry/poetry/issues/5216
-from packaging.tags import sys_tags  # noqa
-from poetry.console.commands.env_command import EnvCommand
-from poetry.core.packages.package import Package
-
-from poeblix.util import util
-
-
-class ValidateDockerPlugin(EnvCommand):
-    """
-    Validates a docker container contains dependencies defined in the pyproject.toml and poetry.lock in the project
-    this command is run.
-    """
-
-    name = "blixvalidatedocker"
-    description = (
-        "Validates a docker container contains dependencies that satisfies constraints in pyproject.toml and "
-        "poetry.lock.  By default, this validates in one direction, where dependencies specified in "
-        "pyproject.toml/poetry.lock should be present in the Docker container, but not the other way around."
-    )
-
-    arguments = [argument("containerId", "Docker Container ID")]
-
-    options: List[Option] = [
-        option(
-            "no-lock",
-            None,
-            "Disables validating lock file dependencies.",
-        ),
-        option(
-            "with-groups",
-            None,
-            "Specify which dependency groups to use to validate the wheel file, on top of required groups from "
-            "pyproject.toml.  Can be specified multiple times or as a comma delimited list.",
-            flag=False,
-            multiple=True,
-        ),
-    ]
-
-    loggers = ["poetry.core.masonry.builders.wheel"]
-
-    def _validate_pyproject_toml(self, docker_deps: dict):
-        cid = self.argument("containerId")
-        required_packages = self.poetry.package.requires
-        for package in required_packages:
-            name = package.pretty_name
-            # Defer to poetry.lock validation if dpeendency is a direct origin source such as git, local path, etc.
-            if not package.is_direct_origin() and name in docker_deps:
-                if Package(name, docker_deps[name]).satisfies(package):
-                    docker_deps.pop(name)
-                else:
-                    raise ValueError(
-                        f"Inconsistency found!  pyproject.toml specifies {name}{package.constraint}, "
-                        f"but docker container {cid} has {name}=={docker_deps[name]}"
-                    )
-
-    def _validate_poetry_lock(self, docker_deps: dict):
-        if self.option("no-lock"):
-            self.line("Skipping poetry.lock validation as --no-lock was specified")
-            return
-
-        with_groups = []
-        for group in self.option("with-groups"):
-            with_groups.extend(group.split(","))
-
-        cid = self.argument("containerId")
-        locked_repo = self.poetry.locker.locked_repository()
-        ops = util.resolve_dependencies(self.poetry, self.env, locked_repo, with_groups)
-        for op in ops:
-            dependency_package = op.package
-            name = dependency_package.pretty_name
-            version = dependency_package.version
-            if name in docker_deps:
-                proc_version = docker_deps[name]
-                if proc_version != str(version):
-                    raise ValueError(
-                        f"Inconsistency found!  poetry.lock specifies {name}=={version}, "
-                        f"but docker container {cid} has {name}=={proc_version}"
-                    )
-
-    def handle(self) -> int:
-        cid = self.argument("containerId")
-        self.line(f"Fetching 'pip freeze' from docker image {cid} and validating against pyproject.toml/poetry.lock")
-
-        docker_freeze = subprocess.check_output(f'docker exec {cid} python3 -m pip freeze | grep -v "@"', shell=True)
-        docker_deps = {
-            dsplit[0]: dsplit[1] for dsplit in (dep.split("==") for dep in docker_freeze.decode("utf-8").splitlines())
-        }
-
-        # Validate against pyproject.toml
-        self._validate_pyproject_toml(docker_deps)
-        # Validate against poetry.lock
-        self._validate_poetry_lock(docker_deps)
-
-        self.line(
-            f"Validation success!  Docker image {cid} has consistent versions with dependencies specified "
-            f"in this project"
-        )
-
-        return 0
+import subprocess
+from typing import List
+
+from cleo.helpers import argument, option
+from cleo.io.inputs.option import Option
+
+# For fixing https://github.com/python-poetry/poetry/issues/5216
+from packaging.tags import sys_tags  # noqa
+from poetry.console.commands.env_command import EnvCommand
+from poetry.core.packages.package import Package
+
+from poeblix.util import util
+
+
+class ValidateDockerPlugin(EnvCommand):
+    """
+    Validates a docker container contains dependencies defined in the pyproject.toml and poetry.lock in the project
+    this command is run.
+    """
+
+    name = "blixvalidatedocker"
+    description = (
+        "Validates a docker container contains dependencies that satisfies constraints in pyproject.toml and "
+        "poetry.lock.  By default, this validates in one direction, where dependencies specified in "
+        "pyproject.toml/poetry.lock should be present in the Docker container, but not the other way around."
+    )
+
+    arguments = [argument("containerId", "Docker Container ID")]
+
+    options: List[Option] = [
+        option(
+            "no-lock",
+            None,
+            "Disables validating lock file dependencies.",
+        ),
+        option(
+            "with-groups",
+            None,
+            "Specify which dependency groups to use to validate the wheel file, on top of required groups from "
+            "pyproject.toml.  Can be specified multiple times or as a comma delimited list.",
+            flag=False,
+            multiple=True,
+        ),
+    ]
+
+    loggers = ["poetry.core.masonry.builders.wheel"]
+
+    def _validate_pyproject_toml(self, docker_deps: dict):
+        cid = self.argument("containerId")
+        required_packages = self.poetry.package.requires
+        for package in required_packages:
+            name = package.pretty_name
+            # Defer to poetry.lock validation if dpeendency is a direct origin source such as git, local path, etc.
+            if not package.is_direct_origin() and name in docker_deps:
+                if Package(name, docker_deps[name]).satisfies(package):
+                    docker_deps.pop(name)
+                else:
+                    raise ValueError(
+                        f"Inconsistency found!  pyproject.toml specifies {name}{package.constraint}, "
+                        f"but docker container {cid} has {name}=={docker_deps[name]}"
+                    )
+
+    def _validate_poetry_lock(self, docker_deps: dict):
+        if self.option("no-lock"):
+            self.line("Skipping poetry.lock validation as --no-lock was specified")
+            return
+
+        with_groups = []
+        for group in self.option("with-groups"):
+            with_groups.extend(group.split(","))
+
+        cid = self.argument("containerId")
+        locked_repo = self.poetry.locker.locked_repository()
+        ops = util.resolve_dependencies(self.poetry, self.env, locked_repo, with_groups)
+        for op in ops:
+            dependency_package = op.package
+            name = dependency_package.pretty_name
+            version = dependency_package.version
+            if name in docker_deps:
+                proc_version = docker_deps[name]
+                if proc_version != str(version):
+                    raise ValueError(
+                        f"Inconsistency found!  poetry.lock specifies {name}=={version}, "
+                        f"but docker container {cid} has {name}=={proc_version}"
+                    )
+
+    def handle(self) -> int:
+        cid = self.argument("containerId")
+        self.line(f"Fetching 'pip freeze' from docker image {cid} and validating against pyproject.toml/poetry.lock")
+
+        docker_freeze = subprocess.check_output(f'docker exec {cid} python3 -m pip freeze | grep -v "@"', shell=True)
+        docker_deps = {
+            dsplit[0]: dsplit[1] for dsplit in (dep.split("==") for dep in docker_freeze.decode("utf-8").splitlines())
+        }
+
+        # Validate against pyproject.toml
+        self._validate_pyproject_toml(docker_deps)
+        # Validate against poetry.lock
+        self._validate_poetry_lock(docker_deps)
+
+        self.line(
+            f"Validation success!  Docker image {cid} has consistent versions with dependencies specified "
+            f"in this project"
+        )
+
+        return 0
```

### Comparing `poeblix-0.8.1/src/poeblix/validatewheel.py` & `poeblix-0.9/src/poeblix/validatewheel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,188 +1,190 @@
-import re
-from pathlib import Path
-from typing import List, Dict
-from zipfile import ZipFile
-
-import pkginfo
-from cleo.helpers import argument, option
-from cleo.io.inputs.option import Option
-from cleo.io.outputs.output import Verbosity
-
-# For fixing https://github.com/python-poetry/poetry/issues/5216
-from packaging.tags import sys_tags  # noqa
-from poetry.console.commands.env_command import EnvCommand
-from poetry.core.semver.helpers import parse_constraint
-
-# e.g. "nemoize (>=0.1.0,<0.2.0)"
-from tomlkit.exceptions import NonExistentKey
-
-from poeblix.util import util
-
-package_regex = r"(.*) \((.*)\)"
-
-
-class ValidateWheelPlugin(EnvCommand):
-    """
-    Validates a wheel file contains Requires Dist as specified in pyproject.toml and poetry.lock files in the project
-    this command is run.
-    """
-
-    name = "blixvalidatewheel"
-    description = (
-        "Validates a wheel file contains Requires Dist that satisfies constraints in pyproject.toml and poetry.lock "
-        "files in the project this command is ran.  This by default validates in both directions, as in "
-        "it validates the wheel file's Requires Dist is specified in the project and vice versa."
-    )
-
-    arguments = [argument("wheelPath", "Wheel file path")]
-
-    # TODO: Add groups to options
-    options: List[Option] = [
-        option(
-            "no-lock",
-            None,
-            "Disables validating lock file dependencies.",
-        ),
-        option(
-            "with-groups",
-            None,
-            "Specify which dependency groups to use to validate the wheel file, on top of required groups from "
-            "pyproject.toml.  Can be specified multiple times or as a comma delimited list.",
-            flag=False,
-            multiple=True,
-        ),
-    ]
-
-    loggers = ["poetry.core.masonry.builders.wheel"]
-
-    def _validate_data_files(self, path):
-        """
-        Validates wheel archive contains data_files as specified in pyproject.toml, if exists.
-        """
-        self.line("Validating data_files in wheel file contain those specified in pyproject.toml")
-        # Get files in wheel
-        wheel = pkginfo.Wheel(path)
-        wheel_files = ZipFile(path).namelist()
-        self.line(f"Wheel files: {wheel_files}", verbosity=Verbosity.DEBUG)
-        data_file_prefix = f"{wheel.name}-{wheel.version}.data/data/"
-
-        wheel_data_files = [fname for fname in wheel_files if data_file_prefix in fname]
-        self.line(f"Wheel data files: {wheel_data_files}", verbosity=Verbosity.DEBUG)
-
-        try:
-            data_files_config = self.poetry.pyproject.data["tool"]["blix"]["data"]
-            if "data_files" in data_files_config:
-                data_files = data_files_config["data_files"]
-
-                for data_file in list(data_files):
-                    destination = data_file["destination"]
-                    sources = data_file["from"]
-
-                    # TODO: Use OS specific separator
-                    if destination[-1] != "/":
-                        destination += "/"
-
-                    for src in sources:
-                        filename = src.rsplit("/", 1)[1]
-                        data_file_path = data_file_prefix + destination + filename
-
-                        if data_file_path not in wheel_data_files:
-                            raise RuntimeError(
-                                f"Wheel at [{path}] does not contain expected data_file [{data_file_path}]"
-                            )
-                        else:
-                            wheel_data_files.remove(data_file_path)
-        except NonExistentKey:
-            self.line(f"[tool.blix.data] section not found in {self.poetry.file}")
-        # If any wheel data files leftover, raise error
-        if wheel_data_files:
-            raise RuntimeError(
-                f"Wheel at [{path}] contains extraneous data_files not specified in pyproject.toml: {wheel_data_files}"
-            )
-
-    def _validate_pyproject_toml(self, requires_dist: Dict[str, str], leftover_wheel_packages: set):
-        """Validates that dependencies in pyproject.toml are exactly reflected in the wheel file's requires_dist"""
-        # TODO: Only checks main group
-        self.line("Validating against pyproject.toml...")
-        required_packages = self.poetry.package.requires
-        leftover_pyproject_packages = set([p.pretty_name for p in required_packages])
-        for package in required_packages:
-            name = package.pretty_name
-            # Defer to poetry.lock validation if dpeendency is a direct origin source such as git, local path, etc.
-            if not package.is_direct_origin() and name in requires_dist:
-                leftover_pyproject_packages.remove(name)
-                leftover_wheel_packages.discard(name)
-                # Parse constraint into an object using poetry's helper
-                wheel_version = parse_constraint(requires_dist[name])
-                if package.constraint.difference(wheel_version).is_any():
-                    raise RuntimeError(
-                        f"Wheel file has different version constraints for Package(name={name}, "
-                        f"version={wheel_version}) compared to pyproject.toml Package(name={name}, "
-                        f"version={package.constraint})"
-                    )
-        if leftover_pyproject_packages:
-            raise RuntimeError(
-                f"Packages in pyproject.toml are not present in the Wheel file: {list(leftover_pyproject_packages)}"
-            )
-
-    def _validate_poetry_lock(self, requires_dist: Dict[str, str], leftover_wheel_packages: set):
-        """Validates that dependencies in poetry.lock are exactly reflected in the wheel file's requires_dist"""
-        if self.option("no-lock"):
-            self.line("Skipping poetry.lock validation as --no-lock was specified")
-            return
-
-        with_groups = []
-        for group in self.option("with-groups"):
-            with_groups.extend(group.split(","))
-
-        self.line("Validating against poetry.lock...")
-        locked_repo = self.poetry.locker.locked_repository()
-        ops = util.resolve_dependencies(self.poetry, self.env, locked_repo, with_groups)
-        leftover_lock_packages = set([p.package.pretty_name for p in ops])
-        for op in ops:
-            dependency_package = op.package
-            name = dependency_package.pretty_name
-            if name in requires_dist:
-                leftover_lock_packages.remove(name)
-                leftover_wheel_packages.discard(name)
-                # Parse constraint into an object using poetry's helper
-                wheel_version = parse_constraint(requires_dist[name])
-                if dependency_package.version.difference(wheel_version).is_any():
-                    raise RuntimeError(
-                        f"Wheel file has different version constraints for Package(name={name}, "
-                        f"version={wheel_version}) compared to poetry.lock Package(name={name}, "
-                        f"version={dependency_package.version})"
-                    )
-        if leftover_lock_packages:
-            raise RuntimeError(
-                f"Packages in poetry.lock are not present in the Wheel file: {sorted(list(leftover_lock_packages))}"
-            )
-
-    def handle(self) -> int:
-        path = self.argument("wheelPath")
-        if not Path(path).is_file():
-            raise ValueError(f"Path [{path}] does not point to a valid file")
-        self.line(f"Validating Requires Dist for wheel [{path}] against pyproject.toml/poetry.lock")
-        metadata = pkginfo.get_metadata(path)
-        assert metadata is not None, f"Could not get metadata at path [{path}]"
-        self.line(f"Wheel Requires Dist: {metadata.requires_dist}", verbosity=Verbosity.DEBUG)
-        packages = {}
-        for package in metadata.requires_dist:
-            parsed = re.search(package_regex, package)
-            if not parsed:
-                raise ValueError(f"Could not parse Requires Dist package [{package}].  Please submit an Issue!")
-            packages[parsed.group(1)] = parsed.group(2)
-        self.line(f"Parsed Requires Dist: {packages}", verbosity=Verbosity.DEBUG)
-        # Keep track of wheel files we've scanned over to validate wheel does not contain extra dependencies not
-        # specified in the project
-        leftover_wheel_packages = set(packages.keys())
-        self._validate_pyproject_toml(packages, leftover_wheel_packages)
-        self._validate_poetry_lock(packages, leftover_wheel_packages)
-        if leftover_wheel_packages:
-            raise RuntimeError(
-                f"Packages in Wheel file are not present in pyproject.toml/poetry.lock: {list(leftover_wheel_packages)}"
-            )
-        self._validate_data_files(path)
-        self.line("Validation succeeded!")
-
-        return 0
+import re
+from pathlib import Path
+from typing import List, Dict
+from zipfile import ZipFile
+
+import pkginfo
+from cleo.helpers import argument, option
+from cleo.io.inputs.option import Option
+from cleo.io.outputs.output import Verbosity
+
+# For fixing https://github.com/python-poetry/poetry/issues/5216
+from packaging.tags import sys_tags  # noqa
+from poetry.console.commands.env_command import EnvCommand
+from poetry.core.semver.helpers import parse_constraint
+
+# e.g. "nemoize (>=0.1.0,<0.2.0)"
+from tomlkit.exceptions import NonExistentKey
+
+from poeblix.util import util
+
+package_regex = r"(.*) \((.*)\)"
+
+
+class ValidateWheelPlugin(EnvCommand):
+    """
+    Validates a wheel file contains Requires Dist as specified in pyproject.toml and poetry.lock files in the project
+    this command is run.
+    """
+
+    name = "blixvalidatewheel"
+    description = (
+        "Validates a wheel file contains Requires Dist that satisfies constraints in pyproject.toml and poetry.lock "
+        "files in the project this command is ran.  This by default validates in both directions, as in "
+        "it validates the wheel file's Requires Dist is specified in the project and vice versa."
+    )
+
+    arguments = [argument("wheelPath", "Wheel file path")]
+
+    # TODO: Add groups to options
+    options: List[Option] = [
+        option(
+            "no-lock",
+            None,
+            "Disables validating lock file dependencies.",
+        ),
+        option(
+            "with-groups",
+            None,
+            "Specify which dependency groups to use to validate the wheel file, on top of required groups from "
+            "pyproject.toml.  Can be specified multiple times or as a comma delimited list.",
+            flag=False,
+            multiple=True,
+        ),
+    ]
+
+    loggers = ["poetry.core.masonry.builders.wheel"]
+
+    def _validate_data_files(self, path):
+        """
+        Validates wheel archive contains data_files as specified in pyproject.toml, if exists.
+        """
+        self.line("Validating data_files in wheel file contain those specified in pyproject.toml")
+        # Get files in wheel
+        wheel = pkginfo.Wheel(path)
+        wheel_files = ZipFile(path).namelist()
+        self.line(f"Wheel files: {wheel_files}", verbosity=Verbosity.DEBUG)
+        data_file_prefix = f"{wheel.name}-{wheel.version}.data/data/"
+
+        wheel_data_files = [fname for fname in wheel_files if data_file_prefix in fname]
+        self.line(f"Wheel data files: {wheel_data_files}", verbosity=Verbosity.DEBUG)
+
+        try:
+            data_files_config = self.poetry.pyproject.data["tool"]["blix"]["data"]
+            if "data_files" in data_files_config:
+                data_files = data_files_config["data_files"]
+
+                for data_file in list(data_files):
+                    destination = data_file["destination"]
+                    sources = data_file["from"]
+
+                    # TODO: Use OS specific separator
+                    if destination[-1] != "/":
+                        destination += "/"
+
+                    for src in sources:
+                        filename = src.rsplit("/", 1)[1]
+                        data_file_path = data_file_prefix + destination + filename
+
+                        if data_file_path not in wheel_data_files:
+                            raise RuntimeError(
+                                f"Wheel at [{path}] does not contain expected data_file [{data_file_path}]"
+                            )
+                        else:
+                            wheel_data_files.remove(data_file_path)
+        except NonExistentKey:
+            self.line(f"[tool.blix.data] section not found in {self.poetry.file}")
+        # If any wheel data files leftover, raise error
+        if wheel_data_files:
+            raise RuntimeError(
+                f"Wheel at [{path}] contains extraneous data_files not specified in pyproject.toml: {wheel_data_files}"
+            )
+
+    def _validate_pyproject_toml(self, requires_dist: Dict[str, str], leftover_wheel_packages: set):
+        """Validates that dependencies in pyproject.toml are exactly reflected in the wheel file's requires_dist"""
+        # TODO: Only checks main group
+        self.line("Validating against pyproject.toml...")
+        required_packages = self.poetry.package.requires
+        leftover_pyproject_packages = set([p.pretty_name.lower() for p in required_packages])
+        for package in required_packages:
+            name = package.pretty_name.lower()
+            # Defer to poetry.lock validation if dependency is a direct origin source such as git, local path, etc.
+            if not package.is_direct_origin() and name in requires_dist:
+                leftover_pyproject_packages.remove(name)
+                leftover_wheel_packages.discard(name)
+                # Parse constraint into an object using poetry's helper
+                wheel_version = parse_constraint(requires_dist[name])
+                if package.constraint.difference(wheel_version).is_any():
+                    raise RuntimeError(
+                        f"Wheel file has different version constraints for Package(name={name}, "
+                        f"version={wheel_version}) compared to pyproject.toml Package(name={name}, "
+                        f"version={package.constraint})"
+                    )
+        if leftover_pyproject_packages:
+            raise RuntimeError(
+                f"Packages in pyproject.toml are not present in the Wheel file: {list(leftover_pyproject_packages)}"
+            )
+
+    def _validate_poetry_lock(self, requires_dist: Dict[str, str], leftover_wheel_packages: set):
+        """Validates that dependencies in poetry.lock are exactly reflected in the wheel file's requires_dist"""
+        if self.option("no-lock"):
+            self.line("Skipping poetry.lock validation as --no-lock was specified")
+            return
+
+        with_groups = []
+        for group in self.option("with-groups"):
+            with_groups.extend(group.split(","))
+
+        self.line("Validating against poetry.lock...")
+        locked_repo = self.poetry.locker.locked_repository()
+        ops = util.resolve_dependencies(self.poetry, self.env, locked_repo, with_groups)
+        leftover_lock_packages = set([p.package.pretty_name for p in ops])
+        for op in ops:
+            dependency_package = op.package
+            name = dependency_package.pretty_name.lower()
+            if name in requires_dist:
+                leftover_lock_packages.remove(name)
+                leftover_wheel_packages.discard(name)
+                # Parse constraint into an object using poetry's helper
+                wheel_version = parse_constraint(requires_dist[name])
+                if dependency_package.version.difference(wheel_version).is_any():
+                    raise RuntimeError(
+                        f"Wheel file has different version constraints for Package(name={name}, "
+                        f"version={wheel_version}) compared to poetry.lock Package(name={name}, "
+                        f"version={dependency_package.version})"
+                    )
+        if leftover_lock_packages:
+            raise RuntimeError(
+                f"Packages in poetry.lock are not present in the Wheel file: {sorted(list(leftover_lock_packages))}"
+            )
+
+    def handle(self) -> int:
+        path = self.argument("wheelPath")
+        if not Path(path).is_file():
+            raise ValueError(f"Path [{path}] does not point to a valid file")
+        self.line(f"Validating Requires Dist for wheel [{path}] against pyproject.toml/poetry.lock")
+        metadata = pkginfo.get_metadata(path)
+        assert metadata is not None, f"Could not get metadata at path [{path}]"
+        self.line(f"Wheel Requires Dist: {metadata.requires_dist}", verbosity=Verbosity.DEBUG)
+        packages = {}
+        for package in metadata.requires_dist:
+            parsed = re.search(package_regex, package)
+            if not parsed:
+                raise ValueError(f"Could not parse Requires Dist package [{package}].  Please submit an Issue!")
+            packages[parsed.group(1)] = parsed.group(2)
+        self.line(f"Parsed Requires Dist: {packages}", verbosity=Verbosity.DEBUG)
+        # Case insensitive checking: https://github.com/spoorn/poeblix/issues/11
+        packages_lower = {key.lower(): val for key, val in packages.items()}
+        # Keep track of wheel files we've scanned over to validate wheel does not contain extra dependencies not
+        # specified in the project
+        leftover_wheel_packages = set(packages_lower.keys())
+        self._validate_pyproject_toml(packages_lower, leftover_wheel_packages)
+        self._validate_poetry_lock(packages_lower, leftover_wheel_packages)
+        if leftover_wheel_packages:
+            raise RuntimeError(
+                f"Packages in Wheel file are not present in pyproject.toml/poetry.lock: {list(leftover_wheel_packages)}"
+            )
+        self._validate_data_files(path)
+        self.line("Validation succeeded!")
+
+        return 0
```

### Comparing `poeblix-0.8.1/PKG-INFO` & `poeblix-0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,7 @@
-Metadata-Version: 2.1
-Name: poeblix
-Version: 0.8.1
-Summary: Poetry plugin that adds support for building wheel files using the poetry.lock file, and data_files just like in setup.py
-Home-page: https://github.com/spoorn/poeblix
-Keywords: poeblix,utility,poetry,plugin,poetry-plugin,wheel,distribution,data_files
-Author: spoorn
-Author-email: spookump@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: poetry (>=1.2.0rc1,<2.0)
-Project-URL: Repository, https://github.com/spoorn/poeblix
-Description-Content-Type: text/markdown
-
 # poeblix
 Poetry Plugin that adds various features that extend the `poetry` command such as building wheel files with locked dependencies, and validations of wheel/docker containers.
 
 Supports poetry versions `1.2+`
 
 # Overview
 These contain custom poetry plugins that enable functionality not available in the official distribution of poetry.  These include:
@@ -213,8 +189,7 @@
 ```
 
 **plugins.py** : contains our plugin that adds the `poetry blixbuild` command for building our wheel file
 
 **validatewheel.py**: adds a `poetry blixvalidatewheel` command that validates a wheel file contains the Required Dist as specified in pyproject.toml/poetry.lock
 
 **validatedocker.py** : adds a command that validates a docker file contains dependencies as specified in pyproject.toml and poetry.lock.  This does *NOT* validate that they are exactly matching, but rather that all dependencies in pyproject.toml/poetry.lock exist in the docker container on the correct versions.  The docker image may contain more extra dependencies
-
```

