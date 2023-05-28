# Comparing `tmp/maturin-1.0.0b9.tar.gz` & `tmp/maturin-1.0.1.tar.gz`

## Comparing `maturin-1.0.0b9.tar` & `maturin-1.0.1.tar`

### file list

```diff
@@ -1,69 +1,64 @@
--rw-r--r--   0        0        0     4522 1970-01-01 00:00:00.000000 maturin-1.0.0b9/Cargo.toml
--rw-r--r--   0     1001      123     1692 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.cirrus.yml
--rw-r--r--   0     1001      123       94 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.codespellrc
--rw-r--r--   0     1001      123      252 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.config/nextest.toml
--rw-r--r--   0     1001      123      180 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.dockerignore
--rw-r--r--   0     1001      123      184 2023-05-06 13:28:59.000000 maturin-1.0.0b9/.gitignore
--rw-r--r--   0     1001      123    65671 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Cargo.lock
--rw-r--r--   0     1001      123    55621 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Changelog.md
--rw-r--r--   0     1001      123     3228 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Code-of-Conduct.md
--rw-r--r--   0     1001      123     2386 2023-05-06 13:28:59.000000 maturin-1.0.0b9/Dockerfile
--rw-r--r--   0     1001      123      245 2023-05-06 13:28:59.000000 maturin-1.0.0b9/MANIFEST.in
--rw-r--r--   0     1001      123    16573 2023-05-06 13:28:59.000000 maturin-1.0.0b9/README.md
--rw-r--r--   0     1001      123       16 2023-05-06 13:28:59.000000 maturin-1.0.0b9/clippy.toml
--rw-r--r--   0     1001      123     9664 2023-05-06 13:28:59.000000 maturin-1.0.0b9/deny.toml
--rw-r--r--   0     1001      123    10847 2023-05-06 13:28:59.000000 maturin-1.0.0b9/license-apache
--rw-r--r--   0     1001      123     1051 2023-05-06 13:28:59.000000 maturin-1.0.0b9/license-mit
--rw-r--r--   0     1001      123     6236 2023-05-06 13:28:59.000000 maturin-1.0.0b9/maturin/__init__.py
--rw-r--r--   0     1001      123      956 2023-05-06 13:28:59.000000 maturin-1.0.0b9/maturin/__main__.py
--rw-r--r--   0     1001      123     5162 2023-05-06 13:28:59.000000 maturin-1.0.0b9/maturin/import_hook.py
--rw-r--r--   0     1001      123      200 2023-05-06 13:28:59.000000 maturin-1.0.0b9/netlify.toml
--rw-r--r--   0     1001      123     2170 2023-05-06 13:28:59.000000 maturin-1.0.0b9/noxfile.py
--rw-r--r--   0     1001      123     1290 2023-05-06 13:28:59.000000 maturin-1.0.0b9/pyproject.toml
--rw-r--r--   0     1001      123     2868 2023-05-06 13:28:59.000000 maturin-1.0.0b9/setup.py
--rw-r--r--   0     1001      123    19534 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/audit.rs
--rw-r--r--   0     1001      123    53261 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/manylinux-policy.json
--rw-r--r--   0     1001      123      242 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/mod.rs
--rw-r--r--   0     1001      123     1862 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/musllinux-policy.json
--rw-r--r--   0     1001      123     1389 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/musllinux.rs
--rw-r--r--   0     1001      123     3777 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/patchelf.rs
--rw-r--r--   0     1001      123     4602 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/platform_tag.rs
--rw-r--r--   0     1001      123     5393 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/policy.rs
--rw-r--r--   0     1001      123     1169 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/auditwheel/repair.rs
--rw-r--r--   0     1001      123    47514 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/build_context.rs
--rw-r--r--   0     1001      123    57281 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/build_options.rs
--rw-r--r--   0     1001      123     5407 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/cargo_toml.rs
--rw-r--r--   0     1001      123    33723 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/ci.rs
--rw-r--r--   0     1001      123    24202 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/compile.rs
--rw-r--r--   0     1001      123     8342 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/cross_compile.rs
--rw-r--r--   0     1001      123     6119 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/develop.rs
--rw-r--r--   0     1001      123     2233 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/lib.rs
--rw-r--r--   0     1001      123    17816 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/main.rs
--rw-r--r--   0     1001      123    32462 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/metadata.rs
--rw-r--r--   0     1001      123    44938 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/module_writer.rs
--rw-r--r--   0     1001      123     8203 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/new_project.rs
--rw-r--r--   0     1001      123    16142 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/project_layout.rs
--rw-r--r--   0     1001      123    17317 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/pyproject_toml.rs
--rw-r--r--   0     1001      123    11820 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/config.rs
--rw-r--r--   0     1001      123     1595 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/get_interpreter_metadata.py
--rw-r--r--   0     1001      123    34577 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/mod.rs
--rw-r--r--   0     1001      123      443 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-emscripten.json
--rw-r--r--   0     1001      123     3861 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-freebsd.json
--rw-r--r--   0     1001      123    14124 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-linux.json
--rw-r--r--   0     1001      123     3812 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-macos.json
--rw-r--r--   0     1001      123      738 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-netbsd.json
--rw-r--r--   0     1001      123     2353 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-openbsd.json
--rw-r--r--   0     1001      123     3341 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/python_interpreter/sysconfig-windows.json
--rw-r--r--   0     1001      123    34671 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/source_distribution.rs
--rw-r--r--   0     1001      123    18478 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/target.rs
--rw-r--r--   0     1001      123      686 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/.gitignore.j2
--rw-r--r--   0     1001      123      518 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/Cargo.toml.j2
--rw-r--r--   0     1001      123      149 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/__init__.py.j2
--rw-r--r--   0     1001      123      123 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/build.rs.j2
--rw-r--r--   0     1001      123       47 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/example.udl.j2
--rw-r--r--   0     1001      123      722 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/lib.rs.j2
--rw-r--r--   0     1001      123       45 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/main.rs.j2
--rw-r--r--   0     1001      123      859 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/templates/pyproject.toml.j2
--rw-r--r--   0     1001      123    22846 2023-05-06 13:28:59.000000 maturin-1.0.0b9/src/upload.rs
--rwxr-xr-x   0     1001      123      974 2023-05-06 13:28:59.000000 maturin-1.0.0b9/test-dockerfile.sh
--rw-r--r--   0        0        0    17754 1970-01-01 00:00:00.000000 maturin-1.0.0b9/PKG-INFO
+-rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 maturin-1.0.1/Cargo.toml
+-rw-r--r--   0     1001      123     1681 2023-05-28 02:31:17.000000 maturin-1.0.1/.cirrus.yml
+-rw-r--r--   0     1001      123       94 2023-05-28 02:31:17.000000 maturin-1.0.1/.codespellrc
+-rw-r--r--   0     1001      123      252 2023-05-28 02:31:17.000000 maturin-1.0.1/.config/nextest.toml
+-rw-r--r--   0     1001      123      488 2023-05-28 02:31:17.000000 maturin-1.0.1/.devcontainer/devcontainer.json
+-rwxr-xr-x   0     1001      123      351 2023-05-28 02:31:17.000000 maturin-1.0.1/.devcontainer/post_create.sh
+-rw-r--r--   0     1001      123      180 2023-05-28 02:31:17.000000 maturin-1.0.1/.dockerignore
+-rw-r--r--   0     1001      123      184 2023-05-28 02:31:17.000000 maturin-1.0.1/.gitignore
+-rw-r--r--   0     1001      123    69147 2023-05-28 02:31:17.000000 maturin-1.0.1/Cargo.lock
+-rw-r--r--   0     1001      123    57326 2023-05-28 02:31:17.000000 maturin-1.0.1/Changelog.md
+-rw-r--r--   0     1001      123     3228 2023-05-28 02:31:17.000000 maturin-1.0.1/Code-of-Conduct.md
+-rw-r--r--   0     1001      123     2386 2023-05-28 02:31:17.000000 maturin-1.0.1/Dockerfile
+-rw-r--r--   0     1001      123      245 2023-05-28 02:31:17.000000 maturin-1.0.1/MANIFEST.in
+-rw-r--r--   0     1001      123    16809 2023-05-28 02:31:17.000000 maturin-1.0.1/README.md
+-rw-r--r--   0     1001      123       16 2023-05-28 02:31:17.000000 maturin-1.0.1/clippy.toml
+-rw-r--r--   0     1001      123     9936 2023-05-28 02:31:17.000000 maturin-1.0.1/deny.toml
+-rw-r--r--   0     1001      123    10847 2023-05-28 02:31:17.000000 maturin-1.0.1/license-apache
+-rw-r--r--   0     1001      123     1051 2023-05-28 02:31:17.000000 maturin-1.0.1/license-mit
+-rw-r--r--   0     1001      123     6739 2023-05-28 02:31:17.000000 maturin-1.0.1/maturin/__init__.py
+-rw-r--r--   0     1001      123      956 2023-05-28 02:31:17.000000 maturin-1.0.1/maturin/__main__.py
+-rw-r--r--   0     1001      123     5162 2023-05-28 02:31:17.000000 maturin-1.0.1/maturin/import_hook.py
+-rw-r--r--   0     1001      123      200 2023-05-28 02:31:17.000000 maturin-1.0.1/netlify.toml
+-rw-r--r--   0     1001      123     2170 2023-05-28 02:31:17.000000 maturin-1.0.1/noxfile.py
+-rw-r--r--   0     1001      123     1290 2023-05-28 02:31:17.000000 maturin-1.0.1/pyproject.toml
+-rw-r--r--   0     1001      123     2890 2023-05-28 02:31:17.000000 maturin-1.0.1/setup.py
+-rw-r--r--   0     1001      123    19534 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/audit.rs
+-rw-r--r--   0     1001      123    53261 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/manylinux-policy.json
+-rw-r--r--   0     1001      123      242 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/mod.rs
+-rw-r--r--   0     1001      123     1862 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/musllinux-policy.json
+-rw-r--r--   0     1001      123     1389 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/musllinux.rs
+-rw-r--r--   0     1001      123     3777 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/patchelf.rs
+-rw-r--r--   0     1001      123     4602 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/platform_tag.rs
+-rw-r--r--   0     1001      123     5393 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/policy.rs
+-rw-r--r--   0     1001      123     1169 2023-05-28 02:31:17.000000 maturin-1.0.1/src/auditwheel/repair.rs
+-rw-r--r--   0     1001      123    47638 2023-05-28 02:31:17.000000 maturin-1.0.1/src/build_context.rs
+-rw-r--r--   0     1001      123    57614 2023-05-28 02:31:17.000000 maturin-1.0.1/src/build_options.rs
+-rw-r--r--   0     1001      123     5407 2023-05-28 02:31:17.000000 maturin-1.0.1/src/cargo_toml.rs
+-rw-r--r--   0     1001      123    33723 2023-05-28 02:31:17.000000 maturin-1.0.1/src/ci.rs
+-rw-r--r--   0     1001      123    24173 2023-05-28 02:31:17.000000 maturin-1.0.1/src/compile.rs
+-rw-r--r--   0     1001      123     8342 2023-05-28 02:31:17.000000 maturin-1.0.1/src/cross_compile.rs
+-rw-r--r--   0     1001      123     6092 2023-05-28 02:31:17.000000 maturin-1.0.1/src/develop.rs
+-rw-r--r--   0     1001      123     2233 2023-05-28 02:31:17.000000 maturin-1.0.1/src/lib.rs
+-rw-r--r--   0     1001      123    17816 2023-05-28 02:31:17.000000 maturin-1.0.1/src/main.rs
+-rw-r--r--   0     1001      123    32462 2023-05-28 02:31:17.000000 maturin-1.0.1/src/metadata.rs
+-rw-r--r--   0     1001      123    45608 2023-05-28 02:31:17.000000 maturin-1.0.1/src/module_writer.rs
+-rw-r--r--   0     1001      123     8203 2023-05-28 02:31:17.000000 maturin-1.0.1/src/new_project.rs
+-rw-r--r--   0     1001      123    16869 2023-05-28 02:31:17.000000 maturin-1.0.1/src/project_layout.rs
+-rw-r--r--   0     1001      123    18607 2023-05-28 02:31:17.000000 maturin-1.0.1/src/pyproject_toml.rs
+-rw-r--r--   0     1001      123    28354 2023-05-28 02:31:17.000000 maturin-1.0.1/src/python_interpreter/config.rs
+-rw-r--r--   0     1001      123     1595 2023-05-28 02:31:17.000000 maturin-1.0.1/src/python_interpreter/get_interpreter_metadata.py
+-rw-r--r--   0     1001      123    35318 2023-05-28 02:31:17.000000 maturin-1.0.1/src/python_interpreter/mod.rs
+-rw-r--r--   0     1001      123    35086 2023-05-28 02:31:17.000000 maturin-1.0.1/src/source_distribution.rs
+-rw-r--r--   0     1001      123    18602 2023-05-28 02:31:17.000000 maturin-1.0.1/src/target.rs
+-rw-r--r--   0     1001      123      686 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/.gitignore.j2
+-rw-r--r--   0     1001      123      518 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/Cargo.toml.j2
+-rw-r--r--   0     1001      123      149 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/__init__.py.j2
+-rw-r--r--   0     1001      123      123 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/build.rs.j2
+-rw-r--r--   0     1001      123       47 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/example.udl.j2
+-rw-r--r--   0     1001      123      722 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/lib.rs.j2
+-rw-r--r--   0     1001      123       45 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/main.rs.j2
+-rw-r--r--   0     1001      123      859 2023-05-28 02:31:17.000000 maturin-1.0.1/src/templates/pyproject.toml.j2
+-rw-r--r--   0     1001      123    22914 2023-05-28 02:31:17.000000 maturin-1.0.1/src/upload.rs
+-rwxr-xr-x   0     1001      123      974 2023-05-28 02:31:17.000000 maturin-1.0.1/test-dockerfile.sh
+-rw-r--r--   0        0        0    17988 1970-01-01 00:00:00.000000 maturin-1.0.1/PKG-INFO
```

