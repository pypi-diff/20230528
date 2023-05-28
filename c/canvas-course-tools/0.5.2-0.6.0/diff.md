# Comparing `tmp/canvas_course_tools-0.5.2.tar.gz` & `tmp/canvas_course_tools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvas_course_tools-0.5.2.tar", max compression
+gzip compressed data, was "canvas_course_tools-0.6.0.tar", max compression
```

## Comparing `canvas_course_tools-0.5.2.tar` & `canvas_course_tools-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,24 @@
--rw-r--r--   0        0        0    35129 2021-04-16 18:11:54.000000 canvas_course_tools-0.5.2/LICENSE
--rw-r--r--   0        0        0     1149 2023-02-21 16:38:48.000000 canvas_course_tools-0.5.2/README.md
--rw-r--r--   0        0        0     1157 2023-03-09 20:27:13.868177 canvas_course_tools-0.5.2/pyproject.toml
--rw-r--r--   0        0        0       22 2023-03-09 20:27:13.868198 canvas_course_tools-0.5.2/src/canvas_course_tools/__init__.py
--rw-r--r--   0        0        0     4821 2023-02-21 16:33:25.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/canvas_tasks.py
--rw-r--r--   0        0        0      897 2023-03-06 12:00:58.666232 canvas_course_tools-0.5.2/src/canvas_course_tools/cli.py
--rw-r--r--   0        0        0     1407 2023-02-20 18:42:01.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/configfile.py
--rw-r--r--   0        0        0     4274 2023-03-06 12:04:39.547276 canvas_course_tools-0.5.2/src/canvas_course_tools/courses.py
--rw-r--r--   0        0        0     1148 2023-03-06 20:48:46.763376 canvas_course_tools-0.5.2/src/canvas_course_tools/datatypes.py
--rw-r--r--   0        0        0     2405 2023-03-06 20:34:05.114028 canvas_course_tools-0.5.2/src/canvas_course_tools/group_lists.py
--rw-r--r--   0        0        0     3711 2023-03-09 20:17:06.113306 canvas_course_tools-0.5.2/src/canvas_course_tools/groups.py
--rw-r--r--   0        0        0     1824 2023-03-06 12:04:47.022815 canvas_course_tools-0.5.2/src/canvas_course_tools/servers.py
--rw-r--r--   0        0        0     1390 2023-03-06 12:04:50.029295 canvas_course_tools-0.5.2/src/canvas_course_tools/students.py
--rwxr-xr-x   0        0        0     1291 2023-02-21 10:44:27.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/exam.tex
--rwxr-xr-x   0        0        0      945 2023-02-21 10:44:19.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/peer-feedback.tex
--rwxr-xr-x   0        0        0     1380 2023-03-07 09:40:42.488273 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/photos.tex
--rwxr-xr-x   0        0        0     1024 2023-02-21 10:48:56.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/signatures.tex
--rwxr-xr-x   0        0        0      630 2023-02-21 14:27:49.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/student-list-pairs.tex
--rwxr-xr-x   0        0        0      546 2023-02-21 14:27:59.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/student-list.tex
--rw-r--r--   0        0        0      245 2023-03-06 20:40:35.976728 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/student-list.txt
--rw-r--r--   0        0        0      379 2023-03-06 15:35:56.420385 canvas_course_tools-0.5.2/src/canvas_course_tools/templates/template-info.toml
--rw-r--r--   0        0        0     7075 2023-03-09 20:27:15.442395 canvas_course_tools-0.5.2/src/canvas_course_tools/templates.py
--rw-r--r--   0        0        0      400 2023-02-21 16:47:46.000000 canvas_course_tools-0.5.2/src/canvas_course_tools/utils.py
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 canvas_course_tools-0.5.2/setup.py
--rw-r--r--   0        0        0     2456 1970-01-01 00:00:00.000000 canvas_course_tools-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0    35129 2021-04-16 18:11:54.000000 canvas_course_tools-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1149 2023-02-21 16:38:48.000000 canvas_course_tools-0.6.0/README.md
+-rw-r--r--   0        0        0     1181 2023-05-26 18:46:18.162541 canvas_course_tools-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      171 2023-05-28 14:30:27.596828 canvas_course_tools-0.6.0/src/canvas_course_tools/__init__.py
+-rw-r--r--   0        0        0     6014 2023-05-26 16:34:41.489772 canvas_course_tools-0.6.0/src/canvas_course_tools/canvas_tasks.py
+-rw-r--r--   0        0        0      925 2023-05-24 12:22:29.497305 canvas_course_tools-0.6.0/src/canvas_course_tools/cli.py
+-rw-r--r--   0        0        0     1407 2023-02-20 18:42:01.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/configfile.py
+-rw-r--r--   0        0        0     4274 2023-05-24 12:28:18.600764 canvas_course_tools-0.6.0/src/canvas_course_tools/courses.py
+-rw-r--r--   0        0        0     1366 2023-05-26 10:35:52.897835 canvas_course_tools-0.6.0/src/canvas_course_tools/datatypes.py
+-rw-r--r--   0        0        0     2405 2023-03-06 20:34:05.114028 canvas_course_tools-0.6.0/src/canvas_course_tools/group_lists.py
+-rw-r--r--   0        0        0     4066 2023-05-26 16:30:06.266271 canvas_course_tools-0.6.0/src/canvas_course_tools/groups.py
+-rw-r--r--   0        0        0     1824 2023-03-06 12:04:47.022815 canvas_course_tools-0.6.0/src/canvas_course_tools/servers.py
+-rw-r--r--   0        0        0     2102 2023-05-26 18:35:54.857315 canvas_course_tools-0.6.0/src/canvas_course_tools/students.py
+-rwxr-xr-x   0        0        0     1171 2023-05-24 09:46:37.435270 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/exam.tex
+-rwxr-xr-x   0        0        0      945 2023-02-21 10:44:19.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/peer-feedback.tex
+-rwxr-xr-x   0        0        0     1391 2023-05-26 18:44:58.002544 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/photos.tex
+-rwxr-xr-x   0        0        0     1024 2023-02-21 10:48:56.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/signatures.tex
+-rwxr-xr-x   0        0        0      630 2023-02-21 14:27:49.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list-pairs.tex
+-rwxr-xr-x   0        0        0      546 2023-02-21 14:27:59.000000 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list.tex
+-rw-r--r--   0        0        0      245 2023-03-06 20:40:35.976728 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list.txt
+-rw-r--r--   0        0        0      379 2023-03-06 15:35:56.420385 canvas_course_tools-0.6.0/src/canvas_course_tools/templates/template-info.toml
+-rw-r--r--   0        0        0     7076 2023-05-24 12:40:34.346462 canvas_course_tools-0.6.0/src/canvas_course_tools/templates.py
+-rw-r--r--   0        0        0      836 2023-05-26 16:21:14.865830 canvas_course_tools-0.6.0/src/canvas_course_tools/utils.py
+-rw-r--r--   0        0        0     2495 1970-01-01 00:00:00.000000 canvas_course_tools-0.6.0/PKG-INFO
```

### Comparing `canvas_course_tools-0.5.2/LICENSE` & `canvas_course_tools-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/README.md` & `canvas_course_tools-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/pyproject.toml` & `canvas_course_tools-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canvas-course-tools"
-version = "0.5.2"
+version = "0.6.0"
 homepage = "https://github.com/davidfokkema/canvas-course-tools"
 description = "Canvas course tools"
 authors = ["David Fokkema <d.b.r.a.fokkema@vu.nl>"]
 readme = "README.md"
 packages = [{include = "canvas_course_tools", from = "src"}]
 license = "GPL-3.0-or-later"
 classifiers = [
@@ -23,21 +23,22 @@
 [tool.poetry.scripts]
 canvas = "canvas_course_tools.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 appdirs = "^1.4.4"
-rich = "^12.5.1"
-canvasapi = "^2.2.0"
+rich = "^13.3.5"
+canvasapi = "^3.1.0"
 python-dateutil = "^2.8.1"
 rich-click = "^1.5.2"
 jinja2 = "^3.1.2"
 tomli-w = "^1.0.0"
 tomli = "^2.0.1"
+trogon = "^0.4.0"
 
-[tool.poetry.dev-dependencies]
-ipython = "^7.22.0"
+[tool.poetry.group.dev.dependencies]
+ipython = "^8.13.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/cli.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,25 @@
 This command-line application enables you to quickly perform a variety of tasks
 that would otherwise require you to log in to a Canvas site. Since using this
 tool requires no mouse-clicks at all, these tasks are performed much quicker and
 easier than through the web interface.
 """
 
 import rich_click as click
+import trogon
 
 from canvas_course_tools import __version__
 from canvas_course_tools.courses import courses
 from canvas_course_tools.groups import groups
 from canvas_course_tools.servers import servers
 from canvas_course_tools.students import students
 from canvas_course_tools.templates import templates
 
 
+@trogon.tui()
 @click.group()
 @click.version_option(version=__version__)
 def cli():
     pass
 
 
 cli.add_command(servers)
```

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/configfile.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/configfile.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/courses.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/courses.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/group_lists.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/group_lists.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/groups.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import pathlib
 
 import rich_click as click
 from rich import print
 from rich.progress import Progress
 
-from canvas_course_tools import configfile
 from canvas_course_tools.canvas_tasks import (
     CanvasObjectExistsError,
     Forbidden,
     ResourceDoesNotExist,
 )
 from canvas_course_tools.group_lists import parse_group_list
-from canvas_course_tools.utils import get_canvas
+from canvas_course_tools.utils import find_course
 
 
 @click.group()
 def groups():
     """Create Canvas groups based on group lists."""
     pass
 
@@ -39,39 +38,33 @@
     starts with a #-character, the rest of the line is interpreted as a title.
     If it starts with ##, the rest of the line is interpreted as a group name.
     There can be multiple groups defined in one file. All other non-empty lines
     are interpreted as a student name with optional student id and notes field.
     It must be of the form "student name (id) [notes]". For example, the
     following is a valid group list file:
 
-        \b
+
+
+    \b
         # Physics 101
         ## Group A
         Drew Ferrell (800057) [second year]
         Amanda James (379044)
         Antonio Morris (804407) [skips thursdays]
 
-        \b
+    \b
         ## Group B
         Elizabeth Allison (312702)
         James Morales (379332)
 
     \f
     Ignore the \b and \f characters in this docstring. They are to tell click to
     not wrap paragraphs (\b) and not display this note (\f).
     """
-    config = configfile.read_config()
-    try:
-        server, course_id = (
-            config["courses"][course_alias][k] for k in ("server", "course_id")
-        )
-    except KeyError:
-        raise click.BadArgumentUsage(f"Unknown course {course_alias}.")
-    canvas = get_canvas(server)
-    course = canvas.get_course(course_id)
+    canvas, course = find_course(course_alias)
 
     file_contents = pathlib.Path(group_list).read_text(encoding="utf-8")
     group_list = parse_group_list(file_contents)
 
     print(f"Creating GroupSet {group_list.name}...")
     try:
         groupset = canvas.create_groupset(group_list.name, course, overwrite)
@@ -99,7 +92,25 @@
                         f"[red]WARNING: you do not have authorization to add student {student.name}."
                     )
                 progress.advance(task_students)
             progress.advance(task_groups)
             print(f"Created {group.name}.")
 
     print("Done")
