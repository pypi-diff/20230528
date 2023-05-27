# Comparing `tmp/fabricius-0.1.0.tar.gz` & `tmp/fabricius-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabricius-0.1.0.tar", max compression
+gzip compressed data, was "fabricius-0.2.0.tar", max compression
```

## Comparing `fabricius-0.1.0.tar` & `fabricius-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,29 @@
--rw-r--r--   0        0        0      153 2022-09-10 15:34:05.338263 fabricius-0.1.0/fabricius/__init__.py
--rw-r--r--   0        0        0    14327 2023-02-17 18:46:29.570262 fabricius-0.1.0/fabricius/_typing.py
--rw-r--r--   0        0        0     1172 2023-02-17 18:33:39.407500 fabricius-0.1.0/fabricius/const.py
--rw-r--r--   0        0        0      628 2023-02-17 18:33:39.408547 fabricius-0.1.0/fabricius/errors.py
--rw-r--r--   0        0        0     9461 2023-02-17 18:33:39.409074 fabricius-0.1.0/fabricius/file.py
--rw-r--r--   0        0        0     4827 2023-02-17 18:33:39.409600 fabricius-0.1.0/fabricius/generator.py
--rw-r--r--   0        0        0      346 2023-02-17 18:33:39.410124 fabricius-0.1.0/fabricius/interfaces.py
--rw-r--r--   0        0        0     8930 2023-02-17 18:33:39.410650 fabricius-0.1.0/fabricius/plugin.py
--rw-r--r--   0        0        0        0 2022-08-28 21:26:11.341048 fabricius-0.1.0/fabricius/plugins/__init__.py
--rw-r--r--   0        0        0       59 2023-02-17 18:33:39.411173 fabricius-0.1.0/fabricius/plugins/define/__init__.py
--rw-r--r--   0        0        0     2767 2023-02-17 18:33:39.412223 fabricius-0.1.0/fabricius/plugins/define/generator.py
--rw-r--r--   0        0        0     3095 2023-02-17 18:33:39.412749 fabricius-0.1.0/fabricius/plugins/generator_rich.py
--rw-r--r--   0        0        0        0 2022-08-28 21:19:29.832177 fabricius-0.1.0/fabricius/py.typed
--rw-r--r--   0        0        0     2460 2023-02-17 18:33:39.413792 fabricius-0.1.0/fabricius/renderer.py
--rw-r--r--   0        0        0     4537 2023-02-17 18:33:39.414320 fabricius-0.1.0/fabricius/terminal.py
--rw-r--r--   0        0        0     4160 2023-02-17 18:33:39.415373 fabricius-0.1.0/fabricius/utils.py
--rw-r--r--   0        0        0     1068 2022-08-28 21:19:29.825340 fabricius-0.1.0/LICENSE
--rw-r--r--   0        0        0     1957 2023-02-17 19:10:29.305221 fabricius-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2337 2023-02-17 18:33:39.400675 fabricius-0.1.0/README.md
--rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 fabricius-0.1.0/setup.py
--rw-r--r--   0        0        0     3929 1970-01-01 00:00:00.000000 fabricius-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      153 2023-03-16 17:40:31.347873 fabricius-0.2.0/fabricius/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-14 21:20:54.257563 fabricius-0.2.0/fabricius/app/main.py
+-rw-r--r--   0        0        0     1750 2023-05-27 15:01:48.807987 fabricius-0.2.0/fabricius/app/signals.py
+-rw-r--r--   0        0        0     1741 2023-05-27 14:50:38.892052 fabricius-0.2.0/fabricius/app/ui.py
+-rw-r--r--   0        0        0     2475 2023-05-15 14:08:38.208520 fabricius-0.2.0/fabricius/exceptions.py
+-rw-r--r--   0        0        0      364 2023-05-14 21:20:54.259581 fabricius-0.2.0/fabricius/globals.py
+-rw-r--r--   0        0        0    10161 2023-05-27 17:35:37.833592 fabricius-0.2.0/fabricius/models/file.py
+-rw-r--r--   0        0        0     1127 2023-05-14 21:20:54.260595 fabricius-0.2.0/fabricius/models/renderer.py
+-rw-r--r--   0        0        0     1348 2023-05-20 22:54:09.227749 fabricius-0.2.0/fabricius/models/signal.py
+-rw-r--r--   0        0        0     4113 2023-05-26 11:44:22.089496 fabricius-0.2.0/fabricius/models/template.py
+-rw-r--r--   0        0        0        0 2023-03-16 17:40:40.836866 fabricius-0.2.0/fabricius/py.typed
+-rw-r--r--   0        0        0     1029 2023-05-27 15:01:12.261102 fabricius-0.2.0/fabricius/readers/cookiecutter/config.py
+-rw-r--r--   0        0        0      518 2023-05-14 21:20:54.262638 fabricius-0.2.0/fabricius/readers/cookiecutter/exceptions.py
+-rw-r--r--   0        0        0     2319 2023-05-14 21:20:54.263659 fabricius-0.2.0/fabricius/readers/cookiecutter/extensions.py
+-rw-r--r--   0        0        0     3121 2023-05-14 21:20:54.263659 fabricius-0.2.0/fabricius/readers/cookiecutter/hooks.py
+-rw-r--r--   0        0        0     9174 2023-05-26 08:19:55.822842 fabricius-0.2.0/fabricius/readers/cookiecutter/setup.py
+-rw-r--r--   0        0        0      313 2023-05-14 21:20:54.261623 fabricius-0.2.0/fabricius/readers/README.md
+-rw-r--r--   0        0        0      277 2023-05-14 21:20:54.265687 fabricius-0.2.0/fabricius/renderers/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-14 21:20:54.265687 fabricius-0.2.0/fabricius/renderers/jinja_renderer.py
+-rw-r--r--   0        0        0      235 2023-05-14 21:20:54.265687 fabricius-0.2.0/fabricius/renderers/mustache.py
+-rw-r--r--   0        0        0      266 2023-05-14 21:20:54.266700 fabricius-0.2.0/fabricius/renderers/python_format.py
+-rw-r--r--   0        0        0      753 2023-05-14 21:20:54.266700 fabricius-0.2.0/fabricius/renderers/python_string_template.py
+-rw-r--r--   0        0        0      338 2023-05-14 21:20:54.267714 fabricius-0.2.0/fabricius/renderers/utils.py
+-rw-r--r--   0        0        0     1377 2023-05-20 11:29:45.291185 fabricius-0.2.0/fabricius/types.py
+-rw-r--r--   0        0        0     4490 2023-05-24 05:16:46.083201 fabricius-0.2.0/fabricius/utils.py
+-rw-r--r--   0        0        0     1068 2022-08-28 21:19:29.825340 fabricius-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2458 2023-05-27 23:11:42.501865 fabricius-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2337 2023-05-27 16:58:35.756473 fabricius-0.2.0/README.md
+-rw-r--r--   0        0        0     4129 1970-01-01 00:00:00.000000 fabricius-0.2.0/PKG-INFO
```

### Comparing `fabricius-0.1.0/fabricius/file.py` & `fabricius-0.2.0/fabricius/models/file.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,157 +1,129 @@
 import contextlib
 import pathlib
 import typing
 
 from typing_extensions import Self
 