### Comparing `maturin-1.0.0b9/Cargo.toml` & `maturin-1.0.1/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [package]
 authors = ["konstin <konstin@mailbox.org>", "messense <messense@icloud.com>"]
 name = "maturin"
-version = "1.0.0-beta.9"
+version = "1.0.1"
 description = "Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as python packages"
 exclude = ["test-crates/**/*", "sysconfig/*", "test-data/*", "ci/*", "tests/*", "guide/*", ".github/*"]
 homepage = "https://github.com/pyo3/maturin"
 readme = "README.md"
 repository = "https://github.com/pyo3/maturin"
 license = "MIT OR Apache-2.0"
 keywords = ["python", "cffi", "packaging", "pypi", "pyo3"]
@@ -17,34 +17,33 @@
 name = "maturin"
 
 [lib]
 name = "maturin"
 
 [dependencies]
 anyhow = "1.0.63"
-base64 = "0.13.0"
+base64 = "0.21.0"
 glob = "0.3.0"
 cargo-config2 = "0.1.4"
 cargo_metadata = "0.15.3"
 cargo-options = "0.6.0"
 cbindgen = { version = "0.24.2", default-features = false }
 flate2 = "1.0.18"
 goblin = "0.6.1"
-platform-info = "1.0.0"
+platform-info = "2.0.1"
 regex = "1.7.0"
 serde = { version = "1.0.141", features = ["derive"] }
 serde_json = "1.0.80"
 sha2 = "0.10.3"
 tar = "0.4.38"
 tempfile = "3.2.0"
 toml = "0.7.0"
 toml_edit = "0.19.1"
 zip = { version = "0.6.1", default-features = false, features = ["bzip2", "deflate", "time"] }
 thiserror = "1.0.37"
-dirs = "4.0.0"
 fs-err = "2.5.0"
 fat-macho = { version = "0.4.6", default-features = false }
 once_cell = "1.7.2"
 rustc_version = "0.4.0"
 semver = "1.0.13"
 target-lexicon = "0.12.0"
 indexmap = "1.9.3"
@@ -63,29 +62,30 @@
 time = "0.3.17"
 
 # cli
 clap = { version = "4.0.0", features = ["derive", "env", "wrap_help"] }
 clap_complete_command = { version = "0.5.1", optional = true }
 
 # cross compile
-cargo-zigbuild = { version = "0.16.7", default-features = false, optional = true }
-cargo-xwin = { version = "0.14.2", default-features = false, optional = true }
+cargo-zigbuild = { version = "0.16.10", default-features = false, optional = true }
+cargo-xwin = { version = "0.14.3", default-features = false, optional = true }
 
 # log
 tracing = "0.1.36"
 tracing-subscriber = { version = "0.3.15", features = ["env-filter"], optional = true }
 
 # project scaffolding, maturin new/init/generate-ci
 dialoguer = { version = "0.10.2", default-features = false, optional = true }
 console = { version = "0.15.4", optional = true }
-minijinja = { version = "0.31.0", optional = true }
+minijinja = { version = "0.33.0", optional = true }
 
 # upload
 bytesize = { version = "1.0.1", optional = true }
 configparser = { version = "3.0.0", optional = true }
+dirs = { version = "5.0.0", optional = true }
 multipart = { version = "0.18.0", features = ["client"], default-features = false, optional = true }
 ureq = { version = "2.6.1", features = ["gzip", "json", "socks-proxy"], default-features = false, optional = true }
 native-tls = { version = "0.2.8", optional = true }
 rustls = { version = "0.20.8", optional = true }
 rustls-pemfile = { version = "1.0.1", optional = true }
 keyring = { version = "2.0.0", default-features = false, features = ["linux-no-secret-service"], optional = true }
 wild = { version = "2.1.0", optional = true }
@@ -104,15 +104,15 @@
 
 full = ["cli-completion", "cross-compile", "log", "scaffolding", "upload"]
 
 log = ["tracing-subscriber"]
 
 cli-completion = ["dep:clap_complete_command"]
 
-upload = ["ureq", "multipart", "configparser", "bytesize", "dialoguer/password", "url", "wild"]
+upload = ["ureq", "multipart", "configparser", "bytesize", "dialoguer/password", "url", "wild", "dep:dirs"]
 # keyring doesn't support *BSD so it's not enabled in `full` by default
 password-storage = ["upload", "keyring"]
 
 rustls = ["dep:rustls", "ureq?/tls", "cargo-xwin?/rustls-tls", "dep:rustls-pemfile"]
 native-tls = ["dep:native-tls", "ureq?/native-tls", "cargo-xwin?/native-tls", "dep:rustls-pemfile"]
 
 # cross compile using zig or xwin
```

### Comparing `maturin-1.0.0b9/.cirrus.yml` & `maturin-1.0.1/.cirrus.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 env:
   RUST_BACKTRACE: 1
   CARGO_INCREMENTAL: 0
   CARGO_TERM_COLOR: always
   CARGO_REGISTRIES_CRATES_IO_PROTOCOL: sparse
 
 build_and_test: &BUILD_AND_TEST
-  # only run tasks on pull request or bors related branches
-  only_if: $CIRRUS_BRANCH == 'staging' || $CIRRUS_BRANCH == 'trying' || $CIRRUS_PR != ""
+  # only run tasks on pull request or github merge queue branches
+  only_if: $CIRRUS_BRANCH =~ 'gh-readonly-queue/.*' || $CIRRUS_PR != ""
   setup_script:
     - curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y --default-toolchain stable
     - rustup target add wasm32-wasi
     - python3 -m pip install --upgrade cffi virtualenv
   build_script:
     - cargo build
   test_script:
```

### Comparing `maturin-1.0.0b9/Cargo.lock` & `maturin-1.0.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 name = "base64"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e1b586273c5702936fe7b7d6896644d8be71e6314cfe09d3167c95f712589e8"
 
 [[package]]
 name = "base64"
-version = "0.21.0"
+version = "0.21.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a4a4ddaa51a5bc52a6948f74c06d20aaaddb71924eab79b8c97a8c556e942d6a"
+checksum = "604178f6c5c21f02dc555784810edfb88d34ac2c73b2eae109655649ee73ce3d"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -65,27 +65,27 @@
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bstr"
-version = "1.4.0"
+version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3d4260bcc2e8fc9df1eac4919a720effeb63a3f0952f5bf4944adfa18897f09"
+checksum = "a246e68bb43f6cd9db24bea052a53e40405417c5fb372e3d1a8a7f770a564ef5"
 dependencies = [
  "memchr",
  "serde",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.12.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b1ce199063694f33ffb7dd4e0ee620741495c32833cde5aa08f02a0bf96f0c8"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
 
@@ -150,15 +150,15 @@
 checksum = "7ee1e7a7c5bc8f3389f125fb3da214c86d8e21c2b7259923079e0142ac47ffe4"
 dependencies = [
  "cfg-expr",
  "home",
  "once_cell",
  "serde",
  "shell-escape",
- "toml 0.7.3",
+ "toml 0.7.4",
 ]
 
 [[package]]
 name = "cargo-options"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9b8e8daa6b2b84aa7cccd57317d9a9b36d969d75bb95923471f4eabbd36f2955"
@@ -173,17 +173,17 @@
 checksum = "cbdb825da8a5df079a43676dbe042702f1707b1109f713a01420fbb4cc71fa27"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cargo-xwin"
-version = "0.14.2"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00ba77651e6b8d879367dbc0d081dbbae4f44827f0b4d59ea03a790777f5069c"
+checksum = "83f8f065d99c285700e2ea8a10cb7971f59a48c8ec058d2ec2f71ab3f8d692df"
 dependencies = [
  "anyhow",
  "cargo-config2",
  "cargo-options",
  "clap",
  "dirs",
  "fs-err",
@@ -191,17 +191,17 @@
  "path-slash",
  "which",
  "xwin",
 ]
 
 [[package]]
 name = "cargo-zigbuild"
-version = "0.16.7"
+version = "0.16.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00ff7c023d9f668281696d679e2ebc0095275501afb17df6331258c54a9aefda"
+checksum = "065d664a006cb0ede5f2ea22a40e71209c68bdd19a5d6a93d546acb1051a703f"
 dependencies = [
  "anyhow",
  "cargo-options",
  "cargo_metadata",
  "clap",
  "dirs",
  "fs-err",
@@ -237,15 +237,15 @@
  "heck",
  "indexmap",
  "log",
  "proc-macro2",
  "quote",
  "serde",
  "serde_json",
- "syn",
+ "syn 1.0.109",
  "tempfile",
  "toml 0.5.11",
 ]
 
 [[package]]
 name = "cc"
 version = "1.0.79"
@@ -296,33 +296,42 @@
 dependencies = [
  "hashbrown",
  "stacker",
 ]
 
 [[package]]
 name = "clap"
-version = "4.1.10"
+version = "4.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce38afc168d8665cfc75c7b1dd9672e50716a137f433f070991619744a67342a"
+checksum = "906f7fe1da4185b7a282b2bc90172a496f9def1aca4545fe7526810741591e14"
 dependencies = [
- "bitflags",
+ "clap_builder",
  "clap_derive",
+ "once_cell",
+]
+
+[[package]]
+name = "clap_builder"
+version = "4.1.14"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "351f9ad9688141ed83dfd8f5fb998a06225ef444b48ff4dc43de6d409b7fd10b"
+dependencies = [
+ "bitflags",
  "clap_lex",
  "is-terminal",
- "once_cell",
  "strsim",
  "termcolor",
  "terminal_size",
 ]
 
 [[package]]
 name = "clap_complete"
-version = "4.1.6"
+version = "4.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40d3120a421cd111c43f1a6c7d0dd83bb6aaa0659c164468a1654014632a5ec6"
+checksum = "1594fe2312ec4abf402076e407628f5c313e54c32ade058521df4ee34ecac8a8"
 dependencies = [
  "clap",
 ]
 
 [[package]]
 name = "clap_complete_command"
 version = "0.5.1"
@@ -333,53 +342,49 @@
  "clap_complete",
  "clap_complete_fig",
  "clap_complete_nushell",
 ]
 
 [[package]]
 name = "clap_complete_fig"
-version = "4.1.2"
+version = "4.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2171bc6242ad7a1801422bff039574449b5bd832b715222e500714ce10f91a54"
+checksum = "f3af28956330989baa428ed4d3471b853715d445c62de21b67292e22cf8a41fa"
 dependencies = [
  "clap",
  "clap_complete",
 ]
 
 [[package]]
 name = "clap_complete_nushell"
