# Comparing `tmp/SymSpellCppPy-0.0.8.tar.gz` & `tmp/SymSpellCppPy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/SymSpellCppPy-0.0.8.tar", last modified: Wed Sep 30 07:46:04 2020, max compression
+gzip compressed data, was "dist/SymSpellCppPy-0.0.9.tar", last modified: Thu Oct  1 17:26:55 2020, max compression
```

## Comparing `SymSpellCppPy-0.0.8.tar` & `SymSpellCppPy-0.0.9.tar`

### file list

```diff
@@ -1,127 +1,135 @@
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.165047 SymSpellCppPy-0.0.8/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1574 2020-09-29 18:01:05.000000 SymSpellCppPy-0.0.8/CMakeLists.txt
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      468 2020-09-28 18:52:54.000000 SymSpellCppPy-0.0.8/MANIFEST.in
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3123 2020-09-30 07:46:04.165047 SymSpellCppPy-0.0.8/PKG-INFO
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1723 2020-09-30 07:24:55.000000 SymSpellCppPy-0.0.8/README.md
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    11672 2020-09-30 05:11:26.000000 SymSpellCppPy-0.0.8/SymSpellCppPy.cpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3123 2020-09-30 07:46:04.000000 SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/PKG-INFO
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4178 2020-09-30 07:46:04.000000 SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/SOURCES.txt
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)        1 2020-09-30 07:46:04.000000 SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/dependency_links.txt
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)        1 2020-09-30 07:46:04.000000 SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/not-zip-safe
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       14 2020-09-30 07:46:04.000000 SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/top_level.txt
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/include/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      284 2020-09-27 05:42:39.000000 SymSpellCppPy-0.0.8/include/BaseDistance.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      291 2020-09-27 05:44:34.000000 SymSpellCppPy-0.0.8/include/BaseSimilarity.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     8832 2020-09-27 06:10:11.000000 SymSpellCppPy-0.0.8/include/DamerauOSA.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      849 2020-09-27 05:44:12.000000 SymSpellCppPy-0.0.8/include/Defines.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1058 2020-09-27 06:10:43.000000 SymSpellCppPy-0.0.8/include/EditDistance.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7144 2020-09-29 14:58:43.000000 SymSpellCppPy-0.0.8/include/Helpers.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10025 2020-09-27 05:48:44.000000 SymSpellCppPy-0.0.8/include/Levenshtein.h
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/include/cereal/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    14820 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/access.hpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/include/cereal/archives/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6034 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/archives/adapters.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6760 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/archives/binary.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    43681 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/archives/json.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    14780 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/archives/portable_binary.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    39071 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/archives/xml.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    45263 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/cereal.hpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/include/cereal/details/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15930 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/details/helpers.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    37111 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/details/polymorphic_impl.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2902 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/details/polymorphic_impl_fwd.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4918 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/details/static_object.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    96668 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/details/traits.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2931 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/details/util.hpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/include/cereal/external/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4446 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/base64.hpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.161047 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10815 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/allocators.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2365 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/cursorstreamwrapper.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   119446 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/document.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10989 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/encodedstream.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    30191 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/encodings.h
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.161047 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/error/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4080 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/error/en.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6374 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/error/error.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3113 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/filereadstream.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3244 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/filewritestream.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4070 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/fwd.h
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.161047 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     9218 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/biginteger.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    12730 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/diyfp.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     8195 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/dtoa.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3064 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/ieee754.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10194 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/itoa.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6879 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/meta.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3637 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/pow10.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    26328 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/regex.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7345 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/stack.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2255 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/strfunc.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     9155 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/strtod.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1482 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/swap.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4187 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/istreamwrapper.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2595 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/memorybuffer.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2772 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/memorystream.h
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.161047 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/msinttypes/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     8372 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/msinttypes/inttypes.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     9386 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/msinttypes/stdint.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2422 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/ostreamwrapper.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    61159 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/pointer.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10703 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/prettywriter.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    25306 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/rapidjson.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    95072 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/reader.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   105031 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/schema.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6851 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/stream.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4063 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/stringbuffer.h
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    27313 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/writer.h
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.161047 SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2804 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/license.txt
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   119560 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3862 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml_iterators.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15689 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml_print.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3324 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml_utils.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6552 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/macros.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6596 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/specialize.hpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.165047 SymSpellCppPy-0.0.8/include/cereal/types/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3501 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/array.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2309 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/atomic.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7553 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/base_class.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5455 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/bitset.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5545 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/boost_variant.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2899 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/chrono.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5376 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/common.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2375 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/complex.hpp
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.165047 SymSpellCppPy-0.0.8/include/cereal/types/concepts/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3210 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/concepts/pair_associative_container.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2448 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/deque.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2886 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/forward_list.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1975 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/functional.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2432 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/list.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1833 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/map.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    16846 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/memory.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2555 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/optional.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    22311 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/polymorphic.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4761 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/queue.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3548 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/set.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2880 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/stack.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2935 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/string.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4633 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/tuple.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1893 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/unordered_map.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3718 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/unordered_set.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2127 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/utility.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3942 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/valarray.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4185 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/variant.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4845 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/types/vector.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2342 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.8/include/cereal/version.hpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    30767 2020-09-29 18:23:05.000000 SymSpellCppPy-0.0.8/library.cpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15565 2020-09-30 02:08:41.000000 SymSpellCppPy-0.0.8/library.h
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.165047 SymSpellCppPy-0.0.8/resources/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)  1332147 2020-09-25 17:57:16.000000 SymSpellCppPy-0.0.8/resources/frequency_dictionary_en_82_765.txt
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       19 2020-09-27 14:10:53.000000 SymSpellCppPy-0.0.8/resources/frequency_dictionary_en_test_verbosity.txt
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       38 2020-09-30 07:46:04.165047 SymSpellCppPy-0.0.8/setup.cfg
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4182 2020-09-30 07:45:19.000000 SymSpellCppPy-0.0.8/setup.py
-drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-09-30 07:46:04.157047 SymSpellCppPy-0.0.8/tests/
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5920 2020-09-30 02:13:01.000000 SymSpellCppPy-0.0.8/tests/CatchMain.cpp
--rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3484 2020-09-30 02:25:15.000000 SymSpellCppPy-0.0.8/tests/SymSpellCppPyTest.py
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.913213 SymSpellCppPy-0.0.9/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1508 2020-10-01 16:50:08.000000 SymSpellCppPy-0.0.9/CMakeLists.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      468 2020-09-28 18:52:54.000000 SymSpellCppPy-0.0.9/MANIFEST.in
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3206 2020-10-01 17:26:55.913213 SymSpellCppPy-0.0.9/PKG-INFO
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1798 2020-10-01 16:48:11.000000 SymSpellCppPy-0.0.9/README.md
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    12331 2020-10-01 15:30:45.000000 SymSpellCppPy-0.0.9/SymSpellCppPy.cpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.873213 SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3206 2020-10-01 17:26:55.000000 SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/PKG-INFO
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4423 2020-10-01 17:26:55.000000 SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/SOURCES.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)        1 2020-10-01 17:26:55.000000 SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/dependency_links.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)        1 2020-10-01 17:26:55.000000 SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/not-zip-safe
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       14 2020-10-01 17:26:55.000000 SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/top_level.txt
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.873213 SymSpellCppPy-0.0.9/include/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      284 2020-09-27 05:42:39.000000 SymSpellCppPy-0.0.9/include/BaseDistance.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      291 2020-09-27 05:44:34.000000 SymSpellCppPy-0.0.9/include/BaseSimilarity.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     8832 2020-10-01 10:02:34.000000 SymSpellCppPy-0.0.9/include/DamerauOSA.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)      849 2020-09-27 05:44:12.000000 SymSpellCppPy-0.0.9/include/Defines.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1061 2020-10-01 10:02:22.000000 SymSpellCppPy-0.0.9/include/EditDistance.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7190 2020-10-01 15:08:58.000000 SymSpellCppPy-0.0.9/include/Helpers.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10025 2020-10-01 10:01:26.000000 SymSpellCppPy-0.0.9/include/Levenshtein.h
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.873213 SymSpellCppPy-0.0.9/include/cereal/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    14820 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/access.hpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.873213 SymSpellCppPy-0.0.9/include/cereal/archives/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6034 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/archives/adapters.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6760 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/archives/binary.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    43681 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/archives/json.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    14780 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/archives/portable_binary.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    39071 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/archives/xml.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    45263 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/cereal.hpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.877213 SymSpellCppPy-0.0.9/include/cereal/details/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15930 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/details/helpers.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    37111 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/details/polymorphic_impl.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2902 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/details/polymorphic_impl_fwd.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4918 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/details/static_object.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    96668 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/details/traits.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2931 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/details/util.hpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.877213 SymSpellCppPy-0.0.9/include/cereal/external/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4446 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/base64.hpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.881213 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10815 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/allocators.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2365 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/cursorstreamwrapper.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   119446 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/document.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10989 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/encodedstream.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    30191 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/encodings.h
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.881213 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/error/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4080 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/error/en.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6374 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/error/error.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3113 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/filereadstream.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3244 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/filewritestream.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4070 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/fwd.h
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.889213 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     9218 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/biginteger.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    12730 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/diyfp.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     8195 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/dtoa.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3064 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/ieee754.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10194 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/itoa.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6879 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/meta.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3637 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/pow10.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    26328 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/regex.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7345 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/stack.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2255 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/strfunc.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     9155 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/strtod.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1482 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/swap.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4187 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/istreamwrapper.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2595 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/memorybuffer.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2772 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/memorystream.h
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.889213 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/msinttypes/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     8372 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/msinttypes/inttypes.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     9386 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/msinttypes/stdint.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2422 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/ostreamwrapper.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    61159 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/pointer.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    10703 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/prettywriter.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    25306 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/rapidjson.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    95072 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/reader.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   105031 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/schema.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6851 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/stream.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4063 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/stringbuffer.h
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    27313 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/writer.h
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.893213 SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2804 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/license.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   119560 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3862 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml_iterators.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15689 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml_print.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3324 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml_utils.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6552 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/macros.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     6596 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/specialize.hpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.901213 SymSpellCppPy-0.0.9/include/cereal/types/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3501 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/array.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2309 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/atomic.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7553 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/base_class.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5455 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/bitset.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5545 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/boost_variant.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2899 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/chrono.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     5376 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/common.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2375 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/complex.hpp
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.901213 SymSpellCppPy-0.0.9/include/cereal/types/concepts/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3210 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/concepts/pair_associative_container.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2448 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/deque.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2886 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/forward_list.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1975 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/functional.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2432 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/list.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1833 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/map.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    16846 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/memory.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2555 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/optional.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    22311 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/polymorphic.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4761 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/queue.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3548 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/set.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2880 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/stack.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2935 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/string.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4633 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/tuple.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     1893 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/unordered_map.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3718 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/unordered_set.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2127 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/utility.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     3942 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/valarray.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4185 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/variant.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4845 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/types/vector.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     2342 2020-09-29 17:47:13.000000 SymSpellCppPy-0.0.9/include/cereal/version.hpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    33516 2020-10-01 16:42:12.000000 SymSpellCppPy-0.0.9/library.cpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15607 2020-10-01 15:16:00.000000 SymSpellCppPy-0.0.9/library.h
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.905213 SymSpellCppPy-0.0.9/resources/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)  5137213 2020-10-01 08:14:28.000000 SymSpellCppPy-0.0.9/resources/frequency_bigramdictionary_en_243_342.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)  1332144 2020-09-30 16:42:32.000000 SymSpellCppPy-0.0.9/resources/frequency_dictionary_en_82_765.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       19 2020-09-27 14:10:53.000000 SymSpellCppPy-0.0.9/resources/frequency_dictionary_en_test_verbosity.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       38 2020-10-01 17:26:55.913213 SymSpellCppPy-0.0.9/setup.cfg
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     4076 2020-10-01 16:49:21.000000 SymSpellCppPy-0.0.9/setup.py
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.873213 SymSpellCppPy-0.0.9/tests/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)     7042 2020-10-01 10:53:35.000000 SymSpellCppPy-0.0.9/tests/CatchMain.cpp
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    30493 2020-10-01 16:47:22.000000 SymSpellCppPy-0.0.9/tests/SymSpellCppPyTest.py
+drwxrwxr-x   0 vigi99    (1000) vigi99    (1000)        0 2020-10-01 17:26:55.913213 SymSpellCppPy-0.0.9/tests/fortests/
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       56 2020-10-01 05:38:45.000000 SymSpellCppPy-0.0.9/tests/fortests/bad_dict.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)  6488675 2020-10-01 05:38:45.000000 SymSpellCppPy-0.0.9/tests/fortests/big_modified.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)   342633 2020-10-01 05:38:45.000000 SymSpellCppPy-0.0.9/tests/fortests/big_words.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)    15935 2020-10-01 05:38:45.000000 SymSpellCppPy-0.0.9/tests/fortests/noisy_query_en_1000.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       19 2020-10-01 05:38:45.000000 SymSpellCppPy-0.0.9/tests/fortests/non_en_dict.txt
+-rw-rw-r--   0 vigi99    (1000) vigi99    (1000)       82 2020-10-01 05:38:45.000000 SymSpellCppPy-0.0.9/tests/fortests/separator_dict.txt
```

### Comparing `SymSpellCppPy-0.0.8/CMakeLists.txt` & `SymSpellCppPy-0.0.9/CMakeLists.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 
 set(CMAKE_CXX_STANDARD 14)
 set(CMAKE_CXX_STANDARD_REQUIRED ON)
 set(CMAKE_CXX_EXTENSIONS ON)
 set(CMAKE_BUILD_TYPE "Release")
 
 option(BUILD_FOR_PYTHON "Build for Python" OFF)