-from fabricius.const import FILE_STATE, Data, PathStrOrPath
-from fabricius.errors import FabriciusError
-from fabricius.renderer import (
+from fabricius.app.signals import (
+    after_file_commit,
+    before_file_commit,
+    on_file_commit_fail,
+)
+from fabricius.exceptions import AlreadyCommittedError, MissingRequiredValueError
+from fabricius.models.renderer import Renderer
+from fabricius.renderers import (
     ChevronRenderer,
+    JinjaRenderer,
     PythonFormatRenderer,
-    Renderer,
     StringTemplateRenderer,
 )
+from fabricius.types import FILE_STATE, Data, FileCommitResult, PathStrOrPath
 
 
-class NoContentError(FabriciusError):
-    """
-    The file does not have any content.
-    """
-
-    def __init__(self, file_name: str) -> None:
-        """
-        The file does not have any content.
-        """
-        super().__init__(f"File '{file_name}' was not set with a content/template.")
-
-
-class NoDestinationError(FabriciusError):
-    """
-    The file does not know where to go.
-    """
-
-    def __init__(self, file_name: str) -> None:
-        """
-        The file does not know where to go.
-        """
-        super().__init__(f"File '{file_name}' does not have a destination set.")
-
-
-class AlreadyCommittedError(FabriciusError):
-    """
-    The file has already been committed/persisted.
-    """
-
-    def __init__(self, file_name: str) -> None:
-        """
-        The file has already been committed/persisted.
-        """
-        super().__init__(f"File '{file_name}' has already been committed.")
-
-
-class FileCommitResult(typing.TypedDict):
-    """
-    A FileCommitResult is returned when a file was successfully saved.
-    It returns its information after its creation.
-    """
-
-    name: str
-    """
-    The name of the file.
-    """
-
-    state: FILE_STATE
-    """
-    The state of the file. Should always be "persisted".
-    """
-
-    destination: pathlib.Path
-    """
-    Where the file is located/has been saved.
-    """
-
-    data: Data
-    """
-    The data that has been passed during rendering.
-    """
-
-    template_content: str
-    """
-    The original content of the template.
-    """
-
-    content: str
+class File:
     """
-    The resulting content of the saved file.
+    The builder class to initialize a file template.
+    The result (Through the :py:meth:`.generate` method) is the render of the file's content.
+    You can "commit" the file to the disk to persist the file's content.
     """
 
-
-class File:
     name: str
     """
     The name of the file that will be generated.
     """
 
     state: FILE_STATE
     """
     The state of the file.
     """
 
-    content: typing.Optional[str]
+    content: str | None
     """
     The template's content.
     """
 
-    template_content: typing.Optional[str]
+    template_content: str | None
     """
     The content of the base template, if set.
     """
 
-    destination: typing.Optional[pathlib.Path]
+    destination: pathlib.Path | None
     """
     The destination of the file, if set.
     """
 
-    renderer: typing.Type[Renderer]
+    renderer: type[Renderer]
     """
     The renderer to use to generate the file.
     """
 
     data: Data
     """
     The data that will be passed to the renderer.
     """
 
-    will_fake: bool
+    _will_fake: bool
     """
     If the file should fake its creation upon commit.
     """
 
     def __init__(self, name: str, extension: typing.Optional[str] = None) -> None:
         """
-        Create a file's generator.
-
         Parameters
         ----------
         name : :py:class:`str`
             The name of the file.
         extension : :py:class:`str`
-            The extension of the file, without dot, same as ``name="<name>.<extension>"``
+            The extension of the file, without dot, same as ``name="<name>.<extension>"`` (Where
+            ``<name>`` and ``<extensions>`` are the arguments given to the class).
         """
         self.name = f"{name}.{extension}" if extension else name
         self.state = "pending"
         self.content = None
         self.destination = None
-        self.will_fake = False
+        self._will_fake = False
 
         self.renderer = PythonFormatRenderer
         self.data = {}
 
+    def compute_destination(self) -> pathlib.Path:
+        """
+        Compute the destination of the file.
+
+        Raises
+        ------
+        :py:exc:`fabricius.exceptions.MissingRequiredValueError` :
+            If the object does not have the property "destination" set.
+            (Use :py:meth:`.to_directory`)
+
+        Returns
+        -------
+        pathlib.Path :
+            The final path.
+        """
+        if not self.destination:
+            raise MissingRequiredValueError(self, "destination")
+
+        if not self.destination.exists() and (not self._will_fake):
+            self.destination.mkdir(parents=True)
+        return self.destination.joinpath(self.name)
+
+    @property
+    def can_commit(self) -> typing.Literal["destination", "content", "state", True]:
+        # sourcery skip: reintroduce-else
+        if not self.destination:
+            return "destination"
+        if not self.content:
+            return "content"
+        if self.state == "persisted":
+            return "state"
+
+        return True
+
     def from_file(self, path: str | pathlib.Path) -> Self:
         """
         Read the content from a file template.
 
         Raises
         ------
         :py:exc:`FileNotFoundError` :
@@ -208,68 +180,86 @@
     def use_string_template(self) -> Self:
         """
         Use string.Template to render the template.
         """
         self.renderer = StringTemplateRenderer
         return self
 
+    def use_jinja(self) -> Self:
+        """
+        Use Jinja2 to render the template.
+        """
+        self.renderer = JinjaRenderer
+        return self
+
     def with_renderer(self, renderer: typing.Type[Renderer]) -> Self:
         """
         Use a custom renderer to render the template.
 
         Parameters
         ----------
-        renderer : Type of :py:class:`fabricius.generator.renderer.Renderer`
+        renderer : Type of :py:class:`fabricius.models.renderer.Renderer`
             The renderer to use to format the file.
             It must be not initialized.
         """
         self.renderer = renderer
         return self
 
     def with_data(self, data: Data, *, overwrite: bool = True) -> Self:
         """
         Add data to pass to the template.
 
         Parameters
         ----------
-        data : :py:data:`fabricius.const.Data`
+        data : :py:const:`fabricius.types.Data`
             The data you want to pass to the template.
         overwrite : :py:class:`bool`
             If the data that already exists should be deleted. If False, the new data will be
             added on top of the already existing data. Default to ``True``.
         """
         if overwrite:
             self.data = {}
         self.data.update(data)
         return self
 
     def fake(self) -> Self:
-        self.will_fake = True
+        """
+        Set the file to fake the commit.
+        This will ensure that the file does not get stored on the machine upon commit.
+        """
+        self._will_fake = True
         return self
 
     def restore(self) -> Self:
-        self.will_fake = False
+        """
+        Set the file to not fake the commit.
+        This will ensure that the file gets stored on the machine upon commit.
+
+        .. hint ::
+           This is the default behavior. It's only useful to use this method if you have used :py:meth:`.fake`.
+        """
+        self._will_fake = False
         return self
 
     def generate(self) -> str:
         """
         Generate the file's content.
 
         Raises
         ------
-        :py:exc:`fabricius.generator.errors.NoContentError` :
+        :py:exc:`fabricius.exceptions.MissingRequiredValue` :
             If no content to the file were added.
 
         Returns
         -------
         :py:class:`str` :
             The final content of the file.
         """
         if not self.content:
-            raise NoContentError(self.name)
+            raise MissingRequiredValueError(self, "content")
 
         return self.renderer(self.data).render(self.content)
 
     def commit(self, *, overwrite: bool = False) -> FileCommitResult:
         """
         Save the file to the disk.
 
@@ -277,59 +267,66 @@
         ----------
         overwrite : :py:class:`bool`
             If a file exist at the given path, shall the overwrite parameter say if the file
             should be overwritten or not. Default to ``False``.
 
         Raises
         ------
-        :py:exc:`fabricius.generator.errors.NoContentError` :
-            If no content to the file were added.
-        :py:exc:`fabricius.generator.errors.NoDestinationError` :
-            If no destination/path were designated.
-        :py:exc:`fabricius.generator.errors.AlreadyCommittedError` :
+        :py:exc:`MissingRequiredValueError <fabricius.exceptions.MissingRequiredValueError>` :
+            If a required value was not set. (Content or destination)
+        :py:exc:`fabricius.exceptions.AlreadyCommittedError` :
             If the file has already been saved to the disk.
         :py:exc:`FileExistsError` :
             If the file already exists on the disk and ``overwrite`` is set to ``False``.
 
             This is different from
-            :py:exc:`AlreadyCommittedError <fabricius.generator.errors.AlreadyCommittedError>`
+            :py:exc:`AlreadyCommittedError <fabricius.exceptions.AlreadyCommittedError>`
             because this indicates that the content of the file this generator was never actually
             saved.
         :py:exc:`OSError` :
             The file's name is not valid for the OS.
 
         Returns
         -------
-        :py:class:`fabricius.file.FileCommitResult` :
+        :py:class:`fabricius.types.FileCommitResult` :
             A typed dict with information about the created file.
         """
         if not self.destination:
-            raise NoDestinationError(self.name)
+            raise MissingRequiredValueError(self, "destination")
         if not self.content:
-            raise NoContentError(self.name)
+            raise MissingRequiredValueError(self, "content")
         if self.state == "persisted":
             raise AlreadyCommittedError(self.name)
 
         final_content = self.generate()
 
-        if not self.destination.exists() and (not self.will_fake):
-            self.destination.mkdir(parents=True)
-        destination = self.destination.joinpath(self.name)
+        destination = self.compute_destination()
 
         if destination.exists() and not overwrite:
-            raise FileExistsError(f"File '{self.name}' already exists.")
+            exception = FileExistsError(f"File '{self.name}' already exists.")
+            exception.filename = self.name
+            raise exception
 
-        if self.will_fake:
-            self.state = "persisted"
-        else:
-            with contextlib.suppress(NotADirectoryError):
-                destination.write_text(final_content)
+        before_file_commit.send(self)
+
+        try:
+            if self._will_fake:
                 self.state = "persisted"
+            else:
+                with contextlib.suppress(NotADirectoryError):
+                    destination.write_text(final_content)
+                    self.state = "persisted"
+        except Exception as exception:
+            on_file_commit_fail.send(self)
 
-        return FileCommitResult(
+        commit = FileCommitResult(
             name=self.name,
             state=self.state,
             data=self.data,
             template_content=self.content,
             content=final_content,
             destination=self.destination.joinpath(self.name),
+            fake=self._will_fake,
         )
+
+        after_file_commit.send(self, commit)
+        return commit
```

### Comparing `fabricius-0.1.0/fabricius/renderer.py` & `fabricius-0.2.0/fabricius/models/template.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,137 @@
-import abc
-import string
+import pathlib
 import typing
-from collections import UserDict
 
-import chevron
+from typing_extensions import Self
 
-from .const import Data
+from fabricius.app.signals import after_template_commit, before_template_commit
+from fabricius.exceptions import (
+    AlreadyCommittedError,
+    ConflictError,
+    MissingRequiredValueError,
+)
+from fabricius.models.file import File, FileCommitResult
+from fabricius.models.renderer import Renderer
+from fabricius.types import Data, PathStrOrPath
 
+STATE = typing.Literal["pending", "failed", "persisted"]
+RendererType = typing.TypeVar("RendererType", bound=type[Renderer])
 
-class DictAllowMiss(UserDict[str, typing.Any]):
-    """
-    A subclass of Dict to return an empty string in case of missing key, instead of raising an
-    error, so that it can play nice with renderer.
 
-    :meta private:
+class Template(typing.Generic[RendererType]):
     """
+    The :py:class:`Template` class represent "a collection of files that, in its whole, represents
+    a project"
+
+    The difference between the :py:class:`.Template` class and a collection of :py:class:`.File`
+    is that a template assumes all of your files have the same properties. (Requires the same
+    renderer, the same data, etc.)
 
-    def __missing__(self, _: str) -> typing.Literal[""]:
-        return ""
+    Typically, a template only use one renderer, and shares the same data across the whole project
+    template.
 
+    The :py:class:`.Template` will assist creating a project, while providing a similar interface
+    of the :py:class:`.File` model.
+    """
 
-class Renderer(abc.ABC):
+    state: STATE
+    """
+    The state of the template
     """
-    The Renderer is what translate and generates the output of templates. Core of the work.
 
-    You must subclass this class and override the :py:meth:`render` method, if possible, also add
-    a name.
+    base_folder: pathlib.Path
+    """
+    The folder where the template will be generated.
     """
 
-    name: typing.Optional[str]
+    files: list[File]
     """
-    The name of the renderer, not necessary, but suggested to add.
+    The list of files that will be rendered when committing.
     """
 
     data: Data
     """
-    A dictionary that contains data passed by the users to pass inside the template.
+    The data to pass to the files.
     """
 
-    def __init__(self, data: Data) -> None:
-        self.data = data
+    renderer: RendererType
+    """
+    The renderer that will be used to generate the files.
+    """
 
-    @abc.abstractmethod
-    def render(self, content: str) -> str:
-        """
-        This method will process a given string, the template input and return the processed
-        template as a string too.
+    _will_fake: bool
 
+    def __init__(
+        self,
+        base_folder: PathStrOrPath,
+        renderer: RendererType,
+    ) -> None:
+        """
         Parameters
         ----------
-        content : :py:class:`str`
-            The template
-
-        Returns
-        -------
-        :py:class:`str` :
-            The result of the processed template.
+        base_folder : :py:const:`fabricius.types.PathStrOrPath`
+            Indication of where the template should be generated.
+        renderer : Type of :py:class:`fabricius.models.renderer.Renderer`
+            The renderer to use with the template.
         """
-        raise NotImplementedError()
+        self.base_folder = pathlib.Path(base_folder)
+        self.state = "pending"
+        self.files = []
+        self.data = {}
+        self.renderer = renderer
+        self._will_fake = False
+
+    @property
+    def __files_destinations(self) -> list[pathlib.Path | None]:
+        return [file.destination for file in self.files]
+
+    def add_file(self, file: File) -> Self:
+        if not file.can_commit:
+            reason = file.can_commit
+            if reason == "state":
+                raise AlreadyCommittedError(file.name)
+            raise MissingRequiredValueError(self, reason)
+
+        if file.destination and file.compute_destination() in self.__files_destinations:
+            raise ConflictError(
+                file,
+                f"File {file.name} has a destination that already is present in Template's destinations.",
+            )
+
+        self.files.append(file)
+        return self
+
+    def add_files(self, files: typing.Iterable[File]) -> Self:
+        for file in files:
+            self.add_file(file)
+        return self
 
+    def push_data(self, data: Data) -> Self:
+        self.data = data
+        return self
 
-class PythonFormatRenderer(Renderer):
-    name = "Python str.format"
-
-    def render(self, content: str) -> str:
-        return content.format_map(DictAllowMiss(self.data))
-
-
-class ChevronRenderer(Renderer):
-    name = "Chevron (Moustache)"
-
-    def render(self, content: str) -> str:
-        return chevron.render(content, self.data)
-
-
-class StringTemplateRenderer(Renderer):
-    name = "Python string.Template"
-
-    safe: bool
-    """
-    Indicate if the renderer should use
-    :py:meth:`string.Template.safe_substitute` or
-    :py:meth:`string.Template.substitute`
-    """
+    def fake(self) -> Self:
+        self._will_fake = True
+        return self
+
+    def restore(self) -> Self:
+        self._will_fake = False
+        return self
+
+    def commit(self, *, overwrite: bool = False) -> list[FileCommitResult]:
+        results: list[FileCommitResult] = []
+
+        before_template_commit.send(self)
+
+        for file in self.files:
+            file.with_data(self.data, overwrite=False)
+            if self._will_fake:
+                file.fake()
+            else:
+                # Just in case they've been set to fake...
+                file.restore()
+            result = file.commit(overwrite=overwrite)
+            results.append(result)
 
-    def __init__(self, data: Data, *, safe: bool = True) -> None:
-        self.safe = safe
-        super().__init__(data)
+        after_template_commit.send(self, results)
 
-    def render(self, content: str) -> str:
-        if self.safe:
-            return string.Template(content).safe_substitute(DictAllowMiss(self.data))
-        else:
-            return string.Template(content).substitute(self.data)
+        return results
```

### Comparing `fabricius-0.1.0/fabricius/utils.py` & `fabricius-0.2.0/fabricius/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,24 @@
+import random
 import typing
 
 import inflection
 from rich.color import Color
 
+FABRICIUS_IS_AWESOME = [
+    "Generating your project, hang tight!",
+    "Bing, bonk, bang! Scaffolding your next idea...",
+    "Helping you on your next idea!",
+    "Serious work in progress... Give it a second or two!",
+]
+
+
+def fetch_me_a_beer() -> str:
+    return random.choice(FABRICIUS_IS_AWESOME)
+
 
 def calculate_text_color(
     color: str | Color, *, threshold: int = 150
 ) -> typing.Literal["black", "bright_white"]:
     """
     Calculate if the text should be in black or white depending on a color.
     It uses the following formula: (r * 0.299 + g * 0.587 + b * 0.114) > threshold
```

### Comparing `fabricius-0.1.0/LICENSE` & `fabricius-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabricius-0.1.0/pyproject.toml` & `fabricius-0.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "Fabricius"
-version = "0.1.0"
+version = "0.2.0"
 description = "Fabricius: The supportive templating engine for Python!"
 license = "MIT"
 authors = ["Predeactor <pro.julien.mauroy@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Predeactor/Fabricius"
 documentation = "https://fabricius.readthedocs.org"
 keywords = ["cookiecutter", "template", "project", "scaffold", "pyscaffold"]
 classifiers = [
-    "Development Status :: 1 - Planning",
+    "Development Status :: 2 - Pre-Alpha",
 
     "Intended Audience :: Developers",
     "Intended Audience :: End Users/Desktop",
 
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
 
@@ -36,40 +36,66 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 chevron = "^0.14.0"
 rich = "^12.4.4"
 typing-extensions = "^4.2.0"
 inflection = "^0.5.1"
+click = "^8.1.3"
+jinja2 = "^3.1.2"
+jinja2-time = "^0.2.0"
+slugify = "^0.0.1"
+pyyaml = "^6.0"
 
 # Extra: Docs
 Sphinx = { version = "^5.0.2", optional = true }
 furo = { version = "^2022.6.21", optional = true }
 sphinx-autobuild = { version = "^2021.3.14", optional = true }
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
-black = "^22.3.0"
-isort = "^5.10.1"
+black = "^23.3.0"
+isort = "^5.12.0"
 pre-commit = "^2.19.0"
 mypy = "^1.0.0"
 tox = "^4.4.5"
 types-chevron = "^0.14.2.2"
+esbonio = "^0.16.1"
+ipykernel = "^6.22.0"
+pytest = "^7.3.1"
+poethepoet = "^0.20.0"
 
 [tool.poetry.group.actions]
 optional = true
 
 [tool.poetry.group.actions.dependencies]
 tox-gh-actions = "^3.0.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-autobuild", "furo"]
 
+[tool.poe]
+poetry_command = ""
+
+[tool.poe.tasks]
+_format_black = "black ."
+_format_isort = "isort ."
+format = ["_format_black", "_format_isort"]
+test = "pytest . -v"
+
+[tool.poe.tasks.docs]
+cmd = "make livehtml"
+cwd = "./docs"
+
+[tool.poe.tasks.docscov]
+cmd = "make html -b coverage"
+cwd = "./docs"
+
 [tool.black]
 line-length = 99
 
 [tool.isort]
 profile = "black"
 
 [build-system]
```

### Comparing `fabricius-0.1.0/README.md` & `fabricius-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `fabricius-0.1.0/PKG-INFO` & `fabricius-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fabricius
-Version: 0.1.0
+Version: 0.2.0
 Summary: Fabricius: The supportive templating engine for Python!
 Home-page: https://github.com/Predeactor/Fabricius
 License: MIT
 Keywords: cookiecutter,template,project,scaffold,pyscaffold
 Author: Predeactor
 Author-email: pro.julien.mauroy@gmail.com
 Requires-Python: >=3.10,<4.0
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -20,20 +20,25 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: docs
-Requires-Dist: Sphinx (>=5.0.2,<6.0.0); extra == "docs"
+Requires-Dist: Sphinx (>=5.0.2,<6.0.0) ; extra == "docs"
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
-Requires-Dist: furo (>=2022.6.21,<2023.0.0); extra == "docs"
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: furo (>=2022.6.21,<2023.0.0) ; extra == "docs"
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
+Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
+Requires-Dist: jinja2-time (>=0.2.0,<0.3.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=12.4.4,<13.0.0)
-Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0); extra == "docs"
+Requires-Dist: slugify (>=0.0.1,<0.0.2)
+Requires-Dist: sphinx-autobuild (>=2021.3.14,<2022.0.0) ; extra == "docs"
 Requires-Dist: typing-extensions (>=4.2.0,<5.0.0)
 Project-URL: Documentation, https://fabricius.readthedocs.org
 Project-URL: Repository, https://github.com/Predeactor/Fabricius
 Description-Content-Type: text/markdown
 
 # Fabricius
```