-version = "0.1.10"
+version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c7fa41f5e6aa83bd151b70fd0ceaee703d68cd669522795dc812df9edad1252c"
+checksum = "5d02bc8b1a18ee47c4d2eec3fb5ac034dc68ebea6125b1509e9ccdffcddce66e"
 dependencies = [
  "clap",
  "clap_complete",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.1.9"
+version = "4.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fddf67631444a3a3e3e5ac51c36a5e01335302de677bd78759eaa90ab1f46644"
+checksum = "81d7dc0031c3a59a04fc2ba395c8e2dd463cba1859275f065d225f6122221b45"
 dependencies = [
  "heck",
- "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.3.3"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "033f6b7a4acb1f358c742aaca805c939ee73b4c6209ae4318ec7aca81c42e646"
-dependencies = [
- "os_str_bytes",
-]
+checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
 
 [[package]]
 name = "cli-table"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adfbb116d9e2c4be7011360d0c0bee565712c11e969c9609b25b619366dc379d"
 dependencies = [
@@ -416,15 +421,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c3d79fbe8970a77e3e34151cc13d3b3e248aa0faaecb9f6091fa07ebefe5ad60"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
  "unicode-width",
- "windows-sys",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "content_inspector"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7bda66e858c683005a53a9a60c69a4aca7eeaa45d124526e389f7aec8e62f38"
@@ -446,17 +451,17 @@
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.6"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "280a9f2d8b3a38871a3c8a46fb80db65e5e5ed97da80c4d08bf27fb63e35e181"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
 version = "1.3.2"
@@ -522,22 +527,22 @@
 [[package]]
 name = "ctor"
 version = "0.1.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d2301688392eb071b0bf1a37be05c469d3cc4dbbd95df672fe28ab021e6a096"
 dependencies = [
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "data-encoding"
-version = "2.3.3"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23d8666cb01533c39dde32bcbab8e227b4ed6679b2c925eba05feabea39508fb"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
 
 [[package]]
 name = "dialoguer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "59c6f2989294b9a498d3ad5491a79c6deb604617378e1cdc4bfc1c1361fe2f87"
 dependencies = [
@@ -550,40 +555,41 @@
 name = "diff"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56254986775e3233ffa9c4d7d3faaf6d36a2c09d30b20687e9f88bc8bafc16c8"
 
 [[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "dirs"
-version = "4.0.0"
+version = "5.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ca3aa72a6f96ea37bbc5aa912f6788242832f75369bdfdadcb0e38423f100059"
+checksum = "44c45a9d03d6676652bcb5e724c7e988de1acad23a711b5217ab9cbecbec2225"
 dependencies = [
  "dirs-sys",
 ]
 
 [[package]]
 name = "dirs-sys"
-version = "0.3.7"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1b1d1d91c932ef41c0f2663aa8b0ca0342d444d842c06914aa0a7e352d0bada6"
+checksum = "520f05a5cbd335fae5a99ff7a6ab8627577660ee5cfd6a94a6a929b52ff0321c"
 dependencies = [
  "libc",
+ "option-ext",
  "redox_users",
- "winapi",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "dunce"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56ce8c6da7551ec6c462cbaf3bfbc75131ebbfa1c944aeaa9dab51ca1c5f0c3b"
@@ -617,14 +623,25 @@
 dependencies = [
  "errno-dragonfly",
  "libc",
  "winapi",
 ]
 
 [[package]]
+name = "errno"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
+dependencies = [
+ "errno-dragonfly",
+ "libc",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "errno-dragonfly"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
@@ -646,22 +663,22 @@
 checksum = "67f07131a2b944c2b42b6a58104600ef049c11df5454478d2b44ff5dfe58d149"
 dependencies = [
  "goblin",
 ]
 
 [[package]]
 name = "filetime"
-version = "0.2.19"
+version = "0.2.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e884668cd0c7480504233e951174ddc3b382f7c2666e3b7310b5c4e7b0c37f9"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "flate2"
 version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
@@ -778,14 +795,20 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee512640fe35acbfb4bb779db6f0d80704c2cacfa2e39b601ef3e3f47d1ae4c7"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "hermit-abi"
+version = "0.3.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fed44880c466736ef9a5c5b5facefb5ed0785676d0c02d612db14e54f0d84286"
+
+[[package]]
 name = "home"
 version = "0.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "747309b4b440c06d57b0b25f2aee03ee9b5e5397d288c60e21fc709bb98a7408"
 dependencies = [
  "winapi",
 ]
@@ -848,15 +871,15 @@
 name = "indicatif"
 version = "0.17.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cef509aa9bc73864d6756f0d34d35504af3cf0844373afe9b8669a5b8005a729"
 dependencies = [
  "console",
  "number_prefix",
- "portable-atomic",
+ "portable-atomic 0.3.20",
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
 version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -869,32 +892,33 @@
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "1.0.4"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7d6c6f8c91b4b9ed43484ad1a938e393caf35960fce7f82a040497207bd8e9e"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
+ "hermit-abi 0.3.1",
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.2"
+version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28dfb6c8100ccc63462345b67d1bbc3679177c75ee4bf59bf29c8b1d110b8189"
+checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.3.1",
  "io-lifetimes",
- "rustix",
- "windows-sys",
+ "rustix 0.37.19",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
@@ -906,26 +930,26 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445dde2150c55e483f3d8416706b97ec8e8237c307e5b7b4b8dd15e6af2a0730"
+checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "keyring"
-version = "2.0.2"
+version = "2.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09484a398d672f7332798206e3561dfa022dd4b1fe9d3a638e6bf9cc15a590c5"
+checksum = "e319fe0cb5b29a55cdb228df3f651b6c8cdc5b19520f3e62c8f111dc2582026c"
 dependencies = [
  "byteorder",
  "lazy_static",
  "linux-keyutils",
  "security-framework",
  "winapi",
 ]
@@ -945,17 +969,17 @@
  "fs-err",
  "glob",
  "goblin",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "linux-keyutils"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f27bb67f6dd1d0bb5ab582868e4f65052e58da6401188a08f0da09cf512b84b"
 dependencies = [
@@ -966,14 +990,20 @@
 [[package]]
 name = "linux-raw-sys"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f051f77a7c8e6957c0696eac88f26b0117e54f52d3fc682ab19397a8812846a4"
 
 [[package]]
+name = "linux-raw-sys"
+version = "0.3.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
+
+[[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
  "autocfg",
  "scopeguard",
@@ -1012,18 +1042,18 @@
 checksum = "8263075bb86c5a1b1427b5ae862e8889656f126e9f77c484496e8b47cf5c5558"
 dependencies = [
  "regex-automata",
 ]
 
 [[package]]
 name = "maturin"
-version = "1.0.0-beta.9"
+version = "1.0.1"
 dependencies = [
  "anyhow",
- "base64 0.13.1",
+ "base64 0.21.2",
  "bytesize",
  "cargo-config2",
  "cargo-options",
  "cargo-xwin",
  "cargo-zigbuild",
  "cargo_metadata",
  "cbindgen",
@@ -1069,15 +1099,15 @@
  "sha2",
  "tar",
  "target-lexicon",
  "tempfile",
  "textwrap",
  "thiserror",
  "time",
- "toml 0.7.3",
+ "toml 0.7.4",
  "toml_edit",
  "tracing",
  "tracing-subscriber",
  "trycmd",
  "ureq",
  "url",
  "which",
@@ -1114,17 +1144,17 @@
 dependencies = [
  "mime",
  "unicase",
 ]
 
 [[package]]
 name = "minijinja"
-version = "0.31.1"
+version = "0.33.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0b1dbc390e4447b2500c4071d7bc2a808cf07e925bae6b92db8a3c3eae773c58"
+checksum = "933dc6e6e1f909926a2f6bf72ba8b8d6e38ab4f92778c77ea898001e044a30eb"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
@@ -1197,19 +1227,19 @@
 name = "normalize-line-endings"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61807f77802ff30975e01f4f071c8ba10c022052f98b3294119f3e615d13e5be"
 
 [[package]]
 name = "normpath"
-version = "1.0.1"
+version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3a37f4eb793d70ebef49f4643fe4b8c0e60d266e3fb607158e64b6ee24b0d6d4"
+checksum = "ec60c60a693226186f5d6edf073232bfb6464ed97eb22cf3b01c1e8198fd97f5"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "nu-ansi-term"
 version = "0.46.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77a8165726e8236064dbb45459242600304b42a5ea24ee2948e18e023bf7ba84"
@@ -1220,15 +1250,15 @@
 
 [[package]]
 name = "num_cpus"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fac9e2da13b5eb447a6ce3d392f23a29d8694bff781bf03a16cd9ac8697593b"
 dependencies = [
- "hermit-abi",
+ "hermit-abi 0.2.6",
  "libc",
 ]
 
 [[package]]
 name = "number_prefix"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1238,83 +1268,83 @@
 name = "once_cell"
 version = "1.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b7e5500299e16ebb147ae15a00a942af264cf3688f47923b8fc2cd5858f23ad3"
 
 [[package]]
 name = "openssl"
-version = "0.10.50"
+version = "0.10.52"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e30d8bc91859781f0a943411186324d580f2bbeb71b452fe91ae344806af3f1"
+checksum = "01b8574602df80f7b85fdfc5392fa884a4e3b3f4f35402c070ab34c3d3f78d56"
 dependencies = [
  "bitflags",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
 
 [[package]]
 name = "openssl-macros"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b501e44f11665960c7e7fcf062c7d96a14ade4aa98116c004b2e37b5be7d736c"
+checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-src"
-version = "111.25.2+1.1.1t"
+version = "111.25.3+1.1.1t"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "320708a054ad9b3bf314688b5db87cf4d6683d64cfc835e2337924ae62bf4431"
+checksum = "924757a6a226bf60da5f7dd0311a34d2b52283dd82ddeb103208ddc66362f80c"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.85"
+version = "0.9.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d3d193fb1488ad46ffe3aaabc912cc931d02ee8518fe2959aea8ef52718b0c0"
+checksum = "8e17f59264b2809d77ae94f0e1ebabc434773f370d6ca667bd223ea10e06cc7e"
 dependencies = [
  "cc",
  "libc",
  "openssl-src",
  "pkg-config",
  "vcpkg",
 ]
 
 [[package]]
+name = "option-ext"
+version = "0.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "04744f49eae99ab78e0d5c0b603ab218f515ea8cfe5a456d7629ad883a3b6e7d"
+
+[[package]]
 name = "os_pipe"
-version = "1.1.2"
+version = "1.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c6a252f1f8c11e84b3ab59d7a488e48e4478a93937e027076638c49536204639"
+checksum = "0ae859aa07428ca9a929b936690f8b12dc5f11dd8c6992a18ca93919f28bc177"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
-name = "os_str_bytes"
-version = "6.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceedf44fb00f2d1984b0bc98102627ce622e083e49a5bacdb3e514fa4238e267"
-
-[[package]]
 name = "output_vt100"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "628223faebab4e3e40667ee0b2336d34a5b960ff60ea743ddfdbcf7770bcfb66"
 dependencies = [
  "winapi",
 ]
@@ -1341,15 +1371,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba1ef8814b5c993410bb3adfad7a5ed269563e4a2f90c41f5d85be7fb47133bf"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "path-slash"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1e91099d4268b0e11973f036e885d652fb0b21fedcf69738c627f94db6a44f42"
@@ -1393,39 +1423,48 @@
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "plain"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b4596b6d070b27117e987119b4dac604f3c58cfb0b191112e24771b2faeac1a6"
 
 [[package]]
 name = "platform-info"
-version = "1.0.2"
+version = "2.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4e7c23cfae725ae06d9e43010153fa77bdfa8c827bf08fe4beeb2a3514e6be12"
+checksum = "827dc4f7a81331d48c8abf11b5ac18673b390d33e9632327e286d940289aefab"
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "portable-atomic"
-version = "0.3.19"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26f6a7b87c2e435a3241addceeeff740ff8b7e76b74c13bf9acb17fa454ea00b"
+checksum = "e30165d31df606f5726b090ec7592c308a0eaf61721ff64c9a3018e344a8753e"
+dependencies = [
+ "portable-atomic 1.3.2",
+]
+
+[[package]]
+name = "portable-atomic"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc59d1bcc64fc5d021d67521f818db868368028108d37f0e98d74e33f68297b5"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -1438,42 +1477,18 @@
  "ctor",
  "diff",
  "output_vt100",
  "yansi",
 ]
 
 [[package]]
-name = "proc-macro-error"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
-dependencies = [
- "proc-macro-error-attr",
- "proc-macro2",
- "quote",
- "syn",
- "version_check",
-]
-
-[[package]]
-name = "proc-macro-error-attr"
-version = "1.0.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
-dependencies = [
- "proc-macro2",
- "quote",
- "version_check",
-]
-
-[[package]]
 name = "proc-macro2"
-version = "1.0.56"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "psm"
 version = "0.1.21"
@@ -1489,15 +1504,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f04dbbb336bd88583943c7cd973a32fed323578243a7569f40cb0c7da673321b"
 dependencies = [
  "indexmap",
  "pep440_rs",
  "pep508_rs",
  "serde",
- "toml 0.7.3",
+ "toml 0.7.4",
 ]
 
 [[package]]
 name = "python-pkginfo"
 version = "0.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b8cf2d8981a1c967eebacac69c68a54d9786c1b84b813841d0aab2994705608"
@@ -1509,17 +1524,17 @@
  "tar",
  "thiserror",
  "zip",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "quoted_printable"
 version = "0.4.8"
@@ -1626,15 +1641,15 @@
 
 [[package]]
 name = "rfc2047-decoder"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61fc4b4e52897c3e30b12b7e9b04461215b647fbe66f6def60dd8edbce14ec2e"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
  "charset",
  "chumsky",
  "memchr",
  "quoted_printable",
  "thiserror",
 ]
 
@@ -1665,19 +1680,33 @@
 [[package]]
 name = "rustix"
 version = "0.36.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4fdebc4b395b7fbb9ab11e462e20ed9051e7b16e42d24042c776eca0ac81b03"
 dependencies = [
  "bitflags",
- "errno",
+ "errno 0.2.8",
  "io-lifetimes",
  "libc",
- "linux-raw-sys",
- "windows-sys",
+ "linux-raw-sys 0.1.4",
+ "windows-sys 0.42.0",
+]
+
+[[package]]
+name = "rustix"
+version = "0.37.19"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+dependencies = [
+ "bitflags",
+ "errno 0.3.1",
+ "io-lifetimes",
+ "libc",
+ "linux-raw-sys 0.3.8",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustls"
 version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fff78fc74d175294f4e83b28343315ffcfb114b156f0185e9741cb5570f50e2f"
@@ -1690,15 +1719,15 @@
 
 [[package]]
 name = "rustls-pemfile"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d194b56d58803a43635bdc398cd17e383d6f71f9182b9a192c127ca42494a59b"
 dependencies = [
- "base64 0.21.0",
+ "base64 0.21.2",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f3208ce4d8448b3f3e7d168a73f5e0c43a61e32930de3bceeccedb388b6bf06"
@@ -1720,15 +1749,15 @@
 
 [[package]]
 name = "schannel"
 version = "0.1.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "713cfb06c7059f3588fb8044c0fad1d09e3c01d225e25b9220dbfdcf16dbb1b3"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
@@ -1746,45 +1775,45 @@
 name = "scroll_derive"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bdbda6ac5cd1321e724fa9cee216f3a61885889b896f073b8f82322789c5250e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "sct"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d53dcdb7c9f8158937a7981b48accfd39a43af418591a5d008c7b22b5e1b7ca4"
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "security-framework"
-version = "2.8.2"
+version = "2.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a332be01508d814fed64bf28f798a146d73792121129962fdf335bb3c49a4254"
+checksum = "1fc758eb7bffce5b308734e9b0c1468893cae9ff70ebf13e7090be8dcbcc83a8"
 dependencies = [
  "bitflags",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.8.0"
+version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31c9bb296072e961fcbd8853511dd39c2d8be2deb1e17c6860b1d30732b323b4"
+checksum = "f51d0c0d83bec45f16480d0ce0058397a69e48fcdc52d1dc8855fb68acbd31a7"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
@@ -1793,48 +1822,48 @@
 checksum = "bebd363326d05ec3e2f532ab7660680f3b02130d780c299bca73469d521bc0ed"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.155"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71f2b4817415c6d4210bfe1c7bfcf4801b2d904cb4d0e1a8fdb651013c9e86b8"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.155"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d071a94a3fac4aff69d023a7f411e33f40f3483f8c5190b1953822b6b76d7630"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0efd8caf556a6cebd3b285caf480045fcc1ac04f6bd786b09a6f11af30c4fcf4"
+checksum = "93107647184f6027e3b7dcb2e11034cf95ffa1e3a682c67951963ac69c1c007d"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "sha2"
 version = "0.10.6"
@@ -1905,15 +1934,15 @@
  "normalize-line-endings",
  "os_pipe",
  "similar",
  "snapbox-macros",
  "tempfile",
  "wait-timeout",
  "walkdir",
- "windows-sys",
+ "windows-sys 0.42.0",
  "yansi",
 ]
 
 [[package]]
 name = "snapbox-macros"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1969,14 +1998,25 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
 name = "tar"
 version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b55807c0344e1e6c04d7c965f5289c39a8d94ae23ed5c0b57aabac549f871c6"
 dependencies = [
  "filetime",
  "libc",
@@ -1994,35 +2034,35 @@
 version = "3.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af18f7ae1acd354b992402e9ec5864359d693cd8a79dcbef59f76891701c1e95"
 dependencies = [
  "cfg-if",
  "fastrand",
  "redox_syscall",
- "rustix",
- "windows-sys",
+ "rustix 0.36.7",
+ "windows-sys 0.42.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be55cf8942feac5c765c2c993422806843c9a9a45d4d5c407ad6dd2ea95eb9b6"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "terminal_size"
-version = "0.2.3"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb20089a8ba2b69debd491f8d2d023761cbf196e999218c591fa1e7e15a21907"
+checksum = "8e6bf6f19e9f8ed8d4048dc22981458ebcf406d67e94cd422e5ecd73d63b3237"
 dependencies = [
- "rustix",
- "windows-sys",
+ "rustix 0.37.19",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
@@ -2030,64 +2070,64 @@
  "smawk",
  "unicode-linebreak",
  "unicode-width",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5ab016db510546d856297882807df8da66a16fb8c4101cb8b30054b0d5b2d9c"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.39"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5420d42e90af0c38c3290abcca25b9b3bdf379fc9f55c528f53a269d9c9a267e"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
 dependencies = [
  "cfg-if",
  "once_cell",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.21"
+version = "0.3.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
+checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
 dependencies = [
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.1"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
+checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
 
 [[package]]
 name = "time-macros"
-version = "0.2.9"
+version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
+checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tinyvec"
 version = "1.6.0"
@@ -2110,38 +2150,38 @@
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml"
-version = "0.7.3"
+version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b403acf6f2bb0859c93c7f0d967cb4a75a7ac552100f9322faf64dc047669b21"
+checksum = "d6135d499e69981f9ff0ef2167955a5333c35e36f6937d382974566b3d5b94ec"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.1"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
+checksum = "5a76a9312f5ba4c2dec6b9161fdf25d87ad8a09256ccea5a556fef03c706a10f"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.19.8"
+version = "0.19.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
+checksum = "2380d56e8670370eee6566b0bfd4265f65b3f432e8c6d85623f728d4fa31f739"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
@@ -2157,28 +2197,28 @@
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
 name = "tracing-attributes"
-version = "0.1.23"
+version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4017f8f45139870ca7e672686113917c71c7a6e02d4924eda67186083c03081a"
+checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tracing-core"
-version = "0.1.30"
+version = "0.1.31"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "24eb03ba0eab1fd845050058ce5e616558e8f8d8fca633e6b163fe25c797213a"
+checksum = "0955b8137a1df6f1a2e9a37d8a6656291ff0297c1a97c24e0d8425fe2312f79a"
 dependencies = [
  "once_cell",
  "valuable",
 ]
 
 [[package]]
 name = "tracing-log"
@@ -2268,17 +2308,17 @@
 name = "unicode-bidi"
 version = "0.3.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-linebreak"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5faade31a542b8b35855fff6e8def199853b2da8da256da52f52f1316ee3137"
 dependencies = [
@@ -2337,17 +2377,17 @@
  "idna",
  "percent-encoding",
  "serde",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.3.1"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 
 [[package]]
 name = "valuable"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "830b7e5d4d90034032940e4ace0d9a9a057e7a45cd94e6c007832e39edb82f6d"
 
@@ -2396,71 +2436,71 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31f8dcbc21f30d9b8f2ea926ecb58f6b91192c17e9d33594b3df58b2007ca53b"
+checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "95ce90fd5bcc06af55a641a86428ee4229e44e07033963a2290a8e241607ccb9"
+checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c21f77c0bedc37fd5dc21f897894a5ca01e7bb159884559461862ae90c0b4c5"
+checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2aff81306fcac3c7515ad4e177f521b5c9a15f2b08f4e32d823066102f35a5f6"
+checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.84"
+version = "0.2.86"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0046fef7e28c3804e5e38bfa31ea2a0f73905319b677e57ebe37e49358989b5d"
+checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
 
 [[package]]
 name = "web-sys"
-version = "0.3.61"
+version = "0.3.63"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e33b99f4b23ba3eec1a53ac264e35a755f00e966e0065077d6027c0f575b0b97"
+checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
@@ -2534,66 +2574,132 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.42.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.42.2",
+ "windows_aarch64_msvc 0.42.2",
+ "windows_i686_gnu 0.42.2",
+ "windows_i686_msvc 0.42.2",
+ "windows_x86_64_gnu 0.42.2",
+ "windows_x86_64_gnullvm 0.42.2",
+ "windows_x86_64_msvc 0.42.2",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
+dependencies = [
+ "windows_aarch64_gnullvm 0.48.0",
+ "windows_aarch64_msvc 0.48.0",
+ "windows_i686_gnu 0.48.0",
+ "windows_i686_msvc 0.48.0",
+ "windows_x86_64_gnu 0.48.0",
+ "windows_x86_64_gnullvm 0.48.0",
+ "windows_x86_64_msvc 0.48.0",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
+
+[[package]]
 name = "winnow"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "61de7bac303dc551fe038e2b3cef0f571087a47571ea6e79a87692ac99b99699"
 dependencies = [
  "memchr",
 ]
@@ -2648,17 +2754,17 @@
 name = "zeroize"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2a0956f1ba7c7909bfb66c2e9e4124ab6f6482560f6628b5aaeba39207c9aad9"
 
 [[package]]
 name = "zip"
-version = "0.6.4"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0445d0fbc924bb93539b4316c11afb121ea39296f99a3c4c9edad09e3658cdef"
+checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
  "byteorder",
  "bzip2",
  "crc32fast",
  "crossbeam-utils",
  "flate2",
  "time",
```

### Comparing `maturin-1.0.0b9/Changelog.md` & `maturin-1.0.1/Changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,42 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (for the cli, not for the crate).
 
 ## [Unreleased]
 
+## [1.0.1] - 2023-05-28
+
+* Add more Python 3.12 sysconfigs in [#1629](https://github.com/PyO3/maturin/pull/1629)
+* Fix panicking when no cargo build targets are selected in [#1635](https://github.com/PyO3/maturin/pull/1635)
+
+## [1.0.0] - 2023-05-23
+
+* Add support for multiple `--config-settings` in PEP517 backend in [#1624](https://github.com/PyO3/maturin/pull/1624)
+* Remove deprecated `--universal2` cli option in [#1620](https://github.com/PyO3/maturin/pull/1620),
+  use `--target universal2-apple-darwin` instead.
+
+## [0.15.3] - 2023-05-20
+
+* Fix cross compile Apple universal2 wheels on non-macOS platforms by MisLink in [#1613](https://github.com/PyO3/maturin/pull/1613)
+* Add PEP 517 `config_settings` support in [#1619](https://github.com/PyO3/maturin/pull/1619),
+  deprecate `MATURIN_PEP517_ARGS` in favor of the new `build-args` config setting.
+
+## [0.15.2] - 2023-05-16
+
+* When determining the python module name, use pyproject.toml `project.name` over Cargo.toml `package.name` in [#1608](https://github.com/PyO3/maturin/pull/1608)
+* Fix rewriting `dev-dependencies` in sdist in [#1610](https://github.com/PyO3/maturin/pull/1610)
+
+## [0.15.1] - 2023-05-07
+
+* Fix finding interpreters from bundled sysconfigs in [#1598](https://github.com/PyO3/maturin/pull/1598)
+
+## [0.15.0] - 2023-05-07
+
 * **Breaking Change**: Build with `--no-default-features` by default when bootstrapping from sdist in [#1333](https://github.com/PyO3/maturin/pull/1333)
 * **Breaking Change**: Remove deprecated `sdist-include` option in `pyproject.toml` in [#1335](https://github.com/PyO3/maturin/pull/1335)
 * **Breaking Change**: Remove deprecated `python-source` option in `Cargo.toml` in [#1335](https://github.com/PyO3/maturin/pull/1335)
 * **Breaking Change**: Turn `patchelf` version warning into a hard error in [#1335](https://github.com/PyO3/maturin/pull/1335)
 * **Breaking Change**: [`uniffi_bindgen` CLI](https://mozilla.github.io/uniffi-rs/tutorial/Prerequisites.html#the-uniffi-bindgen-cli-tool) is required for building `uniffi` bindings wheels in [#1352](https://github.com/PyO3/maturin/pull/1352)
 * Add Cargo compile targets configuration for filtering multiple bin targets in [#1339](https://github.com/PyO3/maturin/pull/1339)
 * Respect `rustflags` settings in cargo configuration file in [#1405](https://github.com/PyO3/maturin/pull/1405)
@@ -846,15 +874,21 @@
 
  * Show a progress bar for cargo's compile progress
 
 ## 0.1.0 - 2018-08-22
 
  * Initial Release
 
-[Unreleased]: https://github.com/pyo3/maturin/compare/v0.14.17...HEAD
+[Unreleased]: https://github.com/pyo3/maturin/compare/v1.0.1...HEAD
+[1.0.1]: https://github.com/pyo3/maturin/compare/v1.0.0...v1.0.1
+[1.0.0]: https://github.com/pyo3/maturin/compare/v0.15.3...v1.0.0
+[0.15.3]: https://github.com/pyo3/maturin/compare/v0.15.2...v0.15.3
+[0.15.2]: https://github.com/pyo3/maturin/compare/v0.15.1...v0.15.2
+[0.15.1]: https://github.com/pyo3/maturin/compare/v0.15.0...v0.15.1
+[0.15.0]: https://github.com/pyo3/maturin/compare/v0.14.17...v0.15.0
 [0.14.17]: https://github.com/pyo3/maturin/compare/v0.14.16...v0.14.17
 [0.14.16]: https://github.com/pyo3/maturin/compare/v0.14.15...v0.14.16
 [0.14.15]: https://github.com/pyo3/maturin/compare/v0.14.14...v0.14.15
 [0.14.14]: https://github.com/pyo3/maturin/compare/v0.14.13...v0.14.14
 [0.14.13]: https://github.com/pyo3/maturin/compare/v0.14.12...v0.14.13
 [0.14.12]: https://github.com/pyo3/maturin/compare/v0.14.11...v0.14.12
 [0.14.11]: https://github.com/pyo3/maturin/compare/v0.14.10...v0.14.11
```

### Comparing `maturin-1.0.0b9/Code-of-Conduct.md` & `maturin-1.0.1/Code-of-Conduct.md`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/Dockerfile` & `maturin-1.0.1/Dockerfile`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/README.md` & `maturin-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Maturin
 
 _formerly pyo3-pack_
 
 [![Actions Status](https://img.shields.io/github/actions/workflow/status/PyO3/maturin/test.yml?branch=main&logo=github&style=flat-square)](https://github.com/PyO3/maturin/actions)
 [![FreeBSD](https://img.shields.io/cirrus/github/PyO3/maturin/main?logo=CircleCI&style=flat-square)](https://cirrus-ci.com/github/PyO3/maturin)
-[![Bors enabled](https://bors.tech/images/badge_small.svg)](https://app.bors.tech/repositories/55651)
 [![Crates.io](https://img.shields.io/crates/v/maturin.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
 [![PyPI](https://img.shields.io/pypi/v/maturin.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
 [![Maturin User Guide](https://img.shields.io/badge/user-guide-brightgreen?logo=readthedocs&style=flat-square)](https://maturin.rs)
 [![Chat on Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg?logo=gitter&style=flat-square)](https://gitter.im/PyO3/Lobby)
 
 Build and publish crates with pyo3, rust-cpython, cffi and uniffi bindings as well as rust binaries as python packages.
 
@@ -117,14 +116,15 @@
 You can specify a different python source directory in `pyproject.toml` by setting `tool.maturin.python-source`, for example
 
 **pyproject.toml**
 
 ```toml
 [tool.maturin]
 python-source = "python"
+module-name = "my_project._lib_name"
 ```
 
 then the project structure would look like this:
 
 ```
 my-project
 ├── Cargo.toml
@@ -150,20 +150,32 @@
 
 ```
 my-project
 ├── Cargo.toml
 ├── my_project
 │   ├── __init__.py
 │   ├── bar.py
-│   └── my_project.cpython-36m-x86_64-linux-gnu.so
+│   └── _lib_name.cpython-36m-x86_64-linux-gnu.so
 ├── README.md
 └── src
     └── lib.rs
 ```
 
+When doing this also be sure to set the module name in your code to match the last part of `module-name` (don't include the package path):
+
+```
+#[pymodule]
+#[pyo3(name="_lib_name")]
+fn my_lib_name(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+    m.add_class::<MyPythonRustClass>()?;
+    Ok(())
+}
+```
+
+
 ## Python metadata
 
 maturin supports [PEP 621](https://www.python.org/dev/peps/pep-0621/), you can specify python package metadata in `pyproject.toml`.
 maturin merges metadata from `Cargo.toml` and `pyproject.toml`, `pyproject.toml` take precedence over `Cargo.toml`.
 
 To specify python dependencies, add a list `dependencies` in a `[project]` section in the `pyproject.toml`. This list is equivalent to `install_requires` in setuptools:
 
@@ -191,15 +203,15 @@
 
 ## Source distribution
 
 maturin supports building through `pyproject.toml`. To use it, create a `pyproject.toml` next to your `Cargo.toml` with the following content:
 
 ```toml
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 ```
 
 If a `pyproject.toml` with a `[build-system]` entry is present, maturin can build a source distribution of your package when `--sdist` is specified.
 The source distribution will contain the same files as `cargo package`. To only build a source distribution, pass `--interpreter` without any values.
 
 You can then e.g. install your package with `pip install .`. With `pip install . -v` you can see the output of cargo and maturin.
@@ -207,15 +219,15 @@
 You can use the options `compatibility`, `skip-auditwheel`, `bindings`, `strip` and common Cargo build options such as `features` under `[tool.maturin]` the same way you would when running maturin directly.
 The `bindings` key is required for cffi and bin projects as those can't be automatically detected. Currently, all builds are in release mode (see [this thread](https://discuss.python.org/t/pep-517-debug-vs-release-builds/1924) for details).
 
 For a non-manylinux build with cffi bindings you could use the following:
 
 ```toml
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
 bindings = "cffi"
 compatibility = "linux"
 ```
```

### Comparing `maturin-1.0.0b9/deny.toml` & `maturin-1.0.1/deny.toml`

 * *Files 3% similar despite different names*

```diff
@@ -118,14 +118,15 @@
 # aren't accepted for every possible crate as with the normal allow list
 exceptions = [
     # Each entry is the crate and version constraint, and its specific allow
     # list
     { allow = ["ISC", "MIT", "OpenSSL"], name = "ring" },
     { allow = ["MPL-2.0"], name = "webpki-roots" },
     { allow = ["MPL-2.0"], name = "cbindgen" },
+    { allow = ["MPL-2.0"], name = "option-ext" },
     { allow = ["Unicode-DFS-2016"], name = "unicode-ident" },
     { allow = ["MIT", "LGPL-3.0"], name = "configparser" },
 ]
 
 # Some crates don't have (easily) machine readable licensing information,
 # adding a clarification entry for it allows you to manually specify the
 # licensing information
@@ -177,21 +178,26 @@
 ]
 # Certain crates/versions that will be skipped when doing duplicate detection.
 skip = [
     #{ name = "ansi_term", version = "=0.11.0" },
     { name = "base64", version = "0.13.1" },
     # from cbindgen
     { name = "toml", version = "0.5.11" },
+    { name = "syn" },
+    { name = "rustix", version = "0.36.7" },
+    { name = "linux-raw-sys", version = "0.1.4" },
+    { name = "portable-atomic", version = "0.3.20" },
 ]
 # Similarly to `skip` allows you to skip certain crates during duplicate
 # detection. Unlike skip, it also includes the entire tree of transitive
 # dependencies starting at the specified crate, up to a certain depth, which is
 # by default infinite
 skip-tree = [
     #{ name = "ansi_term", version = "=0.11.0", depth = 20 },
+    { name = "windows-sys", version = "0.42.0" },
 ]
 
 # This section is considered when running `cargo deny check sources`.
 # More documentation about the 'sources' section can be found here:
 # https://embarkstudios.github.io/cargo-deny/checks/sources/cfg.html
 [sources]
 # Lint level for what to happen when a crate from a crate registry that is not
```

### Comparing `maturin-1.0.0b9/license-apache` & `maturin-1.0.1/license-apache`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/license-mit` & `maturin-1.0.1/license-mit`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/maturin/__init__.py` & `maturin-1.0.1/maturin/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,16 +28,29 @@
 
 def get_config() -> Dict[str, str]:
     with open("pyproject.toml", "rb") as fp:
         pyproject_toml = tomllib.load(fp)
     return pyproject_toml.get("tool", {}).get("maturin", {})
 
 
-def get_maturin_pep517_args() -> list[str]:
-    args = shlex.split(os.getenv("MATURIN_PEP517_ARGS", ""))
+def get_maturin_pep517_args(
+    config_settings: Mapping[str, Any] | None = None
+) -> list[str]:
+    build_args = config_settings.get("build-args") if config_settings else None
+    if build_args is None:
+        env_args = os.getenv("MATURIN_PEP517_ARGS", "")
+        if env_args:
+            print(
+                f"'MATURIN_PEP517_ARGS' is deprecated, use `--config-settings build-args='{env_args}'` instead."
+            )
+        args = shlex.split(env_args)
+    elif isinstance(build_args, str):
+        args = shlex.split(build_args)
+    else:
+        args = build_args
     return args
 
 
 def _additional_pep517_args() -> list[str]:
     # Support building for 32-bit Python on x64 Windows
     if platform.system().lower() == "windows" and platform.machine().lower() == "amd64":
         pointer_width = struct.calcsize("P") * 8
@@ -64,15 +77,15 @@
         "--compatibility",
         "off",
     ]
     command.extend(_additional_pep517_args())
     if editable:
         command.append("--editable")
 
-    pep517_args = get_maturin_pep517_args()
+    pep517_args = get_maturin_pep517_args(config_settings)
     if pep517_args:
         command.extend(pep517_args)
 
     print("Running `{}`".format(" ".join(command)))
     sys.stdout.flush()
     result = subprocess.run(command, stdout=subprocess.PIPE)
     sys.stdout.buffer.write(result.stdout)
@@ -181,15 +194,15 @@
         metadata_directory,
         # PEP 517 specifies that only `sys.executable` points to the correct
         # python interpreter
         "--interpreter",
         sys.executable,
     ]
     command.extend(_additional_pep517_args())
-    pep517_args = get_maturin_pep517_args()
+    pep517_args = get_maturin_pep517_args(config_settings)
     if pep517_args:
         command.extend(pep517_args)
 
     print("Running `{}`".format(" ".join(command)))
     try:
         _output = subprocess.check_output(command)
     except subprocess.CalledProcessError as e:
```

### Comparing `maturin-1.0.0b9/maturin/__main__.py` & `maturin-1.0.1/maturin/__main__.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/maturin/import_hook.py` & `maturin-1.0.1/maturin/import_hook.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/noxfile.py` & `maturin-1.0.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/pyproject.toml` & `maturin-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/setup.py` & `maturin-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # Note that this is really only a workaround for bootstrapping and not suited
 # for general purpose packaging, i.e. only building a wheel (as in
 # `python setup.py bdist_wheel`) and installing (as in
 # `pip install <source dir>`) are supported. For creating a source distribution
 # for maturin itself use `maturin sdist`.
 
 import os
+import shlex
 
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 from setuptools import setup
 
@@ -43,15 +44,15 @@
 with open("Cargo.toml", "rb") as fp:
     version = tomllib.load(fp)["package"]["version"]
 
 # Use `--no-default-features` by default for a minimal build to support PEP 517.
 # `MATURIN_SETUP_ARGS` env var can be used to pass customized arguments to cargo.
 cargo_args = ["--no-default-features"]
 if os.getenv("MATURIN_SETUP_ARGS"):
-    cargo_args = os.getenv("MATURIN_SETUP_ARGS").split()
+    cargo_args = shlex.split(os.getenv("MATURIN_SETUP_ARGS", ""))
 
 setup(
     name="maturin",
     author="konstin",
     author_email="konstin@mailbox.org",
     url="https://github.com/pyo3/maturin",
     description="Build and publish crates with pyo3, rust-cpython and cffi bindings as well as rust binaries as "
```

### Comparing `maturin-1.0.0b9/src/auditwheel/audit.rs` & `maturin-1.0.1/src/auditwheel/audit.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/manylinux-policy.json` & `maturin-1.0.1/src/auditwheel/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/musllinux-policy.json` & `maturin-1.0.1/src/auditwheel/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/musllinux.rs` & `maturin-1.0.1/src/auditwheel/musllinux.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/patchelf.rs` & `maturin-1.0.1/src/auditwheel/patchelf.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/platform_tag.rs` & `maturin-1.0.1/src/auditwheel/platform_tag.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/policy.rs` & `maturin-1.0.1/src/auditwheel/policy.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/auditwheel/repair.rs` & `maturin-1.0.1/src/auditwheel/repair.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/build_context.rs` & `maturin-1.0.1/src/build_context.rs`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,15 @@
                         *minor,
                     )?);
                 }
                 if !non_abi3_interps.is_empty() {
                     let interp_names: HashSet<_> = non_abi3_interps
                         .iter()
                         .map(|interp| match interp.interpreter_kind {
-                            InterpreterKind::CPython => interp.implmentation_name.to_string(),
+                            InterpreterKind::CPython => interp.implementation_name.to_string(),
                             InterpreterKind::PyPy => "PyPy".to_string(),
                         })
                         .collect();
                     eprintln!(
                         "⚠️ Warning: {} does not yet support abi3 so the build artifacts will be version-specific.",
                         interp_names.iter().join(", ")
                     );
@@ -587,17 +587,18 @@
                 format!("emscripten_{release}_wasm32")
             }
             (Os::Wasi, Arch::Wasm32) => {
                 "any".to_string()
             }
             // osname_release_machine fallback for any POSIX system
             (_, _) => {
-                let info = PlatformInfo::new()?;
-                let mut release = info.release().replace(['.', '-'], "_");
-                let mut machine = info.machine().replace([' ', '/'], "_");
+                let info = PlatformInfo::new()
+                    .map_err(|e| anyhow!("Failed to fetch platform information: {e}"))?;
+                let mut release = info.release().to_string_lossy().replace(['.', '-'], "_");
+                let mut machine = info.machine().to_string_lossy().replace([' ', '/'], "_");
 
                 let mut os = target.target_os().to_string().to_ascii_lowercase();
                 // See https://github.com/python/cpython/blob/46c8d915715aa2bd4d697482aa051fe974d440e1/Lib/sysconfig.py#L722-L730
                 if os.starts_with("sunos") {
                     // Solaris / Illumos
                     if let Some((major, other)) = release.split_once('_') {
                         let major_ver: u64 = major.parse().context("illumos major version is not a number")?;
```

### Comparing `maturin-1.0.0b9/src/build_options.rs` & `maturin-1.0.1/src/build_options.rs`

 * *Files 1% similar despite different names*

```diff
@@ -181,19 +181,14 @@
     /// Default to manylinux2014/manylinux_2_17 if you do not specify an `--compatibility`
     ///
     /// Make sure you installed zig with `pip install maturin[zig]`
     #[cfg(feature = "zig")]
     #[arg(long)]
     pub zig: bool,
 
-    /// Control whether to build universal2 wheel for macOS or not.
-    /// Only applies to macOS targets, do nothing otherwise.
-    #[arg(long)]
-    pub universal2: bool,
-
     /// Cargo build options
     #[command(flatten)]
     pub cargo: CargoOptions,
 }
 
 impl Deref for BuildOptions {
     type Target = CargoOptions;
@@ -288,15 +283,15 @@
                                 ext_suffix: ext_suffix.to_string(),
                                 abi_tag,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
-                            implmentation_name: interpreter_kind.to_string().to_ascii_lowercase(),
+                            implementation_name: interpreter_kind.to_string().to_ascii_lowercase(),
                             soabi: soabi.cloned(),
                         });
                     } else {
                         if interpreter.is_empty() && !self.find_interpreter {
                             bail!("Couldn't find any python interpreters. Please specify at least one with -i");
                         }
                         for interp in interpreter {
@@ -356,15 +351,15 @@
                                 ext_suffix: ".pyd".to_string(),
                                 abi_tag: None,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
-                            implmentation_name: "cpython".to_string(),
+                            implementation_name: "cpython".to_string(),
                             soabi: None,
                         }])
                     } else if let Some(config_file) = env::var_os("PYO3_CONFIG_FILE") {
                         let interpreter_config =
                             InterpreterConfig::from_pyo3_config(config_file.as_ref(), target)
                                 .context("Invalid PYO3_CONFIG_FILE")?;
                         Ok(vec![PythonInterpreter::from_config(interpreter_config)])
@@ -383,15 +378,15 @@
                                 ext_suffix: ".pyd".to_string(),
                                 abi_tag: None,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
-                            implmentation_name: "cpython".to_string(),
+                            implementation_name: "cpython".to_string(),
                             soabi: None,
                         }])
                     } else {
                         bail!("Failed to find a python interpreter");
                     }
                 } else {
                     let found_interpreters =
@@ -423,15 +418,15 @@
                                 ext_suffix: "".to_string(),
                                 abi_tag: None,
                                 pointer_width: None,
                             },
                             executable: PathBuf::new(),
                             platform: None,
                             runnable: false,
-                            implmentation_name: "cpython".to_string(),
+                            implementation_name: "cpython".to_string(),
                             soabi: None,
                         }])
                     } else if target.cross_compiling() {
                         let mut interps = Vec::with_capacity(found_interpreters.len());
                         let mut pypys = Vec::new();
                         for interp in found_interpreters {
                             if interp.interpreter_kind.is_pypy() {
@@ -506,21 +501,15 @@
                  (Make sure you have set an appropriate [lib] name or \
                  [tool.maturin] module-name in your pyproject.toml)"
             );
         }
 
         let mut target_triple = self.target.clone();
 
-        let mut universal2 = self.universal2;
-        if universal2 {
-            eprintln!("⚠️  Warning: `--universal2` is deprecated, use `--target universal2-apple-darwin` instead");
-        } else if target_triple.as_deref() == Some("universal2-apple-darwin") {
-            universal2 = true;
-            target_triple = None;
-        }
+        let mut universal2 = target_triple.as_deref() == Some("universal2-apple-darwin");
         // Also try to determine universal2 from ARCHFLAGS environment variable
         if let Ok(arch_flags) = env::var("ARCHFLAGS") {
             let arches: HashSet<&str> = arch_flags
                 .split("-arch")
                 .filter_map(|x| {
                     let x = x.trim();
                     if x.is_empty() {
@@ -537,14 +526,17 @@
                 }
                 (false, true) if target_triple.is_none() => {
                     target_triple = Some("aarch64-apple-darwin".to_string())
                 }
                 _ => {}
             }
         };
+        if universal2 {
+            target_triple = None;
+        }
 
         let target = Target::from_target_triple(target_triple)?;
 
         let wheel_dir = match self.out {
             Some(ref dir) => dir.clone(),
             None => PathBuf::from(&cargo_metadata.target_directory).join("wheels"),
         };
@@ -651,14 +643,17 @@
             .target_dir
             .clone()
             .unwrap_or_else(|| cargo_metadata.target_directory.clone().into_std_path_buf());
 
         let config_targets = pyproject.and_then(|x| x.targets());
         let compile_targets =
             filter_cargo_targets(&cargo_metadata, bridge, config_targets.as_deref())?;
+        if compile_targets.is_empty() {
+            bail!("No Cargo targets to build, please check your bindings configuration in pyproject.toml.");
+        }
 
         let crate_name = cargo_toml.package.name;
         Ok(BuildContext {
             target,
             compile_targets,
             project_layout,
             pyproject_toml_path,
@@ -1053,41 +1048,53 @@
 /// fallback to bundled sysconfig if not found in host machine
 fn find_interpreter(
     bridge: &BridgeModel,
     interpreter: &[PathBuf],
     target: &Target,
     requires_python: Option<&VersionSpecifiers>,
 ) -> Result<Vec<PythonInterpreter>> {
-    let mut interpreters = Vec::new();
+    let mut found_interpreters = Vec::new();
     if !interpreter.is_empty() {
         let mut missing = Vec::new();
         for interp in interpreter {
             match PythonInterpreter::check_executable(interp.clone(), target, bridge) {
-                Ok(Some(interp)) => interpreters.push(interp),
+                Ok(Some(interp)) => found_interpreters.push(interp),
                 _ => missing.push(interp.clone()),
             }
         }
         if !missing.is_empty() {
             let sysconfig_interps =
                 find_interpreter_in_sysconfig(&missing, target, requires_python)?;
-            interpreters.extend(sysconfig_interps);
+            found_interpreters.extend(sysconfig_interps);
         }
     } else {
-        interpreters = PythonInterpreter::find_all(target, bridge, requires_python)
+        found_interpreters = PythonInterpreter::find_all(target, bridge, requires_python)
             .context("Finding python interpreters failed")?;
     };
 
-    if interpreters.is_empty() {
-        if let Some(requires_python) = requires_python {
-            bail!("Couldn't find any python interpreters with version {}. Please specify at least one with -i", requires_python);
+    if found_interpreters.is_empty() {
+        if interpreter.is_empty() {
+            if let Some(requires_python) = requires_python {
+                bail!("Couldn't find any python interpreters with version {}. Please specify at least one with -i", requires_python);
+            } else {
+                bail!("Couldn't find any python interpreters. Please specify at least one with -i");
+            }
         } else {
-            bail!("Couldn't find any python interpreters. Please specify at least one with -i");
+            let interps_str = interpreter
+                .iter()
+                .map(|path| format!("'{}'", path.display()))
+                .collect::<Vec<_>>()
+                .join(", ");
+            bail!(
+                "Couldn't find any python interpreters from {}.",
+                interps_str
+            );
         }
     }
-    Ok(interpreters)
+    Ok(found_interpreters)
 }
 
 /// Find python interpreters in the host machine
 fn find_interpreter_in_host(
     bridge: &BridgeModel,
     interpreter: &[PathBuf],
     target: &Target,
@@ -1137,26 +1144,29 @@
             .unwrap_or(false)
         {
             // Eg: -i 3.9 without interpreter kind, assume it's CPython
             (InterpreterKind::CPython, &*python)
         } else {
             bail!("Unsupported Python interpreter: {}", python);
         };
+        if python_ver.is_empty() {
+            continue;
+        }
         let (ver_major, ver_minor) = python_ver
             .split_once('.')
             .context("Invalid python interpreter version")?;
         let ver_major = ver_major.parse::<usize>().with_context(|| {
             format!("Invalid python interpreter major version '{ver_major}', expect a digit")
         })?;
         let ver_minor = ver_minor.parse::<usize>().with_context(|| {
             format!("Invalid python interpreter minor version '{ver_minor}', expect a digit")
         })?;
-        let sysconfig = InterpreterConfig::lookup(target, python_impl, (ver_major, ver_minor))
+        let sysconfig = InterpreterConfig::lookup_one(target, python_impl, (ver_major, ver_minor))
             .with_context(|| {
-                format!("Failed to find a {python_impl} {ver_major}.{ver_minor} interpreter")
+                format!("Failed to find a {python_impl} {ver_major}.{ver_minor} interpreter in known sysconfig")
             })?;
         debug!(
             "Found {} {}.{} in bundled sysconfig",
             sysconfig.interpreter_kind, sysconfig.major, sysconfig.minor,
         );
         interpreters.push(PythonInterpreter::from_config(sysconfig.clone()));
     }
```

### Comparing `maturin-1.0.0b9/src/cargo_toml.rs` & `maturin-1.0.1/src/cargo_toml.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/ci.rs` & `maturin-1.0.1/src/ci.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/compile.rs` & `maturin-1.0.1/src/compile.rs`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 /// specific python version. Returns a mapping from crate type (e.g. cdylib)
 /// to artifact location.
 pub fn compile(
     context: &BuildContext,
     python_interpreter: Option<&PythonInterpreter>,
     targets: &[CompileTarget],
 ) -> Result<Vec<HashMap<String, BuildArtifact>>> {
-    if context.target.is_macos() && context.universal2 {
+    if context.universal2 {
         compile_universal2(context, python_interpreter, targets)
     } else {
         compile_targets(context, python_interpreter, targets)
     }
 }
 
 /// Build an universal2 wheel for macos which contains both an x86 and an aarch64 binary
```

### Comparing `maturin-1.0.0b9/src/cross_compile.rs` & `maturin-1.0.1/src/cross_compile.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/develop.rs` & `maturin-1.0.1/src/develop.rs`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
         interpreter: vec![python.clone()],
         find_interpreter: false,
         bindings,
         out: Some(wheel_dir.path().to_path_buf()),
         skip_auditwheel: false,
         #[cfg(feature = "zig")]
         zig: false,
-        universal2: false,
         cargo: CargoOptions {
             target: target_triple,
             ..cargo_options
         },
     };
 
     let build_context = build_options.into_build_context(release, strip, true)?;
```

### Comparing `maturin-1.0.0b9/src/lib.rs` & `maturin-1.0.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/main.rs` & `maturin-1.0.1/src/main.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/metadata.rs` & `maturin-1.0.1/src/metadata.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/module_writer.rs` & `maturin-1.0.1/src/module_writer.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 //! The wheel format is (mostly) specified in PEP 427
 use crate::project_layout::ProjectLayout;
 use crate::target::Os;
 use crate::{
     pyproject_toml::Format, BridgeModel, Metadata21, PyProjectToml, PythonInterpreter, Target,
 };
 use anyhow::{anyhow, bail, Context, Result};
+use base64::engine::general_purpose::URL_SAFE_NO_PAD;
+use base64::Engine;
 use flate2::write::GzEncoder;
 use flate2::Compression;
 use fs_err as fs;
 use fs_err::File;
 use ignore::overrides::Override;
 use ignore::WalkBuilder;
 use indexmap::IndexMap;
 use normpath::PathExt as _;
 use sha2::{Digest, Sha256};
 use std::collections::{HashMap, HashSet};
 use std::env;
 use std::ffi::OsStr;
 use std::fmt::Write as _;
-#[cfg(target_family = "unix")]
+#[cfg(unix)]
 use std::fs::OpenOptions;
 use std::io;
 use std::io::{Read, Write};
-#[cfg(target_family = "unix")]
-use std::os::unix::fs::OpenOptionsExt;
+#[cfg(unix)]
+use std::os::unix::fs::{OpenOptionsExt, PermissionsExt};
 use std::path::{Path, PathBuf};
 use std::process::{Command, Output};
 use std::str;
 use tempfile::{tempdir, TempDir};
 use tracing::debug;
 use zip::{self, DateTime, ZipWriter};
 
@@ -187,15 +189,15 @@
             }
         }
         .context(format!("Failed to create a file at {}", path.display()))?;
 
         file.write_all(bytes)
             .context(format!("Failed to write to file at {}", path.display()))?;
 
-        let hash = base64::encode_config(Sha256::digest(bytes), base64::URL_SAFE_NO_PAD);
+        let hash = URL_SAFE_NO_PAD.encode(Sha256::digest(bytes));
         self.record.push((
             target.as_ref().to_str().unwrap().to_owned(),
             hash,
             bytes.len(),
         ));
 
         Ok(())
@@ -244,15 +246,15 @@
         if let Some(mtime) = mtime {
             options = options.last_modified_time(mtime);
         }
 
         self.zip.start_file(target.clone(), options)?;
         self.zip.write_all(bytes)?;
 
-        let hash = base64::encode_config(Sha256::digest(bytes), base64::URL_SAFE_NO_PAD);
+        let hash = URL_SAFE_NO_PAD.encode(Sha256::digest(bytes));
         self.record.push((target, hash, bytes.len()));
 
         Ok(())
     }
 }
 
 impl WheelWriter {
@@ -1156,15 +1158,20 @@
                     .expect("No files found for pattern")
                     .filter_map(Result::ok)
                 {
                     let target = source.strip_prefix(pyproject_dir)?.to_path_buf();
                     if source.is_dir() {
                         writer.add_directory(target)?;
                     } else {
-                        writer.add_file(target, source)?;
+                        let permissions = source.metadata()?.permissions();
+                        #[cfg(unix)]
+                        let mode = permissions.mode();
+                        #[cfg(not(unix))]
+                        let mode = 0o644;
+                        writer.add_file_with_permissions(target, source, mode)?;
                     }
                 }
             }
         }
     }
 
     Ok(())
@@ -1243,23 +1250,32 @@
             debug!("Adding data from {}", subdir.path().display());
             (|| {
                 for file in WalkBuilder::new(subdir.path())
                     .standard_filters(false)
                     .build()
                 {
                     let file = file?;
+                    let permissions = file.metadata()?.permissions();
+                    #[cfg(unix)]
+                    let mode = permissions.mode();
+                    #[cfg(not(unix))]
+                    let mode = 0o644;
                     let relative = file.path().strip_prefix(data.parent().unwrap()).unwrap();
 
                     if file.path_is_symlink() {
                         // Copy the actual file contents, not the link, so that you can create a
                         // data directory by joining different data sources
                         let source = fs::read_link(file.path())?;
-                        writer.add_file(relative, source.parent().unwrap())?;
+                        writer.add_file_with_permissions(
+                            relative,
+                            source.parent().unwrap(),
+                            mode,
+                        )?;
                     } else if file.path().is_file() {
-                        writer.add_file(relative, file.path())?;
+                        writer.add_file_with_permissions(relative, file.path(), mode)?;
                     } else if file.path().is_dir() {
                         writer.add_directory(relative)?;
                     } else {
                         bail!("Can't handle data dir entry {}", file.path().display());
                     }
                 }
                 Ok(())
```

### Comparing `maturin-1.0.0b9/src/new_project.rs` & `maturin-1.0.1/src/new_project.rs`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/project_layout.rs` & `maturin-1.0.1/src/project_layout.rs`

 * *Files 3% similar despite different names*

```diff
@@ -85,16 +85,15 @@
         cargo_options.manifest_path = Some(manifest_file.clone());
 
         let cargo_toml = CargoToml::from_path(&manifest_file)?;
         cargo_toml.check_removed_python_metadata()?;
 
         let manifest_dir = manifest_file.parent().unwrap();
         let pyproject_toml: Option<PyProjectToml> = if pyproject_file.is_file() {
-            let pyproject =
-                PyProjectToml::new(&pyproject_file).context("pyproject.toml is invalid")?;
+            let pyproject = PyProjectToml::new(&pyproject_file)?;
             pyproject.warn_missing_maturin_version();
             pyproject.warn_missing_build_backend();
             Some(pyproject)
         } else {
             None
         };
         let pyproject = pyproject_toml.as_ref();
@@ -115,25 +114,28 @@
             metadata21.merge_pyproject_toml(pyproject_dir, pyproject)?;
         }
 
         let crate_name = &cargo_toml.package.name;
 
         // If the package name contains minuses, you must declare a module with
         // underscores as lib name
-        let module_name = cargo_toml
-            .lib
-            .as_ref()
-            .and_then(|lib| lib.name.as_ref())
+        // Precedence:
+        //  * Explicitly declared pyproject.toml `tool.maturin.module-name`
+        //  * Cargo.toml `lib.name`
+        //  * pyproject.toml `project.name`
+        //  * Cargo.toml `package.name`
+        let module_name = pyproject
+            .and_then(|x| x.module_name())
+            .or(cargo_toml.lib.as_ref().and_then(|lib| lib.name.as_deref()))
+            .or(pyproject
+                .and_then(|pyproject| pyproject.project.as_ref())
+                .map(|project| project.name.as_str()))
             .unwrap_or(crate_name)
             .to_owned();
 
-        let extension_name = pyproject
-            .and_then(|x| x.module_name())
-            .unwrap_or(&module_name);
-
         let project_root = if pyproject_file.is_file() {
             pyproject_file.parent().unwrap_or(manifest_dir)
         } else {
             manifest_dir
         };
         let python_packages = pyproject
             .and_then(|x| x.python_packages())
@@ -171,16 +173,23 @@
         let data = pyproject.and_then(|x| x.data()).map(|data| {
             if data.is_absolute() {
                 data.to_path_buf()
             } else {
                 project_root.join(data)
             }
         });
-        let project_layout =
-            ProjectLayout::determine(project_root, extension_name, py_root, python_packages, data)?;
+        let custom_python_source = pyproject.and_then(|x| x.python_source()).is_some();
+        let project_layout = ProjectLayout::determine(
+            project_root,
+            &module_name,
+            py_root,
+            python_packages,
+            data,
+            custom_python_source,
+        )?;
         Ok(Self {
             project_layout,
             cargo_toml_path: manifest_file,
             cargo_toml,
             pyproject_toml_path: pyproject_file,
             pyproject_toml,
             module_name,
@@ -230,16 +239,15 @@
             .into_path_buf();
         let pyproject_file = current_dir.join(PYPROJECT_TOML);
         if pyproject_file.is_file() {
             debug!(
                 "Found pyproject.toml in working directory at {:?}",
                 pyproject_file
             );
-            let pyproject =
-                PyProjectToml::new(&pyproject_file).context("pyproject.toml is invalid")?;
+            let pyproject = PyProjectToml::new(&pyproject_file)?;
             if let Some(path) = pyproject.manifest_path() {
                 debug!("Using cargo manifest path from pyproject.toml {:?}", path);
                 return Ok((
                     path.normalize()
                         .with_context(|| format!("failed to normalize path `{}`", path.display()))?
                         .into_path_buf(),
                     pyproject_file,
@@ -329,23 +337,23 @@
         Ok(cargo_metadata)
     }
 }
 
 impl ProjectLayout {
     /// Checks whether a python module exists besides Cargo.toml with the right name
     fn determine(
-        project_root: impl AsRef<Path>,
+        project_root: &Path,
         module_name: &str,
         python_root: PathBuf,
         python_packages: Vec<String>,
         data: Option<PathBuf>,
+        custom_python_source: bool,
     ) -> Result<ProjectLayout> {
         // A dot in the module name means the extension module goes into the module folder specified by the path
         let parts: Vec<&str> = module_name.split('.').collect();
-        let project_root = project_root.as_ref();
         let (python_module, rust_module, extension_name) = if parts.len() > 1 {
             let mut rust_module = python_root.clone();
             rust_module.extend(&parts[0..parts.len() - 1]);
             (
                 python_root.join(parts[0]),
                 rust_module,
                 parts[parts.len() - 1].to_string(),
@@ -359,14 +367,15 @@
         };
         debug!(
             project_root = %project_root.display(),
             python_dir = %python_root.display(),
             rust_module = %rust_module.display(),
             python_module = %python_module.display(),
             extension_name = %extension_name,
+            module_name = %module_name,
             "Project layout resolved"
         );
 
         let data = if let Some(data) = data {
             if !data.is_dir() {
                 bail!("No such data directory {}", data.display());
             }
@@ -391,14 +400,23 @@
                 python_packages,
                 python_module: Some(python_module),
                 rust_module,
                 extension_name,
                 data,
             })
         } else {
+            if custom_python_source {
+                eprintln!(
+                    "⚠️ Warning: You specified the python source as {}, but the python module at \
+                    {} is missing. No python module will be included.",
+                    python_root.display(),
+                    python_module.display()
+                );
+            }
+
             Ok(ProjectLayout {
                 python_dir: python_root,
                 python_packages,
                 python_module: None,
                 rust_module: project_root.to_path_buf(),
                 extension_name,
                 data,
```

### Comparing `maturin-1.0.0b9/src/pyproject_toml.rs` & `maturin-1.0.1/src/pyproject_toml.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 //! A pyproject.toml as specified in PEP 517
 
 use crate::PlatformTag;
-use anyhow::{format_err, Result};
+use anyhow::{Context, Result};
 use fs_err as fs;
-use pyproject_toml::PyProjectToml as ProjectToml;
+use pyproject_toml::{BuildSystem, Project};
 use serde::{Deserialize, Serialize};
 use std::collections::HashMap;
 use std::path::{Path, PathBuf};
 
 /// The `[tool]` section of a pyproject.toml
 #[derive(Serialize, Deserialize, Debug, Clone, Default)]
 #[serde(rename_all = "kebab-case")]
@@ -175,42 +175,40 @@
     pub rustc_args: Option<Vec<String>>,
 }
 
 /// A pyproject.toml as specified in PEP 517
 #[derive(Serialize, Deserialize, Debug, Clone)]
 #[serde(rename_all = "kebab-case")]
 pub struct PyProjectToml {
-    #[serde(flatten)]
-    inner: ProjectToml,
+    /// Build-related data
+    pub build_system: BuildSystem,
+    /// Project metadata
+    pub project: Option<Project>,
     /// PEP 518: The `[tool]` table is where any tool related to your Python project, not just build
     /// tools, can have users specify configuration data as long as they use a sub-table within
     /// `[tool]`, e.g. the flit tool would store its configuration in `[tool.flit]`.
     ///
     /// We use it for `[tool.maturin]`
     pub tool: Option<Tool>,
 }
 
-impl std::ops::Deref for PyProjectToml {
-    type Target = ProjectToml;
-
-    fn deref(&self) -> &Self::Target {
-        &self.inner
-    }
-}
-
 impl PyProjectToml {
     /// Returns the contents of a pyproject.toml with a `[build-system]` entry or an error
     ///
     /// Does no specific error handling because it's only used to check whether or not to build
     /// source distributions
     pub fn new(pyproject_file: impl AsRef<Path>) -> Result<PyProjectToml> {
         let path = pyproject_file.as_ref();
         let contents = fs::read_to_string(path)?;
-        let pyproject: PyProjectToml = toml::from_str(&contents)
-            .map_err(|err| format_err!("pyproject.toml is not PEP 517 compliant: {}", err))?;
+        let pyproject = toml::from_str(&contents).with_context(|| {
+            format!(
+                "pyproject.toml at {} is invalid",
+                pyproject_file.as_ref().display()
+            )
+        })?;
         Ok(pyproject)
     }
 
     /// Returns the value of `[project.name]` in pyproject.toml
     pub fn project_name(&self) -> Option<&str> {
         self.project.as_ref().map(|project| project.name.as_str())
     }
@@ -349,14 +347,15 @@
 #[cfg(test)]
 mod tests {
     use crate::{
         pyproject_toml::{Format, Formats, GlobPattern, ToolMaturin},
         PyProjectToml,
     };
     use fs_err as fs;
+    use indoc::indoc;
     use pretty_assertions::assert_eq;
     use std::path::Path;
     use tempfile::TempDir;
 
     #[test]
     fn test_parse_tool_maturin() {
         let tmp_dir = TempDir::new().unwrap();
@@ -491,8 +490,47 @@
                 GlobPattern::WithFormat {
                     path: "three".to_string(),
                     format: Formats::Multiple(vec![Format::Sdist, Format::Wheel])
                 }
             ])
         );
     }
+
+    #[test]
+    fn test_gh_1615() {
+        let source = indoc!(
+            r#"[build-system]
+            requires = [ "maturin>=0.14", "numpy", "wheel", "patchelf",]
+            build-backend = "maturin"
+            
+            [project]
+            name = "..."
+            license-files = [ "license.txt",]
+            requires-python = ">=3.8"
+            requires-dist = [ "maturin>=0.14", "...",]
+            dependencies = [ "packaging", "...",]
+            zip-safe = false
+            version = "..."
+            readme = "..."
+            description = "..."
+            classifiers = [ "...",]
+        "#
+        );
+        let temp_dir = TempDir::new().unwrap();
+        let pyproject_toml = temp_dir.path().join("pyproject.toml");
+        fs::write(&pyproject_toml, source).unwrap();
+        let outer_error = PyProjectToml::new(&pyproject_toml).unwrap_err();
+        let inner_error = outer_error.source().unwrap();
+
+        assert_eq!(
+            inner_error.to_string(),
+            indoc!(
+                r#"TOML parse error at line 7, column 17
+                  |
+                7 | license-files = [ "license.txt",]
+                  |                 ^^^^^^^^^^^^^^^^^
+                wanted string or table
+                "#
+            )
+        );
+    }
 }
```

### Comparing `maturin-1.0.0b9/src/python_interpreter/get_interpreter_metadata.py` & `maturin-1.0.1/src/python_interpreter/get_interpreter_metadata.py`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/python_interpreter/mod.rs` & `maturin-1.0.1/src/python_interpreter/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 mod config;
 
 /// This snippets will give us information about the python interpreter's
 /// version and abi as json through stdout
 const GET_INTERPRETER_METADATA: &str = include_str!("get_interpreter_metadata.py");
 pub const MINIMUM_PYTHON_MINOR: usize = 7;
 /// Be liberal here to include preview versions
-const MAXIMUM_PYTHON_MINOR: usize = 12;
-const MAXIMUM_PYPY_MINOR: usize = 10;
+pub const MAXIMUM_PYTHON_MINOR: usize = 12;
+pub const MAXIMUM_PYPY_MINOR: usize = 10;
 
 /// Identifies conditions where we do not want to build wheels
 fn windows_interpreter_no_build(
     major: usize,
     minor: usize,
     target_width: usize,
     pointer_width: usize,
@@ -360,15 +360,15 @@
     pub platform: Option<String>,
     /// Is this interpreter runnable
     ///
     /// When cross compile the target interpreter isn't runnable,
     /// and it's `executable` is empty
     pub runnable: bool,
     /// Comes from `sys.platform.name`
-    pub implmentation_name: String,
+    pub implementation_name: String,
     /// Comes from sysconfig var `SOABI`
     pub soabi: Option<String>,
 }
 
 impl Deref for PythonInterpreter {
     type Target = InterpreterConfig;
 
@@ -429,15 +429,15 @@
         bail!("A python 3 interpreter on linux or mac os must define abiflags in its sysconfig ಠ_ಠ")
     }
 }
 
 impl PythonInterpreter {
     /// Does this interpreter have PEP 384 stable api aka. abi3 support?
     pub fn has_stable_api(&self) -> bool {
-        if self.implmentation_name.parse::<InterpreterKind>().is_err() {
+        if self.implementation_name.parse::<InterpreterKind>().is_err() {
             false
         } else {
             match self.interpreter_kind {
                 InterpreterKind::CPython => true,
                 InterpreterKind::PyPy => false,
             }
         }
@@ -461,20 +461,20 @@
                 platform
             } else {
                 context.get_platform_tag(platform_tags)?
             }
         } else {
             context.get_platform_tag(platform_tags)?
         };
-        let tag = if self.implmentation_name.parse::<InterpreterKind>().is_err() {
+        let tag = if self.implementation_name.parse::<InterpreterKind>().is_err() {
             // Use generic tags when `sys.implementation.name` != `platform.python_implementation()`, for example Pyston
             // See also https://github.com/pypa/packaging/blob/0031046f7fad649580bc3127d1cef9157da0dd79/packaging/tags.py#L234-L261
             format!(
                 "{interpreter}{major}{minor}-{soabi}-{platform}",
-                interpreter = self.implmentation_name,
+                interpreter = self.implementation_name,
                 major = self.major,
                 minor = self.minor,
                 soabi = self
                     .soabi
                     .as_deref()
                     .unwrap_or("none")
                     .replace(['-', '.'], "_"),
@@ -672,43 +672,43 @@
                     .context("syconfig didn't define an `EXT_SUFFIX` ಠ_ಠ")?,
                 abi_tag: message.abi_tag,
                 pointer_width: None,
             },
             executable,
             platform,
             runnable: true,
-            implmentation_name: message.implementation_name,
+            implementation_name: message.implementation_name,
             soabi: message.soabi,
         }))
     }
 
     /// Construct a `PythonInterpreter` from a sysconfig and target
     pub fn from_config(config: InterpreterConfig) -> Self {
-        let implmentation_name = config.interpreter_kind.to_string().to_ascii_lowercase();
+        let implementation_name = config.interpreter_kind.to_string().to_ascii_lowercase();
         PythonInterpreter {
             config,
             executable: PathBuf::new(),
             platform: None,
             runnable: false,
-            implmentation_name,
+            implementation_name,
             soabi: None,
         }
     }
 
     /// Find all available python interpreters for a given target
     pub fn find_by_target(
         target: &Target,
         requires_python: Option<&VersionSpecifiers>,
     ) -> Vec<PythonInterpreter> {
         InterpreterConfig::lookup_target(target)
             .into_iter()
             .filter_map(|config| match requires_python {
                 Some(requires_python) => {
                     if requires_python
-                        .contains(&Version::from_release(vec![config.major, config.major]))
+                        .contains(&Version::from_release(vec![config.major, config.minor]))
                     {
                         Some(Self::from_config(config))
                     } else {
                         None
                     }
                 }
                 None => Some(Self::from_config(config)),
@@ -875,15 +875,15 @@
 
     /// An opaque string that uniquely identifies this Python interpreter.
     /// Used to trigger rebuilds for `pyo3` when the Python interpreter changes.
     pub fn environment_signature(&self) -> String {
         let pointer_width = self.pointer_width.unwrap_or(64);
         format!(
             "{}-{}.{}-{}bit",
-            self.implmentation_name, self.major, self.minor, pointer_width
+            self.implementation_name, self.major, self.minor, pointer_width
         )
     }
 
     /// Returns the site-packages directory inside a venv e.g.
     /// {venv_base}/lib/python{x}.{y} on unix or {venv_base}/Lib on window
     pub fn get_venv_site_package(&self, venv_base: impl AsRef<Path>, target: &Target) -> PathBuf {
         if target.is_unix() {
@@ -924,7 +924,32 @@
                 self.config.major,
                 self.config.minor,
                 self.config.abiflags,
             )
         }
     }
 }
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn test_find_interpreter_by_target() {
+        let target =
+            Target::from_target_triple(Some("x86_64-unknown-linux-gnu".to_string())).unwrap();
+        let pythons = PythonInterpreter::find_by_target(&target, None);
+        assert_eq!(pythons.len(), 10);
+
+        let pythons = PythonInterpreter::find_by_target(
+            &target,
+            Some(&VersionSpecifiers::from_str(">=3.7").unwrap()),
+        );
+        assert_eq!(pythons.len(), 10);
+
+        let pythons = PythonInterpreter::find_by_target(
+            &target,
+            Some(&VersionSpecifiers::from_str(">=3.10").unwrap()),
+        );
+        assert_eq!(pythons.len(), 4);
+    }
+}
```

### Comparing `maturin-1.0.0b9/src/source_distribution.rs` & `maturin-1.0.1/src/source_distribution.rs`

 * *Files 2% similar despite different names*

```diff
@@ -185,37 +185,45 @@
     let mut rewritten = false;
     //  ˇˇˇˇˇˇˇˇˇˇˇˇ dep_category
     // [dependencies]
     // some_path_dep = { path = "../some_path_dep" }
     //                          ^^^^^^^^^^^^^^^^^^ table[&dep_name]["path"]
     // ^^^^^^^^^^^^^ dep_name
     for dep_category in ["dependencies", "dev-dependencies", "build-dependencies"] {
-        if let Some(table) = table.get_mut(dep_category).and_then(|x| x.as_table_mut()) {
+        if let Some(dep_table) = table.get_mut(dep_category).and_then(|x| x.as_table_mut()) {
             if dep_category == "dev-dependencies" && !known_path_deps.is_empty() {
                 // Remove dev-dependencies since building from sdist doesn't need them,
                 // Keep it when there are no path dependencies to support building from
                 // sdist with `--locked`/`--frozen`.
-                table.remove(dep_category);
+                table.remove(dep_category).unwrap();
+                debug!(
+                    "Removing `dev-dependencies` from {} all together since there are no path dependencies",
+                    manifest_path.display(),
+                );
                 rewritten = true;
                 continue;
             }
-            let dep_names: Vec<_> = table.iter().map(|(key, _)| key.to_string()).collect();
+            let dep_names: Vec<_> = dep_table.iter().map(|(key, _)| key.to_string()).collect();
             for dep_name in dep_names {
-                let workspace_inherit = table
+                let workspace_inherit = dep_table
                     .get(&dep_name)
                     .and_then(|x| x.get("workspace"))
                     .and_then(|x| x.as_bool())
                     .unwrap_or_default();
 
                 if !workspace_inherit {
                     // There should either be no value for path, or it should be a string
-                    if table.get(&dep_name).and_then(|x| x.get("path")).is_none() {
+                    if dep_table
+                        .get(&dep_name)
+                        .and_then(|x| x.get("path"))
+                        .is_none()
+                    {
                         continue;
                     }
-                    if !table[&dep_name]["path"].is_str() {
+                    if !dep_table[&dep_name]["path"].is_str() {
                         bail!(
                             "In {}, {} {} has a path value that is not a string",
                             manifest_path.display(),
                             dep_category,
                             dep_name
                         )
                     }
@@ -231,20 +239,22 @@
                 } else {
                     // If a workspace inherited dependency isn't a path dep,
                     // we need to replace `workspace = true` with its full requirement spec.
                     if !known_path_deps.contains_key(&dep_name) {
                         if let Some(workspace_dep) = workspace_deps.and_then(|x| x.get(&dep_name)) {
                             let mut workspace_dep = workspace_dep.clone();
                             // Merge optional and features from the current Cargo.toml
-                            if table[&dep_name].get("optional").is_some() {
+                            if dep_table[&dep_name].get("optional").is_some() {
                                 ensure_dep_is_inline_table(&mut workspace_dep);
-                                workspace_dep["optional"] = table[&dep_name]["optional"].clone();
+                                workspace_dep["optional"] =
+                                    dep_table[&dep_name]["optional"].clone();
                             }
-                            if let Some(features) =
-                                table[&dep_name].get("features").and_then(|x| x.as_array())
+                            if let Some(features) = dep_table[&dep_name]
+                                .get("features")
+                                .and_then(|x| x.as_array())
                             {
                                 ensure_dep_is_inline_table(&mut workspace_dep);
                                 let existing_features = workspace_dep
                                     .as_table_like_mut()
                                     .unwrap()
                                     .entry("features")
                                     .or_insert_with(|| {
@@ -257,38 +267,38 @@
                                         manifest_path.display(),
                                         dep_category,
                                         dep_name
                                     )
                                     })?;
                                 existing_features.extend(features);
                             }
-                            table[&dep_name] = workspace_dep;
+                            dep_table[&dep_name] = workspace_dep;
                             rewritten = true;
                         } else {
                             bail!(
                             "In {}, {} {} is marked as `workspace = true`, but it is found neither in \
                                 the workspace manifest nor in the known path dependencies",
                             manifest_path.display(),
                             dep_category,
                             dep_name
                         )
                         }
                         continue;
                     }
                 }
                 // This is the location of the targeted crate in the source distribution
-                table[&dep_name]["path"] = if root_crate {
+                dep_table[&dep_name]["path"] = if root_crate {
                     toml_edit::value(format!("{local_deps_folder}/{dep_name}"))
                 } else {
                     // Cargo.toml contains relative paths, and we're already in LOCAL_DEPENDENCIES_FOLDER
                     toml_edit::value(format!("../{dep_name}"))
                 };
                 if workspace_inherit {
                     // Remove workspace inheritance now that we converted it into a path dependency
-                    table[&dep_name]
+                    dep_table[&dep_name]
                         .as_table_like_mut()
                         .unwrap()
                         .remove("workspace");
                 }
                 rewritten = true;
             }
         }
```

### Comparing `maturin-1.0.0b9/src/target.rs` & `maturin-1.0.1/src/target.rs`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
     }
 
     /// Returns the platform architecture
     pub fn get_platform_arch(&self) -> Result<String> {
         if self.cross_compiling {
             return Ok(self.arch.to_string());
         }
-        let machine = PlatformInfo::new().map(|info| info.machine().into_owned());
+        let machine = PlatformInfo::new().map(|info| info.machine().to_string_lossy().into_owned());
         let arch = match machine {
             Ok(machine) => {
                 let linux32 = (machine == "x86_64" && self.arch != Arch::X86_64)
                     || (machine == "aarch64" && self.arch != Arch::Aarch64);
                 if linux32 {
                     // When running in Docker sometimes uname returns 64-bit architecture while the container is actually 32-bit,
                     // In this case we trust the architecture of rustc target
@@ -292,16 +292,17 @@
     /// Returns the platform release
     pub fn get_platform_release(&self) -> Result<String> {
         let os = self.os.to_string();
         let os_version = env::var(format!("MATURIN_{}_VERSION", os.to_ascii_uppercase()));
         let release = match os_version {
             Ok(os_ver) => os_ver,
             Err(_) => {
-                let info = PlatformInfo::new()?;
-                info.release().to_string()
+                let info = PlatformInfo::new()
+                    .map_err(|e| anyhow!("Failed to fetch platform information: {e}"))?;
+                info.release().to_string_lossy().into_owned()
             }
         };
         let release = release.replace(['.', '-'], "_");
         Ok(release)
     }
 
     /// Returns the name python uses in `sys.platform` for this architecture.
```

### Comparing `maturin-1.0.0b9/src/templates/.gitignore.j2` & `maturin-1.0.1/src/templates/.gitignore.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/templates/Cargo.toml.j2` & `maturin-1.0.1/src/templates/Cargo.toml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [lib]
 name = "{{ crate_name }}"
 crate-type = ["cdylib"]
 {%- endif %}
 
 [dependencies]
 {% if bindings == "pyo3" -%}
-pyo3 = "0.18.1"
+pyo3 = "0.18.3"
 {% elif bindings == "rust-cpython" -%}
 cpython = "0.7.1"
 {% elif bindings == "uniffi" -%}
 uniffi = "0.23.0"
 
 [build-dependencies]
 uniffi = { version = "0.23.0", features = ["build"] }
```

### Comparing `maturin-1.0.0b9/src/templates/lib.rs.j2` & `maturin-1.0.1/src/templates/lib.rs.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/templates/pyproject.toml.j2` & `maturin-1.0.1/src/templates/pyproject.toml.j2`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/src/upload.rs` & `maturin-1.0.1/src/upload.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 //! The uploading logic was mostly reverse engineered; I wrote it down as
 //! documentation at https://warehouse.readthedocs.io/api-reference/legacy/#upload-api
 
 use crate::build_context::hash_file;
 use anyhow::{bail, Context, Result};
+use base64::engine::general_purpose::STANDARD;
+use base64::Engine;
 use bytesize::ByteSize;
 use configparser::ini::Ini;
 use fs_err as fs;
 use fs_err::File;
 use multipart::client::lazy::Multipart;
 use regex::Regex;
 use serde::Deserialize;
@@ -486,15 +488,15 @@
     let mut form = Multipart::new();
     for (key, value) in api_metadata {
         form.add_text(key, value);
     }
 
     form.add_stream("content", &wheel, Some(wheel_name), None);
     let multipart_data = form.prepare().map_err(|e| e.error)?;
-    let encoded = base64::encode(format!("{}:{}", registry.username, registry.password));
+    let encoded = STANDARD.encode(format!("{}:{}", registry.username, registry.password));
 
     let agent = http_agent()?;
 
     let response = agent
         .post(registry.url.as_str())
         .set(
             "Content-Type",
```

### Comparing `maturin-1.0.0b9/test-dockerfile.sh` & `maturin-1.0.1/test-dockerfile.sh`

 * *Files identical despite different names*

### Comparing `maturin-1.0.0b9/PKG-INFO` & `maturin-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maturin
-Version: 1.0.0b9
+Version: 1.0.1
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: tomli >=1.1.0 ; python_version < '3.11'
 Requires-Dist: ziglang ~=0.10.0 ; extra == 'zig'
 Requires-Dist: patchelf ; extra == 'patchelf'
@@ -25,15 +25,14 @@
 
 # Maturin
 
 _formerly pyo3-pack_
 
 [![Actions Status](https://img.shields.io/github/actions/workflow/status/PyO3/maturin/test.yml?branch=main&logo=github&style=flat-square)](https://github.com/PyO3/maturin/actions)
 [![FreeBSD](https://img.shields.io/cirrus/github/PyO3/maturin/main?logo=CircleCI&style=flat-square)](https://cirrus-ci.com/github/PyO3/maturin)
-[![Bors enabled](https://bors.tech/images/badge_small.svg)](https://app.bors.tech/repositories/55651)
 [![Crates.io](https://img.shields.io/crates/v/maturin.svg?logo=rust&style=flat-square)](https://crates.io/crates/maturin)
 [![PyPI](https://img.shields.io/pypi/v/maturin.svg?logo=python&style=flat-square)](https://pypi.org/project/maturin)
 [![Maturin User Guide](https://img.shields.io/badge/user-guide-brightgreen?logo=readthedocs&style=flat-square)](https://maturin.rs)
 [![Chat on Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg?logo=gitter&style=flat-square)](https://gitter.im/PyO3/Lobby)
 
 Build and publish crates with pyo3, rust-cpython, cffi and uniffi bindings as well as rust binaries as python packages.
 
@@ -142,14 +141,15 @@
 You can specify a different python source directory in `pyproject.toml` by setting `tool.maturin.python-source`, for example
 
 **pyproject.toml**
 
 ```toml
 [tool.maturin]
 python-source = "python"
+module-name = "my_project._lib_name"
 ```
 
 then the project structure would look like this:
 
 ```
 my-project
 ├── Cargo.toml
@@ -175,20 +175,32 @@
 
 ```
 my-project
 ├── Cargo.toml
 ├── my_project
 │   ├── __init__.py
 │   ├── bar.py
-│   └── my_project.cpython-36m-x86_64-linux-gnu.so
+│   └── _lib_name.cpython-36m-x86_64-linux-gnu.so
 ├── README.md
 └── src
     └── lib.rs
 ```
 
+When doing this also be sure to set the module name in your code to match the last part of `module-name` (don't include the package path):
+
+```
+#[pymodule]
+#[pyo3(name="_lib_name")]
+fn my_lib_name(_py: Python<'_>, m: &PyModule) -> PyResult<()> {
+    m.add_class::<MyPythonRustClass>()?;
+    Ok(())
+}
+```
+
+
 ## Python metadata
 
 maturin supports [PEP 621](https://www.python.org/dev/peps/pep-0621/), you can specify python package metadata in `pyproject.toml`.
 maturin merges metadata from `Cargo.toml` and `pyproject.toml`, `pyproject.toml` take precedence over `Cargo.toml`.
 
 To specify python dependencies, add a list `dependencies` in a `[project]` section in the `pyproject.toml`. This list is equivalent to `install_requires` in setuptools:
 
@@ -216,15 +228,15 @@
 
 ## Source distribution
 
 maturin supports building through `pyproject.toml`. To use it, create a `pyproject.toml` next to your `Cargo.toml` with the following content:
 
 ```toml
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 ```
 
 If a `pyproject.toml` with a `[build-system]` entry is present, maturin can build a source distribution of your package when `--sdist` is specified.
 The source distribution will contain the same files as `cargo package`. To only build a source distribution, pass `--interpreter` without any values.
 
 You can then e.g. install your package with `pip install .`. With `pip install . -v` you can see the output of cargo and maturin.
@@ -232,15 +244,15 @@
 You can use the options `compatibility`, `skip-auditwheel`, `bindings`, `strip` and common Cargo build options such as `features` under `[tool.maturin]` the same way you would when running maturin directly.
 The `bindings` key is required for cffi and bin projects as those can't be automatically detected. Currently, all builds are in release mode (see [this thread](https://discuss.python.org/t/pep-517-debug-vs-release-builds/1924) for details).
 
 For a non-manylinux build with cffi bindings you could use the following:
 
 ```toml
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [tool.maturin]
 bindings = "cffi"
 compatibility = "linux"
 ```
```