+
+
+@groups.command("list")
+@click.argument("course_alias")
+def list_groups(course_alias: str) -> None:
+    """List all groups and groupsets in a course.
+
+    List all groups in course COURSE_ALIAS, for all group sets (a.k.a. group
+    categories). Each group set also lists the group set ID in brackets. This
+    can be useful if you want to list all students in a group set. See also the
+    `canvas students` command group.
+    """
+    canvas, course = find_course(course_alias)
+    for group_set in canvas.list_groupsets(course):
+        print(f"{group_set.name} ({group_set.id}):")
+        for group in canvas.list_groups(group_set):
+            print(f"\t{group.name}")
+        print()
```

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/servers.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/servers.py`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates/exam.tex` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/exam.tex`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-{% set start_times = ["9:00", "9:35", "10:10", "10:45", "11:20", "11:55", "13:00", "13:35", "14:10", "14:45"] %}
-{% set end_times = ["9:20", "9:55", "10:30", "11:05", "11:40", "12:15", "13:20", "13:55", "14:30", "15:05"] %}
+{% set start_times = ["9:00", "9:35", "10:10", "10:45", "11:20", "11:55", "13:00", "13:35", "14:10", "14:45", "15:20", "15:55"] %}
+{% set end_times = ["9:20", "9:55", "10:30", "11:05", "11:40", "12:15", "13:20", "13:55", "14:30", "15:05", "15:40", "16:15"] %}
 \documentclass[a4paper,11pt]{article}
 
 \usepackage[scale=.8]{geometry}
 \usepackage{fouriernc}
 \usepackage[utf8]{inputenc}
 \usepackage[T1]{fontenc}
 