+option(BUILD_FOR_TEST "Build Tests" ON)
 
 add_library(SymSpellCpp SHARED library.cpp library.h)
 target_include_directories(SymSpellCpp PUBLIC ${CMAKE_SOURCE_DIR}/include)
 
 if (BUILD_FOR_PYTHON)
+    set(CMAKE_BUILD_TYPE "Release")
     Include(FetchContent)
 
     FetchContent_Declare(
             pybind11
             GIT_REPOSITORY https://github.com/pybind/pybind11.git
             GIT_TAG v2.5.0)
     FetchContent_MakeAvailable(pybind11)
-    add_library(SymSpellCppPy MODULE SymSpellCppPy.cpp)
+    pybind11_add_module(SymSpellCppPy MODULE SymSpellCppPy.cpp)
     target_sources(SymSpellCppPy INTERFACE library.cpp library.h)
-    target_link_libraries(SymSpellCppPy PRIVATE SymSpellCpp pybind11::module)
-    set_target_properties(SymSpellCppPy PROPERTIES PREFIX "${PYTHON_MODULE_PREFIX}"
-            SUFFIX "${PYTHON_MODULE_EXTENSION}")
+    target_link_libraries(SymSpellCppPy PRIVATE SymSpellCpp)
     target_compile_options(SymSpellCppPy PRIVATE
             $<$<CONFIG:Release>:-O3 -DNDEBUG -march=native -mtune=native -fvisibility=hidden -flto>)
     message(STATUS "Build for Python = " ${BUILD_FOR_PYTHON})
 else ()
     Include(FetchContent)
 
     FetchContent_Declare(
```

### Comparing `SymSpellCppPy-0.0.8/PKG-INFO` & `SymSpellCppPy-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: SymSpellCppPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Fast SymSpell port for python written in C++ using pybind11.
 Home-page: https://github.com/viig99/SymSpellCppPy
 Author: Arjun Variar & Mohit Tare
 Author-email: accio.arjun@gmail.com
 License: UNKNOWN
 Description: # SymSpellCppPy
         A Fast SymSpell v6.5 port for python written in C++ using pybind11.
         
-        ![UnitTests](https://img.shields.io/github/workflow/status/viig99/SymSpellCppPy/UnitTests?style=flat-square)
+            ![UnitTests](https://img.shields.io/github/workflow/status/viig99/SymSpellCppPy/UnitTests?style=flat-square)
         ![Docs](https://img.shields.io/readthedocs/symspellcpppy?style=flat-square)
         ![Downloads](https://img.shields.io/pypi/dm/SymSpellCppPy?style=flat-square)
         ![License](https://img.shields.io/github/license/viig99/SymSpellCppPy?style=flat-square)
         
         ## Installation
         ```shell script
-        pip install SymSpellCppPy
+        pip install --upgrade SymSpellCppPy
         ```
         
         ## Documentation
         * Check [examples](https://symspellcpppy.readthedocs.io/en/latest/Examples.html) for provided usage.
         * Check [api docs](https://symspellcpppy.readthedocs.io/en/latest/SymSpellCppPy.html#pybind11-binding-for-symspellpy) for detailed API documentation.
+        * Check `tests/SymSpellCppPyTest.py` for extended api usage.
         
         ## Benchmark Results
         ```shell script
         pip install pytest pytest-benchmark symspellpy SymSpellCppPy
         pytest benchmark.py --benchmark-compare
         ```
         ![Benchmark Results](https://github.com/viig99/SymSpellCppPy/blob/master/resources/benchmark.png?raw=true)
```

### Comparing `SymSpellCppPy-0.0.8/README.md` & `SymSpellCppPy-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # SymSpellCppPy
 A Fast SymSpell v6.5 port for python written in C++ using pybind11.
 
-![UnitTests](https://img.shields.io/github/workflow/status/viig99/SymSpellCppPy/UnitTests?style=flat-square)
+    ![UnitTests](https://img.shields.io/github/workflow/status/viig99/SymSpellCppPy/UnitTests?style=flat-square)
 ![Docs](https://img.shields.io/readthedocs/symspellcpppy?style=flat-square)
 ![Downloads](https://img.shields.io/pypi/dm/SymSpellCppPy?style=flat-square)
 ![License](https://img.shields.io/github/license/viig99/SymSpellCppPy?style=flat-square)
 
 ## Installation
 ```shell script
-pip install SymSpellCppPy
+pip install --upgrade SymSpellCppPy
 ```
 
 ## Documentation
 * Check [examples](https://symspellcpppy.readthedocs.io/en/latest/Examples.html) for provided usage.
 * Check [api docs](https://symspellcpppy.readthedocs.io/en/latest/SymSpellCppPy.html#pybind11-binding-for-symspellpy) for detailed API documentation.
+* Check `tests/SymSpellCppPyTest.py` for extended api usage.
 
 ## Benchmark Results
 ```shell script
 pip install pytest pytest-benchmark symspellpy SymSpellCppPy
 pytest benchmark.py --benchmark-compare
 ```
 ![Benchmark Results](https://github.com/viig99/SymSpellCppPy/blob/master/resources/benchmark.png?raw=true)
```

### Comparing `SymSpellCppPy-0.0.8/SymSpellCppPy.cpp` & `SymSpellCppPy-0.0.9/SymSpellCppPy.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -63,24 +63,33 @@
             .value("TOP", symspellcpppy::Verbosity::Top, "The suggestion with the highest term frequency of the suggestions of smallest edit distance found.")
             .value("CLOSEST", symspellcpppy::Verbosity::Closest, "All suggestions of smallest edit distance found, the suggestions are ordered by term frequency.")
             .value("ALL", symspellcpppy::Verbosity::All, "All suggestions <= maxEditDistance, the suggestions are ordered by edit distance, then by term frequency (slower, no early termination).")
             .export_values();
 
     py::class_<symspellcpppy::SymSpell>(m, "SymSpell")
             .def(py::init<int, int, int, int, unsigned char>(), "SymSpell builder options",
-                 py::arg("initial_capacity") = DEFAULT_INITIAL_CAPACITY,
                  py::arg("max_dictionary_edit_distance") = DEFAULT_MAX_EDIT_DISTANCE,
                  py::arg("prefix_length") = DEFAULT_PREFIX_LENGTH,
                  py::arg("count_threshold") = DEFAULT_COUNT_THRESHOLD,
+                 py::arg("initial_capacity") = DEFAULT_INITIAL_CAPACITY,
                  py::arg("compact_level") = DEFAULT_COMPACT_LEVEL
             )
             .def("word_count", &symspellcpppy::SymSpell::WordCount, "Number of words entered.")
             .def("max_length", &symspellcpppy::SymSpell::MaxLength, "Max length of words entered.")
             .def("entry_count", &symspellcpppy::SymSpell::EntryCount, "Total number of deletes formed.")
             .def("count_threshold", &symspellcpppy::SymSpell::CountThreshold, "Frequency of word so that its considered a valid word for spelling correction.")
+            .def("create_dictionary_entry", [](symspellcpppy::SymSpell &sym, const xstring &key, int64_t count) {
+                auto staging = std::make_shared<SuggestionStage>(128);
+                sym.CreateDictionaryEntry(key, count, staging);
+                sym.CommitStaged(staging);
+                return sym.EntryCount() > 0;
+            }, "Create/Update an entry in the dictionary.", py::arg("key"), py::arg("count"))
+            .def("delete_dictionary_entry", &symspellcpppy::SymSpell::DeleteDictionaryEntry,
+                 "Delete the key from the dictionary & updates internal representation accordingly.",
+                 py::arg("key"))
             .def("load_bigram_dictionary", py::overload_cast<const std::string &, int, int, xchar>(
                     &symspellcpppy::SymSpell::LoadBigramDictionary),
                  "Load multiple dictionary entries from a file of word/frequency count pairs.",
                  py::arg("corpus"),
                  py::arg("term_index"),
                  py::arg("count_index"),
                  py::arg("separator") = DEFAULT_SEPARATOR_CHAR)
```

### Comparing `SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/PKG-INFO` & `SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 Metadata-Version: 2.1
 Name: SymSpellCppPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Fast SymSpell port for python written in C++ using pybind11.
 Home-page: https://github.com/viig99/SymSpellCppPy
 Author: Arjun Variar & Mohit Tare
 Author-email: accio.arjun@gmail.com
 License: UNKNOWN
 Description: # SymSpellCppPy
         A Fast SymSpell v6.5 port for python written in C++ using pybind11.
         
-        ![UnitTests](https://img.shields.io/github/workflow/status/viig99/SymSpellCppPy/UnitTests?style=flat-square)
+            ![UnitTests](https://img.shields.io/github/workflow/status/viig99/SymSpellCppPy/UnitTests?style=flat-square)
         ![Docs](https://img.shields.io/readthedocs/symspellcpppy?style=flat-square)
         ![Downloads](https://img.shields.io/pypi/dm/SymSpellCppPy?style=flat-square)
         ![License](https://img.shields.io/github/license/viig99/SymSpellCppPy?style=flat-square)
         
         ## Installation
         ```shell script
-        pip install SymSpellCppPy
+        pip install --upgrade SymSpellCppPy
         ```
         
         ## Documentation
         * Check [examples](https://symspellcpppy.readthedocs.io/en/latest/Examples.html) for provided usage.
         * Check [api docs](https://symspellcpppy.readthedocs.io/en/latest/SymSpellCppPy.html#pybind11-binding-for-symspellpy) for detailed API documentation.
+        * Check `tests/SymSpellCppPyTest.py` for extended api usage.
         
         ## Benchmark Results
         ```shell script
         pip install pytest pytest-benchmark symspellpy SymSpellCppPy
         pytest benchmark.py --benchmark-compare
         ```
         ![Benchmark Results](https://github.com/viig99/SymSpellCppPy/blob/master/resources/benchmark.png?raw=true)
```

### Comparing `SymSpellCppPy-0.0.8/SymSpellCppPy.egg-info/SOURCES.txt` & `SymSpellCppPy-0.0.9/SymSpellCppPy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -101,11 +101,18 @@
 include/cereal/types/unordered_map.hpp
 include/cereal/types/unordered_set.hpp
 include/cereal/types/utility.hpp
 include/cereal/types/valarray.hpp
 include/cereal/types/variant.hpp
 include/cereal/types/vector.hpp
 include/cereal/types/concepts/pair_associative_container.hpp
+resources/frequency_bigramdictionary_en_243_342.txt
 resources/frequency_dictionary_en_82_765.txt
 resources/frequency_dictionary_en_test_verbosity.txt
 tests/CatchMain.cpp
-tests/SymSpellCppPyTest.py
+tests/SymSpellCppPyTest.py
+tests/fortests/bad_dict.txt
+tests/fortests/big_modified.txt
+tests/fortests/big_words.txt
+tests/fortests/noisy_query_en_1000.txt
+tests/fortests/non_en_dict.txt
+tests/fortests/separator_dict.txt
```

### Comparing `SymSpellCppPy-0.0.8/include/DamerauOSA.h` & `SymSpellCppPy-0.0.9/include/DamerauOSA.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/Defines.h` & `SymSpellCppPy-0.0.9/include/Defines.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/EditDistance.h` & `SymSpellCppPy-0.0.9/include/EditDistance.h`

 * *Files 20% similar despite different names*

```diff
@@ -32,11 +32,11 @@
                 this->distanceComparer = &levenshteinDistance;
                 break;
             default:
                 throw std::invalid_argument("Unknown distance algorithm.");
         }
     }
 
-    int Compare(xstring string1, xstring string2, int maxDistance) {
+    int Compare(xstring string1, xstring string2, double maxDistance) {
         return (int) this->distanceComparer->Distance(std::move(string1), std::move(string2), maxDistance);
     }
 };
```

### Comparing `SymSpellCppPy-0.0.8/include/Helpers.h` & `SymSpellCppPy-0.0.9/include/Helpers.h`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,15 @@
             if (permanentDeletesFinded != permanentDeletesEnd) {
                 suggestions = permanentDeletesFinded->second;
                 i = suggestions.size();
 
                 std::vector<xstring> newSuggestions;
                 newSuggestions.reserve(suggestions.size() + Delete.second.count);
                 std::copy(suggestions.begin(), suggestions.end(), back_inserter(newSuggestions));
+                suggestions = newSuggestions;
             } else {
                 i = 0;
                 int32_t count = Delete.second.count;
                 suggestions.reserve(count);
             }
 
             int next = Delete.second.first;
```

### Comparing `SymSpellCppPy-0.0.8/include/Levenshtein.h` & `SymSpellCppPy-0.0.9/include/Levenshtein.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/access.hpp` & `SymSpellCppPy-0.0.9/include/cereal/access.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/archives/adapters.hpp` & `SymSpellCppPy-0.0.9/include/cereal/archives/adapters.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/archives/binary.hpp` & `SymSpellCppPy-0.0.9/include/cereal/archives/binary.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/archives/json.hpp` & `SymSpellCppPy-0.0.9/include/cereal/archives/json.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/archives/portable_binary.hpp` & `SymSpellCppPy-0.0.9/include/cereal/archives/portable_binary.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/archives/xml.hpp` & `SymSpellCppPy-0.0.9/include/cereal/archives/xml.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/cereal.hpp` & `SymSpellCppPy-0.0.9/include/cereal/cereal.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/details/helpers.hpp` & `SymSpellCppPy-0.0.9/include/cereal/details/helpers.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/details/polymorphic_impl.hpp` & `SymSpellCppPy-0.0.9/include/cereal/details/polymorphic_impl.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/details/polymorphic_impl_fwd.hpp` & `SymSpellCppPy-0.0.9/include/cereal/details/polymorphic_impl_fwd.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/details/static_object.hpp` & `SymSpellCppPy-0.0.9/include/cereal/details/static_object.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/details/traits.hpp` & `SymSpellCppPy-0.0.9/include/cereal/details/traits.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/details/util.hpp` & `SymSpellCppPy-0.0.9/include/cereal/details/util.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/base64.hpp` & `SymSpellCppPy-0.0.9/include/cereal/external/base64.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/allocators.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/allocators.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/cursorstreamwrapper.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/cursorstreamwrapper.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/document.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/document.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/encodedstream.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/encodedstream.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/encodings.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/encodings.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/error/en.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/error/en.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/error/error.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/error/error.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/filereadstream.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/filereadstream.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/filewritestream.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/filewritestream.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/fwd.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/fwd.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/biginteger.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/biginteger.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/diyfp.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/diyfp.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/dtoa.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/dtoa.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/ieee754.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/ieee754.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/itoa.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/itoa.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/meta.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/meta.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/pow10.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/pow10.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/regex.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/regex.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/stack.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/stack.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/strfunc.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/strfunc.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/strtod.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/strtod.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/internal/swap.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/internal/swap.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/istreamwrapper.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/istreamwrapper.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/memorybuffer.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/memorybuffer.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/memorystream.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/memorystream.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/msinttypes/inttypes.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/msinttypes/inttypes.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/msinttypes/stdint.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/msinttypes/stdint.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/ostreamwrapper.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/ostreamwrapper.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/pointer.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/pointer.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/prettywriter.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/prettywriter.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/rapidjson.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/rapidjson.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/reader.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/reader.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/schema.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/schema.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/stream.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/stream.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/stringbuffer.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/stringbuffer.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidjson/writer.h` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidjson/writer.h`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/license.txt` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/license.txt`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml.hpp` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml_iterators.hpp` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml_iterators.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml_print.hpp` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml_print.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/external/rapidxml/rapidxml_utils.hpp` & `SymSpellCppPy-0.0.9/include/cereal/external/rapidxml/rapidxml_utils.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/macros.hpp` & `SymSpellCppPy-0.0.9/include/cereal/macros.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/specialize.hpp` & `SymSpellCppPy-0.0.9/include/cereal/specialize.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/array.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/array.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/atomic.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/atomic.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/base_class.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/base_class.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/bitset.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/bitset.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/boost_variant.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/boost_variant.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/chrono.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/chrono.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/common.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/common.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/complex.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/complex.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/concepts/pair_associative_container.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/concepts/pair_associative_container.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/deque.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/deque.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/forward_list.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/forward_list.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/functional.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/functional.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/list.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/list.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/map.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/map.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/memory.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/memory.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/optional.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/optional.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/polymorphic.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/polymorphic.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/queue.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/queue.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/set.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/set.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/stack.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/stack.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/string.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/string.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/tuple.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/tuple.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/unordered_map.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/unordered_map.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/unordered_set.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/unordered_set.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/utility.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/utility.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/valarray.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/valarray.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/variant.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/variant.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/types/vector.hpp` & `SymSpellCppPy-0.0.9/include/cereal/types/vector.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/include/cereal/version.hpp` & `SymSpellCppPy-0.0.9/include/cereal/version.hpp`

 * *Files identical despite different names*

### Comparing `SymSpellCppPy-0.0.8/library.cpp` & `SymSpellCppPy-0.0.9/library.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -3,89 +3,90 @@
 #include <codecvt>
 #include <utility>
 #include <fstream>
 
 namespace symspellcpppy {
 
     int SymSpell::MaxDictionaryEditDistance() const {
-        return this->maxDictionaryEditDistance;
+        return maxDictionaryEditDistance;
     }
 
     int SymSpell::PrefixLength() const {
-        return this->prefixLength;
+        return prefixLength;
     }
 
     int SymSpell::MaxLength() const {
-        return this->maxDictionaryWordLength;
+        return maxDictionaryWordLength;
     }
 
     long SymSpell::CountThreshold() const {
-        return this->countThreshold;
+        return countThreshold;
     }
 
     int SymSpell::WordCount() {
-        return this->words.size();
+        return words.size();
     }
 
     int SymSpell::EntryCount() {
-        return this->deletes->size();
+        return deletes->size();
     }
 
-    SymSpell::SymSpell(int initialCapacity, int maxDictionaryEditDistance, int prefixLength, int countThreshold,
-                       unsigned char compactLevel) {
-        if (initialCapacity < 0) throw std::invalid_argument("initialCapacity");
-        if (maxDictionaryEditDistance < 0) throw std::invalid_argument("maxDictionaryEditDistance");
-        if (prefixLength < 1 || prefixLength <= maxDictionaryEditDistance) throw std::invalid_argument("prefixLength");
-        if (countThreshold < 0) throw std::invalid_argument("countThreshold");
-        if (compactLevel > 16) throw std::invalid_argument("compactLevel");
-
-        this->initialCapacity = initialCapacity;
-        this->words.reserve(initialCapacity);
-        this->maxDictionaryEditDistance = maxDictionaryEditDistance;
-        this->prefixLength = prefixLength;
-        this->countThreshold = countThreshold;
-        if (compactLevel > 16) compactLevel = 16;
-        this->compactMask = (UINT_MAX >> (3 + compactLevel)) << 2;
-        this->maxDictionaryWordLength = 0;
-        this->words = std::unordered_map<xstring, int64_t>(initialCapacity);
+    SymSpell::SymSpell(int _maxDictionaryEditDistance, int _prefixLength, int _countThreshold, int _initialCapacity,
+                       unsigned char _compactLevel) :
+            maxDictionaryEditDistance(_maxDictionaryEditDistance),
+            prefixLength(_prefixLength),
+            countThreshold(_countThreshold),
+            initialCapacity(_initialCapacity) {
+        if (_initialCapacity < 0) throw std::invalid_argument("initial_capacity is too small.");
+        if (_maxDictionaryEditDistance < 0) throw std::invalid_argument("max_dictionary_edit_distance cannot be negative");
+        if (_prefixLength < 1 || _prefixLength <= _maxDictionaryEditDistance)
+            throw std::invalid_argument("prefix_length cannot be less than 1 or smaller than max_dictionary_edit_distance");
+        if (_countThreshold < 0) throw std::invalid_argument("count_threshold cannot be negative");
+        if (_compactLevel > 16) throw std::invalid_argument("compact_level cannot be greater than 16");
+
+        words.reserve(initialCapacity);
+        if (_compactLevel > 16) _compactLevel = 16;
+        compactMask = (UINT_MAX >> (3 + _compactLevel)) << 2;
+        maxDictionaryWordLength = 0;
+        words = std::unordered_map<xstring, int64_t>(initialCapacity);
     }
 
     bool SymSpell::CreateDictionaryEntry(const xstring &key, int64_t count,
                                          const std::shared_ptr<SuggestionStage> &staging) {
 
         if (count <= 0) {
-            if (this->countThreshold > 0)
+            if (countThreshold > 0)
                 return false; // no point doing anything if count is zero, as it can't change anything
             count = 0;
         }
         int countPrevious = -1;
         auto belowThresholdWordsFinded = belowThresholdWords.find(key);
         auto wordsFinded = words.find(key);
         if (countThreshold > 1 && belowThresholdWordsFinded != belowThresholdWords.end()) {
             countPrevious = belowThresholdWordsFinded->second;
             count = (MAXINT - countPrevious > count) ? countPrevious + count : MAXINT;
             if (count >= countThreshold) {
                 belowThresholdWords.erase(key);
             } else {
-                belowThresholdWords.insert(std::pair<xstring, int64_t>(key, count));
+                belowThresholdWords[key] = count;
                 return false;
             }
         } else if (wordsFinded != words.end()) {
             countPrevious = wordsFinded->second;
             count = (MAXINT - countPrevious > count) ? countPrevious + count : MAXINT;
-            words.insert(std::pair<xstring, int64_t>(key, count));
+            words.at(key) = count;
             return false;
         } else if (count < CountThreshold()) {
-            belowThresholdWords.insert(std::pair<xstring, int64_t>(key, count));
+            belowThresholdWords[key] = count;
             return false;
         }
 
         words.insert(std::pair<xstring, int64_t>(key, count));
 
-        if (key.size() > this->maxDictionaryWordLength) this->maxDictionaryWordLength = key.size();
+        if (key.size() > maxDictionaryWordLength) maxDictionaryWordLength = key.size();
 
         //create deletes
         auto edits = EditsPrefix(key);
         if (staging != nullptr) {
             for (const auto &edit : *edits) {
                 staging->Add(GetstringHash(edit), key);
             }
@@ -93,32 +94,56 @@
 
             for (const auto &edit : *edits) {
                 int deleteHash = GetstringHash(edit);
                 auto deletesFinded = deletes->find(deleteHash);
                 std::vector<xstring> suggestions;
                 if (deletesFinded != deletes->end()) {
                     suggestions = deletesFinded->second;
-                    std::vector<xstring> newSuggestions(suggestions.size() + 1);
-                    for (int id = 0; id < suggestions.size(); id++) {
-                        newSuggestions[id] = suggestions[id];
-                    }
-
-                    (*deletes)[deleteHash] = suggestions = newSuggestions;
+                    std::vector<xstring> newSuggestions;
+                    newSuggestions.reserve(suggestions.size() + 1);
+                    std::copy(suggestions.begin(), suggestions.end(), std::back_inserter(newSuggestions));
+                    deletes->at(deleteHash) = suggestions = newSuggestions;
                 } else {
                     suggestions = std::vector<xstring>(1);
-                    (*deletes).insert(std::pair<int, std::vector<xstring>>(deleteHash, suggestions));
+                    deletes->insert(std::pair<int, std::vector<xstring>>(deleteHash, suggestions));
                 }
                 suggestions[suggestions.size() - 1] = key;
             }
 
         }
 
         return true;
     }
 
+    bool SymSpell::DeleteDictionaryEntry(const std::string &key) {
+        auto wordsFinded = words.find(key);
+        if (wordsFinded != words.end()) {
+            words.erase(wordsFinded);
+            if(wordsFinded->first.size() == maxDictionaryWordLength) {
+                int max_size = 0;
+                for (auto& word: words) {
+                    max_size = std::max(static_cast<int>(word.first.size()), max_size);
+                }
+                maxDictionaryWordLength = max_size;
+            }
+            auto edits = EditsPrefix(key);
+            for (const auto &edit: *edits) {
+                int deleteHash = GetstringHash(edit);
+                auto deletesFinded = deletes->find(deleteHash);
+                if (deletesFinded != deletes->end()) {
+                    auto delete_vec = deletesFinded->second;
+                    auto it = std::find (delete_vec.begin(), delete_vec.end(), key);
+                    if (it < delete_vec.end()) delete_vec.erase(it);
+                }
+            }
+            return true;
+        }
+        return false;
+    }
+
     bool
     SymSpell::LoadBigramDictionary(const std::string &corpus, int termIndex, int countIndex, xchar separatorChars) {
         xifstream corpusStream;
         corpusStream.open(corpus);
 #ifdef UNICODE_SUPPORT
         std::locale utf8(std::locale(), new std::codecvt_utf8<wchar_t>);
         corpusStream.imbue(utf8);
@@ -187,26 +212,28 @@
             i++;
             std::vector<xstring> lineParts;
             xstringstream ss(line);
             xstring token;
             while (getline(ss, token, separatorChars))
                 lineParts.push_back(token);
             if (lineParts.size() >= 2) {
-                int64_t count = stoll(lineParts[countIndex]);
-
+                int64_t count = 1;
+                try {
+                    count = std::stoll(lineParts[countIndex]);
+                } catch (const std::invalid_argument&) {
+                    // Do nothing
+                }
                 CreateDictionaryEntry(lineParts[termIndex], count, staging);
             } else {
                 CreateDictionaryEntry(line, 1, staging);
             }
 
         }
-        if (this->deletes == nullptr)
-            this->deletes = std::make_shared<std::unordered_map<int, std::vector<xstring>>>(staging->DeleteCount());
         CommitStaged(staging);
-        if (this->EntryCount() == 0)
+        if (EntryCount() == 0)
             return false;
         return true;
     }
 
     bool SymSpell::CreateDictionary(const std::string &corpus) {
         xifstream corpusStream;
         corpusStream.open(corpus);
@@ -224,46 +251,46 @@
         auto staging = std::make_shared<SuggestionStage>(16384);
         while (getline(corpusStream, line)) {
             for (const xstring &key : ParseWords(line)) {
                 CreateDictionaryEntry(key, 1, staging);
             }
 
         }
-        if (this->deletes == nullptr)
-            this->deletes = std::make_shared<std::unordered_map<int, std::vector<xstring>>>(staging->DeleteCount());
         CommitStaged(staging);
-        if (this->EntryCount() == 0)
+        if (EntryCount() == 0)
             return false;
         return true;
     }
 
     void SymSpell::PurgeBelowThresholdWords() {
         belowThresholdWords.clear();
     }
 
     void SymSpell::CommitStaged(const std::shared_ptr<SuggestionStage> &staging) {
+        if (deletes == nullptr)
+            deletes = std::make_shared<std::unordered_map<int, std::vector<xstring>>>(staging->DeleteCount());
         staging->CommitTo(deletes);
     }
 
     std::vector<SuggestItem> SymSpell::Lookup(xstring input, Verbosity verbosity) {
-        return Lookup(std::move(input), verbosity, this->maxDictionaryEditDistance, false);
+        return Lookup(std::move(input), verbosity, maxDictionaryEditDistance, false);
     }
 
     std::vector<SuggestItem> SymSpell::Lookup(xstring input, Verbosity verbosity, int maxEditDistance) {
         return Lookup(std::move(input), verbosity, maxEditDistance, false);
     }
 
     std::vector<SuggestItem>
     SymSpell::Lookup(xstring input, Verbosity verbosity, int maxEditDistance, bool includeUnknown) {
         int skip = 0;
-        if (maxEditDistance > this->maxDictionaryEditDistance) throw std::invalid_argument("maxEditDistance");
+        if (maxEditDistance > maxDictionaryEditDistance) throw std::invalid_argument("Distance too large");
 
         std::vector<SuggestItem> suggestions;
         int inputLen = input.size();
-        if (inputLen - maxEditDistance > this->maxDictionaryWordLength) skip = 1;
+        if (inputLen - maxEditDistance > maxDictionaryWordLength) skip = 1;
 
         int64_t suggestionCount = 0;
         if (words.count(input) && !skip) {
             suggestionCount = words.at(input);
             suggestions.emplace_back(input, 0, suggestionCount);
             if (verbosity != All) skip = 1;
         }
@@ -283,15 +310,15 @@
             int inputPrefixLen = inputLen;
             if (inputPrefixLen > prefixLength) {
                 inputPrefixLen = prefixLength;
                 candidates.push_back(input.substr(0, inputPrefixLen));
             } else {
                 candidates.push_back(input);
             }
-            auto distanceComparer = EditDistance(this->distanceAlgorithm);
+            auto distanceComparer = EditDistance(distanceAlgorithm);
             while (candidatePointer < candidates.size()) {
                 xstring candidate = candidates[candidatePointer++];
                 int candidateLen = candidate.size();
                 int lengthDiff = inputPrefixLen - candidateLen;
 
                 if (lengthDiff > maxEditDistance2) {
                     if (verbosity == Verbosity::All) continue;
@@ -432,51 +459,51 @@
                     if (editDistance < maxDictionaryEditDistance) Edits(del, editDistance, deleteWords);
                 }
             }
         }
         return deleteWords;
     }
 
-    std::shared_ptr<std::unordered_set<xstring>> SymSpell::EditsPrefix(xstring key) {
+        std::shared_ptr<std::unordered_set<xstring>> SymSpell::EditsPrefix(xstring key) {
         auto m = std::make_shared<std::unordered_set<xstring>>();
         if (key.size() <= maxDictionaryEditDistance) m->insert(XL(""));
         if (key.size() > prefixLength) key = key.substr(0, prefixLength);
         m->insert(key);
         Edits(key, 0, m);
         return m;
     }
 
     int SymSpell::GetstringHash(xstring s) const {
         int len = s.size();
         int lenMask = len;
         if (lenMask > 3) lenMask = 3;
 
-        uint hash = 2166136261;
+        unsigned int hash = 2166136261;
         for (auto i = 0; i < len; i++) {
             {
                 hash ^= s[i];
                 hash *= 16777619;
             }
         }
 
-        hash &= this->compactMask;
+        hash &= compactMask;
         hash |= (uint) lenMask;
         return (int) hash;
     }
 
     std::vector<SuggestItem> SymSpell::LookupCompound(const xstring &input) {
-        return LookupCompound(input, this->maxDictionaryEditDistance);
+        return LookupCompound(input, maxDictionaryEditDistance);
     }
 
     std::vector<SuggestItem> SymSpell::LookupCompound(const xstring &input, int editDistanceMax) {
         std::vector<xstring> termList1 = ParseWords(input);
 
         std::vector<SuggestItem> suggestions;     //suggestions for a single term
         std::vector<SuggestItem> suggestionParts; //1 line with separate parts
-        auto distanceComparer = EditDistance(this->distanceAlgorithm);
+        auto distanceComparer = EditDistance(distanceAlgorithm);
 
         bool lastCombi = false;
         for (int i = 0; i < termList1.size(); i++) {
             suggestions = Lookup(termList1[i], Top, editDistanceMax);
 
             if ((i > 0) && !lastCombi) {
                 std::vector<SuggestItem> suggestionsCombi = Lookup(termList1[i - 1] + termList1[i], Top,
@@ -531,15 +558,15 @@
 
                                 if (suggestionSplitBest.count) {
                                     if (distance2 > suggestionSplitBest.distance) continue;
                                     if (distance2 < suggestionSplitBest.distance) suggestionSplitBest.count = 0;
                                 }
 
                                 suggestionSplit.distance = distance2;
-                                if (bigrams.count(suggestionSplit.term)) {
+                                if (bigrams.count(suggestionSplit.term) > 0) {
                                     long bigramCount = bigrams.at(suggestionSplit.term);
                                     suggestionSplit.count = bigramCount;
                                     if (!suggestions.empty()) {
                                         if ((suggestions1[0].term + suggestions2[0].term == termList1[i])) {
                                             suggestionSplit.count = std::max(suggestionSplit.count,
                                                                              suggestions[0].count + 2);
                                         } else if ((suggestions1[0].term == suggestions[0].term) ||
@@ -557,15 +584,15 @@
                                 } else {
                                     suggestionSplit.count = std::min(bigramCountMin,
                                                                      (int64_t) ((double) suggestions1[0].count /
                                                                                 (double) N *
                                                                                 (double) suggestions2[0].count));
                                 }
 
-                                if (suggestionSplit.count > suggestionSplitBest.count)
+                                if (suggestionSplitBest.count == 0 || (suggestionSplit.count > suggestionSplitBest.count))
                                     suggestionSplitBest.set(suggestionSplit);
                             }
                         }
                     }
 
                     if (suggestionSplitBest.count) {
                         suggestionParts.push_back(suggestionSplitBest);
@@ -602,22 +629,28 @@
 
         std::vector<SuggestItem> suggestionsLine;
         suggestionsLine.push_back(suggestion);
         return suggestionsLine;
     }
 
     Info SymSpell::WordSegmentation(const xstring &input) {
-        return WordSegmentation(input, this->MaxDictionaryEditDistance(), this->maxDictionaryWordLength);
+        return WordSegmentation(input, MaxDictionaryEditDistance(), maxDictionaryWordLength);
     }
 
     Info SymSpell::WordSegmentation(const xstring &input, int maxEditDistance) {
-        return WordSegmentation(input, maxEditDistance, this->maxDictionaryWordLength);
+        return WordSegmentation(input, maxEditDistance, maxDictionaryWordLength);
     }
 
     Info SymSpell::WordSegmentation(const xstring &input, int maxEditDistance, int maxSegmentationWordLength) {
+        // v6.7
+        // normalize ligatures:
+        // "scientific"
+        // "scientiﬁc" "ﬁelds" "ﬁnal"
+        // TODO: Figure out how to do the below utf-8 normalization in C++.
+        // input = input.Normalize(System.Text.NormalizationForm.FormKC).Replace("\u002D", "");//.Replace("\uC2AD","");
         int arraySize = std::min(maxSegmentationWordLength, (int) input.size());
         std::vector<Info> compositions = std::vector<Info>(arraySize);
         int circularIndex = -1;
 
         for (int j = 0; j < input.size(); j++) {
             int imax = std::min((int) input.size() - j, maxSegmentationWordLength);
             for (int i = 1; i <= imax; i++) {
@@ -634,43 +667,70 @@
                 }
 
                 topEd += part.size();
                 xregex r(XL(" "));
                 part = regex_replace(part, r, XL(""));
                 topEd -= part.size();
 
-                std::vector<SuggestItem> results = this->Lookup(part, Top, maxEditDistance);
+                //v6.7
+                //Lookup against the lowercase term
+                auto partLower = part;
+                std::transform(part.begin(), part.end(), partLower.begin(), ::tolower);
+                std::vector<SuggestItem> results = Lookup(partLower, Top, maxEditDistance);
                 if (!results.empty()) {
                     topResult = results[0].term;
+
+                    //v6.7
+                    //retain/preserve upper case
+                    if (std::isupper(part[0]))
+                    {
+                        topResult[0] = std::toupper(topResult[0]);
+                    }
+
+
                     topEd += results[0].distance;
                     topProbabilityLog = log10((double) results[0].count / (double) N);
                 } else {
                     topResult = part;
                     topEd += part.size();
                     topProbabilityLog = log10(10.0 / (N * pow(10.0, part.size())));
                 }
 
                 int destinationIndex = ((i + circularIndex) % arraySize);
 
+                auto circular_distance = compositions[circularIndex].getDistance();
+                auto destination_distance = compositions[destinationIndex].getDistance();
+                auto circular_probablity = compositions[circularIndex].getProbability();
+                auto destination_probablity = compositions[destinationIndex].getProbability();
+
                 if (j == 0) {
                     compositions[destinationIndex].set(part, topResult, topEd, topProbabilityLog);
                 } else if ((i == maxSegmentationWordLength)
-                           || (((compositions[circularIndex].getDistance() + topEd ==
-                                 compositions[destinationIndex].getDistance()) \
- || (compositions[circularIndex].getDistance() + separatorLength + topEd ==
-     compositions[destinationIndex].getDistance())) \
- && (compositions[destinationIndex].getProbability() <
-     compositions[circularIndex].getProbability() + topProbabilityLog))
-                           || (compositions[circularIndex].getDistance() + separatorLength + topEd <
-                               compositions[destinationIndex].getDistance())) {
-                    xstring seg = compositions[circularIndex].getSegmented() + XL(" ") + part;
-                    xstring correct = compositions[circularIndex].getCorrected() + XL(" ") + topResult;
-                    int d = compositions[circularIndex].getDistance() + separatorLength + topEd;
-                    double prob = compositions[circularIndex].getProbability() + topProbabilityLog;
-                    compositions[destinationIndex].set(seg, correct, d, prob);
+                           || (((circular_distance + topEd == destination_distance)
+                                || (circular_distance + separatorLength + topEd == destination_distance))
+                               && (destination_probablity < circular_probablity + topProbabilityLog))
+                           || (circular_distance + separatorLength + topEd < destination_distance)) {
+                    //v6.7
+                    //keep punctuation or spostrophe adjacent to previous word
+                    if (((topResult.size() == 1) && std::ispunct(topResult[0])) || ((topResult.size() == 2) &&
+                                                                                          topResult.rfind("’", 0) == 0)) {
+                        xstring seg = compositions[circularIndex].getSegmented() + part;
+                        xstring correct = compositions[circularIndex].getCorrected() + topResult;
+                        int d = circular_distance        + topEd;
+                        double prob = circular_probablity + topProbabilityLog;
+                        compositions[destinationIndex].set(seg, correct, d, prob);
+                    }
+                    else {
+                        xstring seg = compositions[circularIndex].getSegmented() + XL(" ") + part;
+                        xstring correct = compositions[circularIndex].getCorrected() + XL(" ") + topResult;
+                        int d = circular_distance + separatorLength + topEd;
+                        double prob = circular_probablity + topProbabilityLog;
+                        compositions[destinationIndex].set(seg, correct, d, prob);
+                    }
+
                 }
             }
             circularIndex++;
             if (circularIndex == arraySize) circularIndex = 0;
         }
         return compositions[circularIndex];
     }
```

### Comparing `SymSpellCppPy-0.0.8/library.h` & `SymSpellCppPy-0.0.9/library.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #pragma once
 
 //#define UNICODE_SUPPORT
-#define DEFAULT_SEPARATOR_CHAR XL('\t')
+#define DEFAULT_SEPARATOR_CHAR XL(' ')
 #define DEFAULT_MAX_EDIT_DISTANCE 2
 #define DEFAULT_PREFIX_LENGTH 7
 #define DEFAULT_COUNT_THRESHOLD 1
 #define DEFAULT_INITIAL_CAPACITY 82765
 #define DEFAULT_COMPACT_LEVEL 5
 #define min3(a, b, c) (min(a, min(b, c)))
-#define MAXINT INT_MAX
+#define MAXINT LLONG_MAX
 #define M
-#define MAXLONG LONG_MAX
+#define MAXLONG MAXINT
 
 #include <fstream>
 #include <sstream>
 #include <cstring>
 #include <cstdlib>
 #include <algorithm>
 #include <cctype>
@@ -130,20 +130,22 @@
         /// but it can help speed up processing by alleviating the need for
         /// data restructuring as the size grows.</remarks>
         /// <param name="initialCapacity">The expected number of words in dictionary.</param>
         /// <param name="maxDictionaryEditDistance">Maximum edit distance for doing lookups.</param>
         /// <param name="prefixLength">The length of word prefixes used for spell checking..</param>
         /// <param name="countThreshold">The minimum frequency count for dictionary words to be considered correct spellings.</param>
         /// <param name="compactLevel">Degree of favoring lower memory use over speed (0=fastest,most memory, 16=slowest,least memory).</param>
-        explicit SymSpell(int initialCapacity = DEFAULT_INITIAL_CAPACITY,
-                          int maxDictionaryEditDistance = DEFAULT_MAX_EDIT_DISTANCE,
+        explicit SymSpell(int maxDictionaryEditDistance = DEFAULT_MAX_EDIT_DISTANCE,
                           int prefixLength = DEFAULT_PREFIX_LENGTH, int countThreshold = DEFAULT_COUNT_THRESHOLD,
+                          int initialCapacity = DEFAULT_INITIAL_CAPACITY,
                           unsigned char compactLevel = DEFAULT_COMPACT_LEVEL);
 
-        bool CreateDictionaryEntry(const xstring &key, int64_t count, const std::shared_ptr<SuggestionStage>& staging);
+        bool CreateDictionaryEntry(const xstring &key, int64_t count, const std::shared_ptr<SuggestionStage> &staging);
+
+        bool DeleteDictionaryEntry(const xstring &key);
 
         std::unordered_map<xstring, long> bigrams;
         int64_t bigramCountMin = MAXLONG;
 
         /// <summary>Load multiple dictionary entries from a file of word/frequency count pairs</summary>
         /// <remarks>Merges with any dictionary data already loaded.</remarks>
         /// <param name="corpus">The path+filename of the file.</param>
@@ -179,15 +181,15 @@
         bool CreateDictionary(xifstream &corpusStream);
 
         /// <summary>Remove all below threshold words from the dictionary.</summary>
         /// <remarks>This can be used to reduce memory consumption after populating the dictionary from
         /// a corpus using CreateDictionary.</remarks>
         void PurgeBelowThresholdWords();
 
-        void CommitStaged(const std::shared_ptr<SuggestionStage>& staging);
+        void CommitStaged(const std::shared_ptr<SuggestionStage> &staging);
 
         /// <summary>Find suggested spellings for a given input word, using the maximum
         /// edit distance specified during construction of the SymSpell dictionary.</summary>
         /// <param name="input">The word being spell checked.</param>
         /// <param name="verbosity">The value controlling the quantity/closeness of the retuned suggestions.</param>
         /// <returns>A List of SuggestItem object representing suggested correct spellings for the input word,
         /// sorted by edit distance, and secondarily by count frequency.</returns>
@@ -285,14 +287,13 @@
         /// <returns>The word segmented string,
         /// the word segmented and spelling corrected string,
         /// the Edit distance sum between input string and corrected string,
         /// the Sum of word occurrence probabilities in log scale (a measure of how common and probable the corrected segmentation is).</returns>
         Info WordSegmentation(const xstring &input, int maxEditDistance, int maxSegmentationWordLength);
 
 
-        template <class Archive>
-        void serialize( Archive & ar )
-        {
-            ar(deletes, words, maxDictionaryWordLength  );
+        template<class Archive>
+        void serialize(Archive &ar) {
+            ar(deletes, words, maxDictionaryWordLength);
         }
     };
 }
```

### Comparing `SymSpellCppPy-0.0.8/resources/frequency_dictionary_en_82_765.txt` & `SymSpellCppPy-0.0.9/resources/frequency_dictionary_en_82_765.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-﻿the 23135851162
+the 23135851162
 of 13151942776
 and 12997637966
 to 12136980858
 a 9081174698
 in 8469404971
 for 5933321709
 is 4705743816
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `SymSpellCppPy-0.0.8/setup.py` & `SymSpellCppPy-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,21 @@
+#!/usr/bin/env python
+
 import os
 import re
 import sys
 import platform
 import subprocess
-import unittest
 
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext
 from distutils.version import LooseVersion
 
-def find_test_suite():
-    test_loader = unittest.TestLoader()
-    test_suite = test_loader.discover('tests', pattern='*.py')
-    return test_suite
-
 from os import path
+
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 class CMakeExtension(Extension):
     def __init__(self, name, sourcedir=''):
@@ -71,26 +68,27 @@
 
         env = os.environ.copy()
         env['CXXFLAGS'] = '{} -DVERSION_INFO=\\"{}\\"'.format(env.get('CXXFLAGS', ''),
                                                               self.distribution.get_version())
         if not os.path.exists(self.build_temp):
             os.makedirs(self.build_temp)
         subprocess.check_call(['cmake', ext.sourcedir] + cmake_args, cwd=self.build_temp, env=env)
-        subprocess.check_call(['cmake', '--build', '.', '--target', os.path.basename(ext.name)] + build_args, cwd=self.build_temp)
+        subprocess.check_call(['cmake', '--build', '.', '--target', os.path.basename(ext.name)] + build_args,
+                              cwd=self.build_temp)
 
 
 setup(
     name='SymSpellCppPy',
-    version='0.0.8',
+    version='0.0.9',
     author='Arjun Variar & Mohit Tare',
     author_email='accio.arjun@gmail.com',
     description='A Fast SymSpell port for python written in C++ using pybind11.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    test_suite='setup.find_test_suite',
+    test_suite="tests/SymSpellCppPyTest.py",
     ext_modules=[CMakeExtension('SymSpellCppPy')],
     cmdclass=dict(build_ext=CMakeBuild),
     python_requires=">=3.4",
     zip_safe=False,
     url="https://github.com/viig99/SymSpellCppPy",
     classifiers=[
         "Intended Audience :: Developers",
```

### Comparing `SymSpellCppPy-0.0.8/tests/CatchMain.cpp` & `SymSpellCppPy-0.0.9/tests/CatchMain.cpp`

 * *Files 20% similar despite different names*

```diff
@@ -2,117 +2,139 @@
 
 #include "catch2/catch.hpp"
 #include "../library.h"
 
 using namespace symspellcpppy;
 
 TEST_CASE("Testing English", "[english]") {
-    const int initialCapacity = 82765;
     const int maxEditDistance = 2;
     const int prefixLength = 3;
 
     SECTION("Do Word Segmentation") {
-        SymSpell symSpell(initialCapacity, maxEditDistance, prefixLength);
+        SymSpell symSpell(maxEditDistance, prefixLength);
         symSpell.LoadDictionary("../resources/frequency_dictionary_en_82_765.txt", 0, 1, XL(' '));
         std::unordered_map<xstring, xstring> sentences = {
-                {XL("thequickbrownfoxjumpsoverthelazydog"),                                                XL("they quick brown fox jumps over therapy dog")},
-                {XL("itwasabrightcolddayinaprilandtheclockswerestrikingthirteen"),                         XL("it was bright holiday in april another clocks were striking thirteen")},
-                {XL("itwasthebestoftimesitwastheworstoftimesitwastheageofwisdomitwastheageoffoolishness"), XL("it waste best of times it waste worst of times it was thereof wisdom it was thereof foolishness")}
+                {XL("thequickbrownfoxjumpsoverthelazydog"),                                                XL("the quick brown fox jumps over the lazy dog")},
+                {XL("itwasabrightcolddayinaprilandtheclockswerestrikingthirteen"),                         XL("it was bright holiday in april and the clocks were striking thirteen")},
+                {XL("itwasthebestoftimesitwastheworstoftimesitwastheageofwisdomitwastheageoffoolishness"), XL("iowa the best of times it waste worst of times it was thereof wisdom it was thereof foolishness")}
         };
 
         for (auto &sentence : sentences) {
-            Info results = symSpell.WordSegmentation(sentence.first);
+            auto results = symSpell.WordSegmentation(sentence.first);
             REQUIRE(results.getCorrected() == sentence.second);
         }
     }
 
     SECTION("Do Spell Correction") {
-        SymSpell symSpell(initialCapacity, maxEditDistance, prefixLength);
+        SymSpell symSpell(maxEditDistance, prefixLength);
         symSpell.LoadDictionary("../resources/frequency_dictionary_en_82_765.txt", 0, 1, XL(' '));
         std::unordered_map<xstring, xstring> words = {
-                {XL("tke"),          XL("take")},
+                {XL("tke"),          XL("the")},
                 {XL("abolution"),    XL("abolition")},
                 {XL("intermedaite"), XL("intermediate")}
         };
 
         for (auto &word : words) {
-            std::vector<SuggestItem> results = symSpell.Lookup(word.first, Verbosity::Closest);
+            auto results = symSpell.Lookup(word.first, Verbosity::Closest);
             REQUIRE(results[0].term == word.second);
         }
     }
 
     SECTION("Do Spell Correction With MaxEditDistance=2") {
-        SymSpell symSpell(initialCapacity, maxEditDistance, prefixLength);
+        SymSpell symSpell(maxEditDistance, prefixLength);
         symSpell.LoadDictionary("../resources/frequency_dictionary_en_82_765.txt", 0, 1, XL(' '));
         std::unordered_map<xstring, xstring> words_within_distance = {
-                {XL("tke"),     XL("take")},
+                {XL("tke"),     XL("the")},
                 {XL("extrine"), XL("extreme")}
         };
 
         std::unordered_map<xstring, xstring> words_far_distance = {
                 {XL("elipnaht"),   XL("elephant")},
                 {XL("aotocrasie"), XL("autocracy")}
         };
 
         for (auto &word : words_within_distance) {
-            std::vector<SuggestItem> results = symSpell.Lookup(word.first, Verbosity::Closest, 2);
+            auto results = symSpell.Lookup(word.first, Verbosity::Closest, 2);
             REQUIRE(results[0].term == word.second);
         }
 
         for (auto &word : words_far_distance) {
-            std::vector<SuggestItem> results = symSpell.Lookup(word.first, Verbosity::Closest, 2);
+            auto results = symSpell.Lookup(word.first, Verbosity::Closest, 2);
             REQUIRE(results.empty());
         }
     }
 
     SECTION("Correct Compound Mistakes") {
-        SymSpell symSpell(initialCapacity, maxEditDistance, prefixLength);
+        SymSpell symSpell(maxEditDistance, prefixLength);
         symSpell.LoadDictionary("../resources/frequency_dictionary_en_82_765.txt", 0, 1, XL(' '));
+        symSpell.LoadBigramDictionary("../resources/frequency_bigramdictionary_en_243_342.txt", 0, 2, XL(' '));
         std::unordered_map<xstring, xstring> compunded_sentences = {
-                {XL("whereis th elove hehad dated forImuch of thepast who couqdn'tread in sixthgrade and ins pired him"), XL("whereas to love head dated for much of theist who couldn't read in sixth grade and inspired him")},
-                {XL("in te dhird qarter oflast jear he hadlearned ofca sekretplan"),                                      XL("in to third quarter of last year he had learned of a secret plan")},
-                {XL("the bigjest playrs in te strogsommer film slatew ith plety of funn"),                                XL("they biggest players in to strong summer film slate with plenty of fun")}
+                {XL("whereis th elove"),                                                                                  XL("where is the love")},
+                {XL("whereis th elove hehad dated forImuch of thepast who couqdn'tread in sixthgrade and ins pired him"), XL("where is the love he had dated for much of the past who couldn't read in sixth grade and inspired him")},
+                {XL("in te dhird qarter oflast jear he hadlearned ofca sekretplan"),                                      XL("in the third quarter of last year he had learned of a secret plan")},
+                {XL("the bigjest playrs in te strogsommer film slatew ith plety of funn"),                                XL("the biggest players in the strong summer film slate with plenty of fun")}
         };
 
         for (auto &sentence : compunded_sentences) {
-            std::vector<SuggestItem> results = symSpell.LookupCompound(sentence.first);
+            auto results = symSpell.LookupCompound(sentence.first);
             REQUIRE(results[0].term == sentence.second);
         }
     }
 
     SECTION("Check top verbosity") {
-        SymSpell symSpellcustom(initialCapacity, maxEditDistance, prefixLength);
+        SymSpell symSpellcustom(maxEditDistance, prefixLength);
         symSpellcustom.LoadDictionary("../resources/frequency_dictionary_en_test_verbosity.txt", 0, 1, XL(' '));
-        std::vector<SuggestItem> results = symSpellcustom.Lookup(XL("stream"), Verbosity::Top, 2);
+        auto results = symSpellcustom.Lookup(XL("stream"), Verbosity::Top, 2);
         REQUIRE(1 == results.size());
         REQUIRE(XL("streamc") == results[0].term);
     }
 
     SECTION("Check all verbosity") {
-        SymSpell symSpellcustom(initialCapacity, maxEditDistance, prefixLength);
+        SymSpell symSpellcustom(maxEditDistance, prefixLength);
         symSpellcustom.LoadDictionary("../resources/frequency_dictionary_en_test_verbosity.txt", 0, 1, XL(' '));
-        std::vector<SuggestItem> results = symSpellcustom.Lookup(XL("stream"), Verbosity::All, 2);
+        auto results = symSpellcustom.Lookup(XL("stream"), Verbosity::All, 2);
         REQUIRE(2 == results.size());
     }
 
     SECTION("check custom entry of dictionary") {
-        SymSpell symSpellcustom(100, maxEditDistance, prefixLength);
+        SymSpell symSpellcustom(maxEditDistance, prefixLength, DEFAULT_COUNT_THRESHOLD, DEFAULT_INITIAL_CAPACITY,
+                                DEFAULT_COMPACT_LEVEL);
         auto staging = std::make_shared<SuggestionStage>(100);
         symSpellcustom.CreateDictionaryEntry(XL("take"), 4, staging);
-        std::vector<SuggestItem> results = symSpellcustom.Lookup(XL("take"), Verbosity::Closest, 2);
+        auto results = symSpellcustom.Lookup(XL("take"), Verbosity::Closest, 2);
         REQUIRE(XL("take") == results[0].term);
     }
 
     SECTION("check save works fine.") {
-        SymSpell symSpellcustom(100, maxEditDistance, prefixLength);
+        SymSpell symSpellcustom(maxEditDistance, prefixLength, DEFAULT_COUNT_THRESHOLD, DEFAULT_INITIAL_CAPACITY,
+                                DEFAULT_COMPACT_LEVEL);
         symSpellcustom.LoadDictionary("../resources/frequency_dictionary_en_test_verbosity.txt", 0, 1, XL(' '));
         auto filepath = "../resources/model.bin";
         std::ofstream binary_path(filepath, std::ios::out | std::ios::app | std::ios::binary);
         if (binary_path.is_open()) {
             cereal::BinaryOutputArchive oarchive(binary_path);
             oarchive(symSpellcustom);
         } else {
             throw std::invalid_argument("Cannot save to file");
         }
         std::remove(filepath);
     }
+
+    SECTION("Compund mistakes distance") {
+        SymSpell symSpell(maxEditDistance, prefixLength);
+        symSpell.LoadDictionary("../resources/frequency_dictionary_en_82_765.txt", 0, 1, XL(' '));
+        symSpell.LoadBigramDictionary("../resources/frequency_bigramdictionary_en_243_342.txt", 0, 2, XL(' '));
+        std::string typo = "the bigjest playrs";
+        std::string correction = "the biggest players";
+        auto results = symSpell.LookupCompound(typo, 2);
+        REQUIRE(results[0].distance == 2);
+    }
+
+    SECTION("Compund mistakes capitals") {
+        SymSpell symSpell(maxEditDistance, prefixLength);
+        symSpell.LoadDictionary("../resources/frequency_dictionary_en_82_765.txt", 0, 1, XL(' '));
+        std::string typo = "can yu readthis";
+        std::string correction = "can you read this";
+        auto results = symSpell.LookupCompound(typo, 2);
+        REQUIRE(results[0].term == correction);
+    }
 }
```