@@ -14,30 +14,27 @@
 
 \renewcommand{\arraystretch}{1.5}
 
 \begin{document}
 
 {% for examinator in groups %}
 
-{\centering\LARGE\textbf{Indeling {{ title -}} }}
+{\centering\LARGE\textbf{ {{ title -}} }}
 
 \vspace{1em}
 
 \section*{ {{ examinator.name }} }
 
 \noindent
 \begin{tabular}{r@{ -- }rll}
     \toprule
     \multicolumn{2}{l}{\textbf{Tijd}} & \textbf{Student} &                          \\
     \midrule
     {% for start, end, student in zip(start_times, end_times, examinator.students) -%}
     {{ start }} & {{ end }} & {{ student.name }} & {% if student.notes %}\textsc{[{{ student.notes }}]}{% endif %}
     {%- if loop.index is divisibleby(3) %} \\[5pt] {% else %} \\ {% endif %}
-    {%- if loop.index == 6 %}
-    12:15                             & 13:00            & \hrulefill \quad pauze \quad \hrulefill \\
-    {%- endif %}
     {% endfor %}
     \bottomrule
 \end{tabular}
 \newpage
 {% endfor %}
-\end{document}
+\end{document}
```

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates/peer-feedback.tex` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/peer-feedback.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates/photos.tex` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/photos.tex`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 \noindent
 \begin{tabularx}{\linewidth}{@{}XXXX@{}}
     {% for rows in page|batch(4) %}
     {% for student in rows %}
     \makecell{
         \makecell[t]{
             {%- if student.photo %}
-            \includegraphics[width=3.5cm]{ {{- student.photo -}} }
+            \includegraphics[width=3.5cm]{ {{- student.photo.as_posix() -}} }
             {%- else %}
             \begin{tikzpicture}
                 \clip (-1.75cm, 0) rectangle +(3.5cm, 4.7cm);
                 \fill[black!10!white] (0, 0) ellipse (1.75cm and 1.25cm);
                 \fill[black!10!white] (0, 2.25cm) circle (1cm);
             \end{tikzpicture}
             {%- endif %} \\
```

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates/signatures.tex` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/signatures.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates/student-list-pairs.tex` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list-pairs.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates/student-list.tex` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates/student-list.tex`

 * *Files identical despite different names*

### Comparing `canvas_course_tools-0.5.2/src/canvas_course_tools/templates.py` & `canvas_course_tools-0.6.0/src/canvas_course_tools/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import importlib.resources
 import pathlib
 
-import rich_click as click
 import jinja2
+import rich_click as click
 import tomli
 from rich import box
 from rich.console import Console
 from rich.syntax import Syntax
 from rich.table import Table
 
 from canvas_course_tools.datatypes import GroupList
 from canvas_course_tools.group_lists import parse_group_list
 
-
 TEMPLATE_INFO_FILE = "template-info.toml"
 
 
 @click.group()
 def templates():
     """Generate files based on templates and group lists."""
     pass
@@ -103,14 +102,16 @@
     line starts with a #-character, the rest of the line is interpreted as a
     title. If it starts with ##, the rest of the line is interpreted as a group
     name. There can be multiple groups defined in one file. All other non-empty
     lines are interpreted as a student name with optional student id and notes
     field. It must be of the form "student name (id) [notes]". For example, the
     following is a valid group list file:
 
+
+
     \b
         # Physics 101
         ## Group A
         Drew Ferrell (800057) [second year]
         Amanda James (379044)
         Antonio Morris (804407) [skips thursdays]
```

### Comparing `canvas_course_tools-0.5.2/PKG-INFO` & `canvas_course_tools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvas-course-tools
-Version: 0.5.2
+Version: 0.6.0
 Summary: Canvas course tools
 Home-page: https://github.com/davidfokkema/canvas-course-tools
 License: GPL-3.0-or-later
 Author: David Fokkema
 Author-email: d.b.r.a.fokkema@vu.nl
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -17,22 +17,23 @@
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
-Requires-Dist: canvasapi (>=2.2.0,<3.0.0)
+Requires-Dist: canvasapi (>=3.1.0,<4.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: python-dateutil (>=2.8.1,<3.0.0)
-Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Requires-Dist: rich-click (>=1.5.2,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: trogon (>=0.4.0,<0.5.0)
 Description-Content-Type: text/markdown
 
 # canvas-course-tools
 
 Canvas course tools was created at the physics practicals at the Vrije
 Universiteit Amsterdam to greatly reduce the time needed to create class lists
 (with photos!) for staff and teaching assistants. Class lists are also created
```

