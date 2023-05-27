# Comparing `tmp/summa_embed-0.1.3.tar.gz` & `tmp/summa_embed-0.15.0.tar.gz`

## Comparing `summa_embed-0.1.3.tar` & `summa_embed-0.15.0.tar`

### file list

```diff
@@ -1,85 +1,86 @@
--rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 summa_embed-0.1.3/local_dependencies/summa-core/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/LICENSE
--rw-r--r--   0      501       20       92 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/collectors/mod.rs
--rw-r--r--   0      501       20     7087 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
--rw-r--r--   0      501       20     2107 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/custom_serializer.rs
--rw-r--r--   0      501       20     5015 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/default_tokenizers.rs
--rw-r--r--   0      501       20     1021 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/driver.rs
--rw-r--r--   0      501       20    13794 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/fruit_extractors.rs
--rw-r--r--   0      501       20    24562 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_holder.rs
--rw-r--r--   0      501       20    13833 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_registry.rs
--rw-r--r--   0      501       20    14335 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_writer_holder.rs
--rw-r--r--   0      501       20     1694 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
--rw-r--r--   0      501       20      144 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/mod.rs
--rw-r--r--   0      501       20     2045 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
--rw-r--r--   0      501       20     5038 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/mod.rs
--rw-r--r--   0      501       20     4711 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/queries/exists_query.rs
--rw-r--r--   0      501       20       54 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/queries/mod.rs
--rw-r--r--   0      501       20      163 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/mod.rs
--rw-r--r--   0      501       20    14304 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
--rw-r--r--   0      501       20     1589 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
--rw-r--r--   0      501       20    53911 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
--rw-r--r--   0      501       20     2216 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/segment_attributes.rs
--rw-r--r--   0      501       20     1901 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/snippet_generator.rs
--rw-r--r--   0      501       20    11168 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_document.rs
--rw-r--r--   0      501       20     7439 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs
--rw-r--r--   0      501       20     2162 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/config_proxy.rs
--rw-r--r--   0      501       20     3093 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/core.rs
--rw-r--r--   0      501       20     3512 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/file_proxy.rs
--rw-r--r--   0      501       20      383 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/mod.rs
--rw-r--r--   0      501       20     3335 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/configs/partial_proxy.rs
--rw-r--r--   0      501       20     8009 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs
--rw-r--r--   0      501       20     8014 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/caching_directory.rs
--rw-r--r--   0      501       20     7015 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
--rw-r--r--   0      501       20     5117 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/external_requests.rs
--rw-r--r--   0      501       20    17667 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
--rw-r--r--   0      501       20     2255 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/mod.rs
--rw-r--r--   0      501       20     6756 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/directories/network_directory.rs
--rw-r--r--   0      501       20     5192 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/errors.rs
--rw-r--r--   0      501       20     2447 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/hyper_external_request.rs
--rw-r--r--   0      501       20      742 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/lib.rs
--rw-r--r--   0      501       20     1471 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs
--rw-r--r--   0      501       20      960 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/label.rs
--rw-r--r--   0      501       20       92 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/mod.rs
--rw-r--r--   0      501       20      583 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/page_rank.rs
--rw-r--r--   0      501       20     9854 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/aggregation.rs
--rw-r--r--   0      501       20     2294 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/compression.rs
--rw-r--r--   0      501       20     1068 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
--rw-r--r--   0      501       20      323 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      662 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/order.rs
--rw-r--r--   0      501       20      582 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/snippet.rs
--rw-r--r--   0      501       20      411 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
--rw-r--r--   0      501       20     2048 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs
--rw-r--r--   0      501       20     1538 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
--rw-r--r--   0      501       20      826 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
--rw-r--r--   0      501       20      218 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/mod.rs
--rw-r--r--   0      501       20      480 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
--rw-r--r--   0      501       20     7908 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
--rw-r--r--   0      501       20      415 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/utils/mod.rs
--rw-r--r--   0      501       20      309 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/utils/random.rs
--rw-r--r--   0      501       20     3165 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/utils/sync.rs
--rw-r--r--   0      501       20      450 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-core/src/validators.rs
--rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 summa_embed-0.1.3/local_dependencies/summa-proto/Cargo.toml
--rw-r--r--   0      501       20     1050 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/LICENSE
--rw-r--r--   0      501       20     2129 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/build.rs
--rwxr-xr-x   0      501       20      244 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/gen-docs.sh
--rw-r--r--   0      501       20     2561 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/markdown.tmpl
--rw-r--r--   0      501       20        0 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/__init__.py
--rw-r--r--   0      501       20     1556 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/consumer_service.proto
--rw-r--r--   0      501       20    10377 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/index_service.proto
--rw-r--r--   0      501       20     7125 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/query.proto
--rw-r--r--   0      501       20      499 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/reflection_service.proto
--rw-r--r--   0      501       20      867 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/search_service.proto
--rw-r--r--   0      501       20       96 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/proto/utils.proto
--rw-r--r--   0      501       20     2183 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/lib.rs
--rw-r--r--   0      501       20     2683 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/collector.rs
--rw-r--r--   0      501       20      212 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/mod.rs
--rw-r--r--   0      501       20      424 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/query.rs
--rw-r--r--   0      501       20      613 2023-04-26 12:21:44.000000 summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/score.rs
--rw-r--r--   0        0        0      839 1970-01-01 00:00:00.000000 summa_embed-0.1.3/Cargo.toml
--rw-r--r--   0      501       20     2809 2023-04-26 12:21:44.000000 summa_embed-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0      501       20      685 2023-04-26 12:21:44.000000 summa_embed-0.1.3/.gitignore
--rw-r--r--   0      501       20      373 2023-04-26 12:21:44.000000 summa_embed-0.1.3/pyproject.toml
--rw-r--r--   0      501       20     4324 2023-04-26 12:21:44.000000 summa_embed-0.1.3/src/lib.rs
--rw-r--r--   0      501       20    88981 2023-04-26 12:22:14.000000 summa_embed-0.1.3/Cargo.lock
--rw-r--r--   0        0        0      260 1970-01-01 00:00:00.000000 summa_embed-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2073 1970-01-01 00:00:00.000000 summa_embed-0.15.0/local_dependencies/summa-core/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/LICENSE
+-rw-r--r--   0      501       20       92 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/collectors/mod.rs
+-rw-r--r--   0      501       20     7087 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs
+-rw-r--r--   0      501       20     2107 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/custom_serializer.rs
+-rw-r--r--   0      501       20     5015 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/default_tokenizers.rs
+-rw-r--r--   0      501       20     1021 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/driver.rs
+-rw-r--r--   0      501       20    13794 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/fruit_extractors.rs
+-rw-r--r--   0      501       20    24562 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_holder.rs
+-rw-r--r--   0      501       20    13833 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_registry.rs
+-rw-r--r--   0      501       20    14335 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_writer_holder.rs
+-rw-r--r--   0      501       20     1694 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs
+-rw-r--r--   0      501       20      144 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/mod.rs
+-rw-r--r--   0      501       20     2045 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs
+-rw-r--r--   0      501       20     5038 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/mod.rs
+-rw-r--r--   0      501       20     4711 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/queries/exists_query.rs
+-rw-r--r--   0      501       20       54 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/queries/mod.rs
+-rw-r--r--   0      501       20      163 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/mod.rs
+-rw-r--r--   0      501       20    14304 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs
+-rw-r--r--   0      501       20     1589 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest
+-rw-r--r--   0      501       20    53916 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs
+-rw-r--r--   0      501       20     2216 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/segment_attributes.rs
+-rw-r--r--   0      501       20     1901 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/snippet_generator.rs
+-rw-r--r--   0      501       20    11168 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_document.rs
+-rw-r--r--   0      501       20     7439 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs
+-rw-r--r--   0      501       20     2162 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/config_proxy.rs
+-rw-r--r--   0      501       20     3093 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/core.rs
+-rw-r--r--   0      501       20     3512 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/file_proxy.rs
+-rw-r--r--   0      501       20      383 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/mod.rs
+-rw-r--r--   0      501       20     3335 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/configs/partial_proxy.rs
+-rw-r--r--   0      501       20     8009 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs
+-rw-r--r--   0      501       20     8014 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/caching_directory.rs
+-rw-r--r--   0      501       20     7015 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs
+-rw-r--r--   0      501       20     5258 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/external_requests.rs
+-rw-r--r--   0      501       20    17667 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs
+-rw-r--r--   0      501       20     2255 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/mod.rs
+-rw-r--r--   0      501       20     6756 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/directories/network_directory.rs
+-rw-r--r--   0      501       20     5192 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/errors.rs
+-rw-r--r--   0      501       20     2421 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/hyper_external_request.rs
+-rw-r--r--   0      501       20      742 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/lib.rs
+-rw-r--r--   0      501       20     1471 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs
+-rw-r--r--   0      501       20      960 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/label.rs
+-rw-r--r--   0      501       20       92 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/mod.rs
+-rw-r--r--   0      501       20      583 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/page_rank.rs
+-rw-r--r--   0      501       20     5490 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/aggregation.rs
+-rw-r--r--   0      501       20     2294 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/compression.rs
+-rw-r--r--   0      501       20     1068 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs
+-rw-r--r--   0      501       20      323 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      662 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/order.rs
+-rw-r--r--   0      501       20      582 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/snippet.rs
+-rw-r--r--   0      501       20      411 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/sort_by_field.rs
+-rw-r--r--   0      501       20     2048 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs
+-rw-r--r--   0      501       20     1538 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs
+-rw-r--r--   0      501       20      826 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs
+-rw-r--r--   0      501       20      218 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/mod.rs
+-rw-r--r--   0      501       20      480 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/safe_into_f64.rs
+-rw-r--r--   0      501       20     7908 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs
+-rw-r--r--   0      501       20      415 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      309 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/utils/random.rs
+-rw-r--r--   0      501       20     3165 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/utils/sync.rs
+-rw-r--r--   0      501       20      450 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-core/src/validators.rs
+-rw-r--r--   0        0        0      913 1970-01-01 00:00:00.000000 summa_embed-0.15.0/local_dependencies/summa-proto/Cargo.toml
+-rw-r--r--   0      501       20     1050 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/LICENSE
+-rw-r--r--   0      501       20     2262 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/build.rs
+-rwxr-xr-x   0      501       20      244 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/gen-docs.sh
+-rw-r--r--   0      501       20     2561 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/markdown.tmpl
+-rw-r--r--   0      501       20        0 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/__init__.py
+-rw-r--r--   0      501       20     1556 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/consumer_service.proto
+-rw-r--r--   0      501       20      393 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/dag_pb.proto
+-rw-r--r--   0      501       20    10377 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/index_service.proto
+-rw-r--r--   0      501       20     7125 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/query.proto
+-rw-r--r--   0      501       20      499 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/reflection_service.proto
+-rw-r--r--   0      501       20      867 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/search_service.proto
+-rw-r--r--   0      501       20      407 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/unixfs.proto
+-rw-r--r--   0      501       20       96 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/proto/utils.proto
+-rw-r--r--   0      501       20     2353 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/lib.rs
+-rw-r--r--   0      501       20     2683 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/collector.rs
+-rw-r--r--   0      501       20      212 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/mod.rs
+-rw-r--r--   0      501       20      424 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/query.rs
+-rw-r--r--   0      501       20      613 2023-05-27 21:56:58.000000 summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/score.rs
+-rw-r--r--   0        0        0      846 1970-01-01 00:00:00.000000 summa_embed-0.15.0/Cargo.toml
+-rw-r--r--   0      501       20      685 2023-05-27 21:56:58.000000 summa_embed-0.15.0/.gitignore
+-rw-r--r--   0      501       20      373 2023-05-27 21:56:58.000000 summa_embed-0.15.0/pyproject.toml
+-rw-r--r--   0      501       20     4324 2023-05-27 21:56:58.000000 summa_embed-0.15.0/src/lib.rs
+-rw-r--r--   0      501       20   100911 2023-05-27 21:57:10.000000 summa_embed-0.15.0/Cargo.lock
+-rw-r--r--   0        0        0      261 1970-01-01 00:00:00.000000 summa_embed-0.15.0/PKG-INFO
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/Cargo.toml` & `summa_embed-0.15.0/local_dependencies/summa-core/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-core"
-version = "0.14.3"
+version = "0.15.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa Core library"
 
 [lib]
 name = "summa_core"
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/LICENSE` & `summa_embed-0.15.0/local_dependencies/summa-core/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/collectors/reservoir_sampling_collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/custom_serializer.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/custom_serializer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/default_tokenizers.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/default_tokenizers.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/driver.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/driver.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/fruit_extractors.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/fruit_extractors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_holder.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_registry.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_registry.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/index_writer_holder.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/index_writer_holder.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/log_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/merge_policies/temporal_merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/mod.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/queries/exists_query.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/queries/exists_query.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/proto_query_parser.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.pest`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/query_parser/summa_ql.rs`

 * *Files 18% similar despite different names*

```diff
@@ -716,179 +716,179 @@
         QueryParser::new(schema, default_fields, &tokenizer_manager).expect("cannot create parser")
     }
 
     #[test]
     pub fn test_parser_base() {
         let query_parser = create_query_parser();
         let query = query_parser.parse_query("search engine");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, TermQuery(Term(type=Str, field=0, \"engine\")))] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })");
         let query = query_parser.parse_query("'search engine'");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"search\")), (1, Term(type=Str, field=0, \"engine\"))], slop: 0 })"
+            "Ok(PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"search\")), (1, Term(field=0, type=Str, \"engine\"))], slop: 0 })"
         );
     }
 
     #[test]
     pub fn test_parser_slop() {
         let query_parser = create_query_parser();
         let query = query_parser.parse_query("body:'search engine'~4");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(PhraseQuery { field: Field(1), phrase_terms: [(0, Term(type=Str, field=1, \"search\")), (1, Term(type=Str, field=1, \"engine\"))], slop: 4 })"
+            "Ok(PhraseQuery { field: Field(1), phrase_terms: [(0, Term(field=1, type=Str, \"search\")), (1, Term(field=1, type=Str, \"engine\"))], slop: 4 })"
         );
     }
 
     #[test]
     pub fn test_parser_fields() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:'search engine'")),
-            "Ok(PhraseQuery { field: Field(1), phrase_terms: [(0, Term(type=Str, field=1, \"search\")), (1, Term(type=Str, field=1, \"engine\"))], slop: 0 })"
+            "Ok(PhraseQuery { field: Field(1), phrase_terms: [(0, Term(field=1, type=Str, \"search\")), (1, Term(field=1, type=Str, \"engine\"))], slop: 0 })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("timestamp:10")),
-            "Ok(TermQuery(Term(type=I64, field=2, 10)))"
+            "Ok(TermQuery(Term(field=2, type=I64, 10)))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("title:search engine")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, TermQuery(Term(type=Str, field=0, \"engine\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("not_field:search engine")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"engine\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:10.0000/abcd.0123 ")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.0000/abcd.0123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:https://doi.org/10.0000/abcd.0123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"https://doi.org/10.0000/abcd.0123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"https://doi.org/10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:doi.org/10.0000/abcd.0123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"doi.org/10.0000/abcd.0123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"doi.org/10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.0000/978123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.0000/978123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/978123\")))"
         );
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/9781234567890")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=4, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(type=Str, field=3, \"10.0000/9781234567890\")), boost=3))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=4, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(type=Str, field=3, \"10.0000/978-12345-6789-0\")), boost=3))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=3, \"10.0000/978-12345-6789-0\"))), (Should, TermQuery(Term(type=Str, field=4, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(type=Str, field=3, \"10.0000/978-12345-6789-0.ch11\")), boost=3))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/cbo978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=3, \"10.0000/cbo978-12345-6789-0\"))), (Should, TermQuery(Term(type=Str, field=4, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(type=Str, field=3, \"10.0000/cbo978-12345-6789-0.ch11\")), boost=3))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/9781234567890")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/9781234567890\")), boost=3))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0\")), boost=3))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0\"))), (Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/978-12345-6789-0.ch11\")), boost=3))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("10.0000/cbo978-12345-6789-0.ch11")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=3, type=Str, \"10.0000/cbo978-12345-6789-0\"))), (Should, TermQuery(Term(field=4, type=Str, \"9781234567890\"))), (Should, Boost(query=TermQuery(Term(field=3, type=Str, \"10.0000/cbo978-12345-6789-0.ch11\")), boost=3))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("978-12345-6789-0")),
-            "Ok(TermQuery(Term(type=Str, field=4, \"9781234567890\")))"
+            "Ok(TermQuery(Term(field=4, type=Str, \"9781234567890\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("9781234567890")),
-            "Ok(TermQuery(Term(type=Str, field=4, \"9781234567890\")))"
+            "Ok(TermQuery(Term(field=4, type=Str, \"9781234567890\")))"
         );
-        assert_eq!(format!("{:?}", query_parser.parse_query("97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"97812\"))), (Should, TermQuery(Term(type=Str, field=0, \"34\"))), (Should, TermQuery(Term(type=Str, field=0, \"5678\"))), (Should, TermQuery(Term(type=Str, field=0, \"909\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"97812\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"5678\"))), (Should, TermQuery(Term(field=0, type=Str, \"909\")))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("isbns:97812-34-5678-90")),
-            "Ok(TermQuery(Term(type=Str, field=4, \"97812-34-5678-90\")))"
+            "Ok(TermQuery(Term(field=4, type=Str, \"97812-34-5678-90\")))"
         );
-        assert_eq!(format!("{:?}", query_parser.parse_query("123 97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"123\"))), (Should, TermQuery(Term(type=Str, field=0, \"97812\"))), (Should, TermQuery(Term(type=Str, field=0, \"34\"))), (Should, TermQuery(Term(type=Str, field=0, \"5678\"))), (Should, TermQuery(Term(type=Str, field=0, \"909\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("123 97812-34-5678-909")), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"123\"))), (Should, TermQuery(Term(field=0, type=Str, \"97812\"))), (Should, TermQuery(Term(field=0, type=Str, \"34\"))), (Should, TermQuery(Term(field=0, type=Str, \"5678\"))), (Should, TermQuery(Term(field=0, type=Str, \"909\")))] })");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.0000/cbo123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.0000/cbo123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/cbo123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi.org/10.0000/abcd.0123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.0000/abcd.0123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.0000/abcd.0123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.0000/abcd.0123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/abcd.0123\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("https://doi.org/10.0000/abcd.0123")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.0000/abcd.0123\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.0000/abcd.0123\")))"
         );
     }
 
     #[test]
     pub fn test_free_queries() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("Search Engines: The Ultimate, Only Guide!")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, TermQuery(Term(type=Str, field=0, \"engines\"))), (Should, TermQuery(Term(type=Str, field=0, \"the\"))), (Should, TermQuery(Term(type=Str, field=0, \"ultimate\"))), (Should, TermQuery(Term(type=Str, field=0, \"only\"))), (Should, TermQuery(Term(type=Str, field=0, \"guide\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engines\"))), (Should, TermQuery(Term(field=0, type=Str, \"the\"))), (Should, TermQuery(Term(field=0, type=Str, \"ultimate\"))), (Should, TermQuery(Term(field=0, type=Str, \"only\"))), (Should, TermQuery(Term(field=0, type=Str, \"guide\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("!! HI !! (SEARCH! ENGINES!")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"hi\"))), (Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, TermQuery(Term(type=Str, field=0, \"engines\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"hi\"))), (Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=0, type=Str, \"engines\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("`non closed")),
-            "Ok(PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"non\")), (1, Term(type=Str, field=0, \"closed\"))], slop: 0 })"
+            "Ok(PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"non\")), (1, Term(field=0, type=Str, \"closed\"))], slop: 0 })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("\"non closed")),
-            "Ok(PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"non\")), (1, Term(type=Str, field=0, \"closed\"))], slop: 0 })"
+            "Ok(PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"non\")), (1, Term(field=0, type=Str, \"closed\"))], slop: 0 })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("non closed`")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"non\"))), (Should, TermQuery(Term(type=Str, field=0, \"closed\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"non\"))), (Should, TermQuery(Term(field=0, type=Str, \"closed\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("non closed\"")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"non\"))), (Should, TermQuery(Term(type=Str, field=0, \"closed\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"non\"))), (Should, TermQuery(Term(field=0, type=Str, \"closed\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("title:(search ")),
-            "Ok(TermQuery(Term(type=Str, field=0, \"title\")))"
+            "Ok(TermQuery(Term(field=0, type=Str, \"title\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("title:(search -")),
-            "Ok(TermQuery(Term(type=Str, field=0, \"title\")))"
+            "Ok(TermQuery(Term(field=0, type=Str, \"title\")))"
         );
         assert_eq!(format!("{:?}", query_parser.parse_query("``")), "Ok(EmptyQuery)");
         assert_eq!(format!("{:?}", query_parser.parse_query("```")), "Ok(EmptyQuery)");
         assert_eq!(format!("{:?}", query_parser.parse_query(")(")), "Ok(EmptyQuery)");
         assert_eq!(
             format!("{:?}", query_parser.parse_query("(a)(b)`")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"a\"))), (Should, TermQuery(Term(type=Str, field=0, \"b\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"a\"))), (Should, TermQuery(Term(field=0, type=Str, \"b\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:'10.1182/blood.v53.1.19.bloodjournal53119'")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.1182/blood.v53.1.19.bloodjournal53119\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.1182/blood.v53.1.19.bloodjournal53119\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("doi:10.1182/blood.v53.1.19.bloodjournal53119")),
-            "Ok(TermQuery(Term(type=Str, field=3, \"10.1182/blood.v53.1.19.bloodjournal53119\")))"
+            "Ok(TermQuery(Term(field=3, type=Str, \"10.1182/blood.v53.1.19.bloodjournal53119\")))"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("10.10 10/10")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"10\"))), (Should, TermQuery(Term(type=Str, field=0, \"10\"))), (Should, TermQuery(Term(type=Str, field=0, \"10\"))), (Should, TermQuery(Term(type=Str, field=0, \"10\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"10\"))), (Should, TermQuery(Term(field=0, type=Str, \"10\"))), (Should, TermQuery(Term(field=0, type=Str, \"10\"))), (Should, TermQuery(Term(field=0, type=Str, \"10\")))] })"
         );
         let query_parser = create_complex_query_parser();
-        assert_eq!(format!("{:?}", query_parser.parse_query("\"search engines\"")), "Ok(BooleanQuery { subqueries: [(Should, PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"search\")), (1, Term(type=Str, field=0, \"engines\"))], slop: 0 }), (Should, PhraseQuery { field: Field(1), phrase_terms: [(0, Term(type=Str, field=1, \"search\")), (1, Term(type=Str, field=1, \"engines\"))], slop: 0 })] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("\"search engines\"")), "Ok(BooleanQuery { subqueries: [(Should, PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"search\")), (1, Term(field=0, type=Str, \"engines\"))], slop: 0 }), (Should, PhraseQuery { field: Field(1), phrase_terms: [(0, Term(field=1, type=Str, \"search\")), (1, Term(field=1, type=Str, \"engines\"))], slop: 0 })] })");
     }
 
     #[test]
     pub fn test_non_ascii() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:поисковые системы")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=1, \"поисковые\"))), (Should, TermQuery(Term(type=Str, field=0, \"системы\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=1, type=Str, \"поисковые\"))), (Should, TermQuery(Term(field=0, type=Str, \"системы\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("(поисковые системы)")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"поисковые\"))), (Should, TermQuery(Term(type=Str, field=0, \"системы\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"поисковые\"))), (Should, TermQuery(Term(field=0, type=Str, \"системы\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("поисковые: системы")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"поисковые\"))), (Should, TermQuery(Term(type=Str, field=0, \"системы\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"поисковые\"))), (Should, TermQuery(Term(field=0, type=Str, \"системы\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("healthcare cyber–physical system")),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"healthcare\"))), (Should, TermQuery(Term(type=Str, field=0, \"cyber\"))), (Should, TermQuery(Term(type=Str, field=0, \"physical\"))), (Should, TermQuery(Term(type=Str, field=0, \"system\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"healthcare\"))), (Should, TermQuery(Term(field=0, type=Str, \"cyber\"))), (Should, TermQuery(Term(field=0, type=Str, \"physical\"))), (Should, TermQuery(Term(field=0, type=Str, \"system\")))] })"
         );
     }
 
     #[test]
     pub fn test_regex() {
         let query_parser = create_query_parser();
         assert_eq!(
@@ -906,85 +906,85 @@
     }
 
     #[test]
     pub fn test_plus_minus() {
         let query_parser = create_query_parser();
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:+search -engine")),
-            "Ok(BooleanQuery { subqueries: [(Must, TermQuery(Term(type=Str, field=1, \"search\"))), (MustNot, TermQuery(Term(type=Str, field=0, \"engine\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Must, TermQuery(Term(field=1, type=Str, \"search\"))), (MustNot, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("body:+'search engine'")),
-            "Ok(BooleanQuery { subqueries: [(Must, PhraseQuery { field: Field(1), phrase_terms: [(0, Term(type=Str, field=1, \"search\")), (1, Term(type=Str, field=1, \"engine\"))], slop: 0 })] })"
+            "Ok(BooleanQuery { subqueries: [(Must, PhraseQuery { field: Field(1), phrase_terms: [(0, Term(field=1, type=Str, \"search\")), (1, Term(field=1, type=Str, \"engine\"))], slop: 0 })] })"
         );
         assert_eq!(
             format!("{:?}", query_parser.parse_query("+search +engine")),
-            "Ok(BooleanQuery { subqueries: [(Must, TermQuery(Term(type=Str, field=0, \"search\"))), (Must, TermQuery(Term(type=Str, field=0, \"engine\")))] })"
+            "Ok(BooleanQuery { subqueries: [(Must, TermQuery(Term(field=0, type=Str, \"search\"))), (Must, TermQuery(Term(field=0, type=Str, \"engine\")))] })"
         );
         let query_parser = create_complex_query_parser();
-        assert_eq!(format!("{:?}", query_parser.parse_query("+search +engine")), "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, TermQuery(Term(type=Str, field=1, \"search\")))] }), (Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"engine\"))), (Should, TermQuery(Term(type=Str, field=1, \"engine\")))] })] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("+search language:+ru")), "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, TermQuery(Term(type=Str, field=1, \"search\")))] }), (Must, TermQuery(Term(type=Str, field=3, \"ru\")))] })");
-        assert_eq!(format!("{:?}", query_parser.parse_query("+c++ language:+ru")), "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"c++\"))), (Should, TermQuery(Term(type=Str, field=1, \"c\")))] }), (Must, TermQuery(Term(type=Str, field=3, \"ru\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("+search +engine")), "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=1, type=Str, \"search\")))] }), (Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"engine\"))), (Should, TermQuery(Term(field=1, type=Str, \"engine\")))] })] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("+search language:+ru")), "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, TermQuery(Term(field=1, type=Str, \"search\")))] }), (Must, TermQuery(Term(field=3, type=Str, \"ru\")))] })");
+        assert_eq!(format!("{:?}", query_parser.parse_query("+c++ language:+ru")), "Ok(BooleanQuery { subqueries: [(Must, BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"c++\"))), (Should, TermQuery(Term(field=1, type=Str, \"c\")))] }), (Must, TermQuery(Term(field=3, type=Str, \"ru\")))] })");
     }
 
     #[test]
     pub fn test_parser_boostings() {
         let query_parser = create_query_parser();
         let query = query_parser.parse_query("search^2.0");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(Boost(query=TermQuery(Term(type=Str, field=0, \"search\")), boost=2))"
+            "Ok(Boost(query=TermQuery(Term(field=0, type=Str, \"search\")), boost=2))"
         );
         let query = query_parser.parse_query("'search engine'~3^2.0");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"search\")), (1, Term(type=Str, field=0, \"engine\"))], slop: 3 }, boost=2))"
+            "Ok(Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"search\")), (1, Term(field=0, type=Str, \"engine\"))], slop: 3 }, boost=2))"
         );
         let query = query_parser.parse_query("search engine^2.0");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"search\"))), (Should, Boost(query=TermQuery(Term(type=Str, field=0, \"engine\")), boost=2))] })"
+            "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"search\"))), (Should, Boost(query=TermQuery(Term(field=0, type=Str, \"engine\")), boost=2))] })"
         );
         let query = query_parser.parse_query("body:title^2.0");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(Boost(query=TermQuery(Term(type=Str, field=1, \"title\")), boost=2))"
+            "Ok(Boost(query=TermQuery(Term(field=1, type=Str, \"title\")), boost=2))"
         );
         let query = query_parser.parse_query("body:'title'^2.0");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(Boost(query=TermQuery(Term(type=Str, field=1, \"title\")), boost=2))"
+            "Ok(Boost(query=TermQuery(Term(field=1, type=Str, \"title\")), boost=2))"
         );
     }
 
     #[test]
     pub fn test_range_queries() {
         let query_parser = create_query_parser();
         let query = query_parser.parse_query("body:[aaa TO ccc]");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(RangeQuery { field: \"body\", value_type: Str, left_bound: Included([97, 97, 97]), right_bound: Included([99, 99, 99]), limit: None })"
+            "Ok(RangeQuery { field: \"body\", value_type: Str, lower_bound: Included([97, 97, 97]), upper_bound: Included([99, 99, 99]), limit: None })"
         );
         let query = query_parser.parse_query("body:[ a to  * ]");
         assert_eq!(
             format!("{:?}", query),
-            "Ok(RangeQuery { field: \"body\", value_type: Str, left_bound: Included([97]), right_bound: Unbounded, limit: None })"
+            "Ok(RangeQuery { field: \"body\", value_type: Str, lower_bound: Included([97]), upper_bound: Unbounded, limit: None })"
         );
         let query = query_parser.parse_query("timestamp:[ 1000 to 2000 ]");
-        assert_eq!(format!("{:?}", query), "Ok(RangeQuery { field: \"timestamp\", value_type: I64, left_bound: Included([128, 0, 0, 0, 0, 0, 3, 232]), right_bound: Included([128, 0, 0, 0, 0, 0, 7, 208]), limit: None })");
+        assert_eq!(format!("{:?}", query), "Ok(RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 3, 232]), upper_bound: Included([128, 0, 0, 0, 0, 0, 7, 208]), limit: None })");
         let query = query_parser.parse_query("timestamp:(-[1100 to 1200] [ 1000 to 2000 ] -1500 +3000)");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(MustNot, RangeQuery { field: \"timestamp\", value_type: I64, left_bound: Included([128, 0, 0, 0, 0, 0, 4, 76]), right_bound: Included([128, 0, 0, 0, 0, 0, 4, 176]), limit: None }), (Should, RangeQuery { field: \"timestamp\", value_type: I64, left_bound: Included([128, 0, 0, 0, 0, 0, 3, 232]), right_bound: Included([128, 0, 0, 0, 0, 0, 7, 208]), limit: None }), (MustNot, TermQuery(Term(type=I64, field=2, 1500))), (Must, TermQuery(Term(type=I64, field=2, 3000)))] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(MustNot, RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 4, 76]), upper_bound: Included([128, 0, 0, 0, 0, 0, 4, 176]), limit: None }), (Should, RangeQuery { field: \"timestamp\", value_type: I64, lower_bound: Included([128, 0, 0, 0, 0, 0, 3, 232]), upper_bound: Included([128, 0, 0, 0, 0, 0, 7, 208]), limit: None }), (MustNot, TermQuery(Term(field=2, type=I64, 1500))), (Must, TermQuery(Term(field=2, type=I64, 3000)))] })");
     }
 
     #[test]
     pub fn test_exact_phrase_promoter() {
         let mut query_parser = create_query_parser();
         query_parser.set_exact_match_promoter(proto::ExactMatchesPromoter { slop: 3, boost: Some(2.0) });
         let query = query_parser.parse_query("old school holy-wood");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(type=Str, field=0, \"old\"))), (Should, TermQuery(Term(type=Str, field=0, \"school\"))), (Should, TermQuery(Term(type=Str, field=0, \"holy\"))), (Should, TermQuery(Term(type=Str, field=0, \"wood\"))), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"old\")), (1, Term(type=Str, field=0, \"school\")), (2, Term(type=Str, field=0, \"holy\")), (3, Term(type=Str, field=0, \"wood\"))], slop: 3 }, boost=2))] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, TermQuery(Term(field=0, type=Str, \"old\"))), (Should, TermQuery(Term(field=0, type=Str, \"school\"))), (Should, TermQuery(Term(field=0, type=Str, \"holy\"))), (Should, TermQuery(Term(field=0, type=Str, \"wood\"))), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"old\")), (1, Term(field=0, type=Str, \"school\")), (2, Term(field=0, type=Str, \"holy\")), (3, Term(field=0, type=Str, \"wood\"))], slop: 3 }, boost=2))] })");
         let query = query_parser.parse_query("old^2.0 school");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(type=Str, field=0, \"old\")), boost=2)), (Should, TermQuery(Term(type=Str, field=0, \"school\")))] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(field=0, type=Str, \"old\")), boost=2)), (Should, TermQuery(Term(field=0, type=Str, \"school\")))] })");
         query_parser.set_field_boosts(HashMap::from_iter(vec![("title".to_string(), 3.0)].into_iter()));
         let query = query_parser.parse_query("old school");
-        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(type=Str, field=0, \"old\")), boost=3)), (Should, Boost(query=TermQuery(Term(type=Str, field=0, \"school\")), boost=3)), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(type=Str, field=0, \"old\")), (1, Term(type=Str, field=0, \"school\"))], slop: 3 }, boost=6))] })");
+        assert_eq!(format!("{:?}", query), "Ok(BooleanQuery { subqueries: [(Should, Boost(query=TermQuery(Term(field=0, type=Str, \"old\")), boost=3)), (Should, Boost(query=TermQuery(Term(field=0, type=Str, \"school\")), boost=3)), (Should, Boost(query=PhraseQuery { field: Field(0), phrase_terms: [(0, Term(field=0, type=Str, \"old\")), (1, Term(field=0, type=Str, \"school\"))], slop: 3 }, boost=6))] })");
     }
 }
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/segment_attributes.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/segment_attributes.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/snippet_generator.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/snippet_generator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_document.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_document.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/components/summa_tokenizer.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/components/summa_tokenizer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/config_proxy.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/config_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/core.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/core.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/file_proxy.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/file_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/configs/partial_proxy.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/configs/partial_proxy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/byte_range_cache.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/byte_range_cache.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/caching_directory.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/caching_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/debug_proxy_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/external_requests.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/external_requests.rs`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,21 @@
     pub headers: Vec<Header>,
 }
 
 #[derive(thiserror::Error, Debug)]
 pub enum RequestError {
     #[error("external: {0}")]
     External(String),
+    #[cfg(feature = "hyper-external-request")]
     #[error("http_error: {0}")]
     HttpError(#[from] hyper::http::Error),
+    #[cfg(feature = "hyper-external-request")]
     #[error("hyper_error: {0}")]
     HyperError(#[from] hyper::Error),
+    #[cfg(feature = "hyper-external-request")]
     #[error("invalid_method: {0}")]
     InvalidMethod(#[from] hyper::http::method::InvalidMethod),
     #[error("io_error: {0} {1}")]
     IoError(io::Error, PathBuf),
     #[error("not_found: {0}")]
     NotFound(PathBuf),
 }
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/hot_cache_directory.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/hot_cache_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/mod.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/mod.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/directories/network_directory.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/directories/network_directory.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/errors.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/errors.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/hyper_external_request.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/hyper_external_request.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 use hyper::client::HttpConnector;
 use hyper::{Client, Method, Request};
 use hyper_tls::HttpsConnector;
 use tracing::info;
 
 use crate::directories::{ExternalRequest, ExternalResponse, Header, RequestError};
-use crate::errors::Error;
 
 #[derive(Clone, Debug)]
 pub struct HyperExternalRequest {
     pub client: Client<HttpsConnector<HttpConnector>>,
     pub method: String,
     pub url: String,
     pub headers: Vec<Header>,
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/lib.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/cache_metrics.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/cache_metrics.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/metrics/label.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/metrics/label.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/page_rank.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/page_rank.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/compression.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/compression.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/merge_policy.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/merge_policy.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/order.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/order.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/proto_traits/snippet.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/proto_traits/snippet.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/eval_scorer_tweaker.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/fast_field_iterator.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/scorers/segment_eval_scorer.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-core/src/utils/sync.rs` & `summa_embed-0.15.0/local_dependencies/summa-core/src/utils/sync.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/Cargo.toml` & `summa_embed-0.15.0/local_dependencies/summa-proto/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "summa-proto"
-version = "0.25.0"
+version = "0.26.0"
 authors = ["Pasha Podolsky <ppodolsky@me.com>"]
 edition = "2021"
 license-file = "LICENSE"
 description = "Summa search server proto files"
 
 [lib]
 name = "summa_proto"
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/LICENSE` & `summa_embed-0.15.0/local_dependencies/summa-proto/LICENSE`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/build.rs` & `summa_embed-0.15.0/local_dependencies/summa-proto/build.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 fn main() -> Result<(), Box<dyn std::error::Error>> {
     std::env::set_var("PROTOC", protoc_bin_vendored::protoc_bin_path().unwrap());
     let files = &[
         "proto/consumer_service.proto",
+        "proto/dag_pb.proto",
         "proto/index_service.proto",
         "proto/query.proto",
         "proto/reflection_service.proto",
         "proto/search_service.proto",
+        "proto/unixfs.proto",
         "proto/utils.proto",
     ];
     let serde_default_structs = &[
+        "dag_pb.PBNode",
+        "dag_pb.PBLink",
         "summa.proto.HistogramAggregation",
         "summa.proto.IndexAttributes",
         "summa.proto.MoreLikeThisQuery",
         "summa.proto.PhraseQuery",
         "summa.proto.ReservoirSamplingCollector",
         "summa.proto.TermsAggregation",
         "summa.proto.TopDocsCollector",
+        "unixfs.Data",
     ];
     #[cfg(feature = "grpc")]
     build_tonic(files, serde_default_structs)?;
     #[cfg(not(feature = "grpc"))]
     build_prost(files, serde_default_structs)?;
     Ok(())
 }
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/markdown.tmpl` & `summa_embed-0.15.0/local_dependencies/summa-proto/markdown.tmpl`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/proto/consumer_service.proto` & `summa_embed-0.15.0/local_dependencies/summa-proto/proto/consumer_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/proto/index_service.proto` & `summa_embed-0.15.0/local_dependencies/summa-proto/proto/index_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/proto/query.proto` & `summa_embed-0.15.0/local_dependencies/summa-proto/proto/query.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/proto/search_service.proto` & `summa_embed-0.15.0/local_dependencies/summa-proto/proto/search_service.proto`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/src/lib.rs` & `summa_embed-0.15.0/local_dependencies/summa-proto/src/lib.rs`

 * *Files 9% similar despite different names*

```diff
@@ -45,12 +45,18 @@
 ///         .await
 ///         .expect("cannot search");
 /// }
 /// ```
 pub mod proto {
     #[cfg(feature = "grpc")]
     pub const FILE_DESCRIPTOR_SET: &[u8] = tonic::include_file_descriptor_set!("summa");
+    pub mod dag_pb {
+        include!(concat!(env!("OUT_DIR"), "/dag_pb.rs"));
+    }
+    pub mod unixfs {
+        include!(concat!(env!("OUT_DIR"), "/unixfs.rs"));
+    }
     #[cfg(feature = "grpc")]
     tonic::include_proto!("summa.proto");
     #[cfg(not(feature = "grpc"))]
     include!(concat!(env!("OUT_DIR"), "/summa.proto.rs"));
 }
```

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/collector.rs` & `summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/collector.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/local_dependencies/summa-proto/src/proto_traits/score.rs` & `summa_embed-0.15.0/local_dependencies/summa-proto/src/proto_traits/score.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/Cargo.toml` & `summa_embed-0.15.0/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [package]
 name = "summa-embed-py"
-version = "0.1.3"
+version = "0.15.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "summa_embed"
 crate-type = ["cdylib"]
 
 [dependencies]
 futures = "0.3"
 pyo3 = { version = "0.18", features = ["serde"] }
 pyo3-asyncio = { version =  "0.18", features = ["attributes", "tokio-runtime"] }
 pythonize = "0.18"
 serde_json = "1.0"
-summa-core = { version = "0.14.3", path = "local_dependencies/summa-core", default_features = false, features = ["hyper-external-request", "tokio-rt"] }
+summa-core = { version = "0.15.0", path = "local_dependencies/summa-core", default_features = false, features = ["fs", "hyper-external-request", "tokio-rt"] }
 summa-proto = { path = "local_dependencies/summa-proto" }
 tantivy = { git = "https://github.com/izihawa/tantivy", branch = "feature/summa", default_features = false, features = ["quickwit", "zstd-compression"] }
 tokio = { version = "1.25", default_features = false }
```

### Comparing `summa_embed-0.1.3/.gitignore` & `summa_embed-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/src/lib.rs` & `summa_embed-0.15.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `summa_embed-0.1.3/Cargo.lock` & `summa_embed-0.15.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -28,26 +28,26 @@
  "cfg-if",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "0.7.20"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc936419f96fa211c1b9166887b38e5e40b19958e5b895be7c1f93adec7071ac"
+checksum = "67fc08ce920c31afb70f013dcce1bfc3a3195de6a228474e45e1f145b36f8d04"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
-version = "0.3.1"
+version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6342bd4f5a1205d7f41e94a41a901f5647c938cdfa96036338e8533c9d6c2450"
+checksum = "0ca84f3628370c59db74ee214b3263d58f9aadd9b4fe7e711fd87dc452b7f163"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "is-terminal",
@@ -86,25 +86,37 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.70"
+version = "1.0.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7de8ce5e0f9f8d88245311066a578d72b7af3e7088f32783804676302df237e4"
+checksum = "9c7d0618f0e0b7e8ff11427422b64564d5fb0be1940354bfe2e0529b18a9d9b8"
 
 [[package]]
 name = "arc-swap"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
 
 [[package]]
+name = "arrayref"
+version = "0.3.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6b4930d2cb77ce62f89ee5d5289b4ac049559b1c45539271f5ed4fdc7db34545"
+
+[[package]]
+name = "arrayvec"
+version = "0.7.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8da52d66c7071e2e3fa2a1e5c6d088fec47b593032b254f5e980de8ea54454d6"
+
+[[package]]
 name = "async-broadcast"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7c48ccdbf6ca6b121e0f586cbc0e73ae440e56c67c30fa0873b4e110d9c26d2b"
 dependencies = [
  "event-listener",
  "futures-core",
@@ -125,39 +137,39 @@
 name = "async-stream-impl"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "axum"
-version = "0.6.17"
+version = "0.6.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b70caf9f1b0c045f7da350636435b775a9733adf2df56e8aa2a29210fbc335d4"
+checksum = "f8175979259124331c1d7bf6586ee7e0da434155e4b2d48ec2c8386281d8df39"
 dependencies = [
  "async-trait",
  "axum-core",
  "bitflags",
  "bytes",
  "futures-util",
  "http",
@@ -191,24 +203,39 @@
  "mime",
  "rustversion",
  "tower-layer",
  "tower-service",
 ]
 
 [[package]]
+name = "base-x"
+version = "0.2.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4cbbc9d0964165b47557570cce6c952866c2678457aca742aafc9fb771d30270"
+
+[[package]]
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
+
+[[package]]
+name = "bincode"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b1f45e9417d87227c7a56d22e471c6206462cba514c7590c09aff4cf6d1ddcad"
+dependencies = [
+ "serde",
+]
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
@@ -218,27 +245,74 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8c7d2ac73c167c06af4a5f37e6e59d84148d57ccbe4480b76f0273eefea82d7"
 dependencies = [
  "crunchy",
 ]
 
 [[package]]
+name = "bitvec"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
+dependencies = [
+ "funty",
+ "radium",
+ "tap",
+ "wyz",
+]
+
+[[package]]
+name = "blake2b_simd"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c2f0dc9a68c6317d884f97cc36cf5a3d20ba14ce404227df55e1af708ab04bc"
+dependencies = [
+ "arrayref",
+ "arrayvec",
+ "constant_time_eq",
+]
+
+[[package]]
+name = "blake2s_simd"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6637f448b9e61dfadbdcbae9a885fadee1f3eaffb1f8d3c1965d3ade8bdfd44f"
+dependencies = [
+ "arrayref",
+ "arrayvec",
+ "constant_time_eq",
+]
+
+[[package]]
+name = "blake3"
+version = "1.3.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42ae2468a89544a466886840aa467a25b766499f4f04bf7d9fcd10ecee9fccef"
+dependencies = [
+ "arrayref",
+ "arrayvec",
+ "cc",
+ "cfg-if",
+ "constant_time_eq",
+]
+
+[[package]]
 name = "block-buffer"
 version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
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
 
@@ -266,41 +340,67 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "cid"
+version = "0.9.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b9b68e3193982cd54187d71afdb2a271ad4cf8af157858e9cb911b91321de143"
+dependencies = [
+ "core2",
+ "multibase",
+ "multihash 0.17.0",
+ "serde",
+ "unsigned-varint",
+]
+
+[[package]]
+name = "cid"
+version = "0.10.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fd94671561e36e4e7de75f753f577edafb0e7c05d6e4547229fdf7938fbcd2c3"
+dependencies = [
+ "core2",
+ "multibase",
+ "multihash 0.18.1",
+ "serde",
+ "unsigned-varint",
+]
+
+[[package]]
 name = "clap"
-version = "4.2.4"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "956ac1f6381d8d82ab4684768f89c0ea3afe66925ceadb4eeb3fc452ffc55d62"
+checksum = "93aae7a4192245f70fe75dd9157fc7b4a5bf53e88d30bd4396f7d8f9284d5acc"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.2.4"
+version = "4.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84080e799e54cff944f4b4a4b0e71630b0e0443b25b985175c7dddc1a859b749"
+checksum = "4f423e341edefb78c9caba2d9c7f7687d0e72e89df3ce3394554754393ac3990"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "once_cell",
  "strsim",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.4.1"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a2dd5a6fe8c6e3502f568a6353e5273bbb15193ad9a89e457b9970798efbea1"
+checksum = "2da6da31387c7e4ef160ffab6d5e7f00c42626fe39aea70a7b0f1773f7dd6c1b"
 
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
@@ -339,14 +439,20 @@
 checksum = "a06aeb73f470f66dcdbf7223caeebb85984942f22f1adb2a088cf9668146bbbc"
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
+name = "constant_time_eq"
+version = "0.2.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "13418e745008f7349ec7e449155f419a61b92b58a99cc3616942b926825ec76b"
+
+[[package]]
 name = "core-foundation"
 version = "0.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
 dependencies = [
  "core-foundation-sys",
  "libc",
@@ -355,14 +461,23 @@
 [[package]]
 name = "core-foundation-sys"
 version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
+name = "core2"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b49ba7ef1ad6107f8824dbe97de947cbaac53c44e7f9756a1fba0d37c1eec505"
+dependencies = [
+ "memchr",
+]
+
+[[package]]
 name = "cpufeatures"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
@@ -476,15 +591,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "907076dfda823b0b36d2a1bb5f90c96660a5bbcd7729e10727f07858f22c4edc"
 dependencies = [
  "cfg-if",
  "hashbrown 0.12.3",
  "lock_api",
  "once_cell",
- "parking_lot_core",
+ "parking_lot_core 0.9.7",
+]
+
+[[package]]
+name = "data-encoding"
+version = "2.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c2e66c9d817f1720209181c316d28635c050fa304f9c79e47a520882661b7308"
+
+[[package]]
+name = "data-encoding-macro"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c904b33cc60130e1aeea4956ab803d08a3f4a0ca82d64ed757afac3891f2bb99"
+dependencies = [
+ "data-encoding",
+ "data-encoding-macro-internal",
+]
+
+[[package]]
+name = "data-encoding-macro-internal"
+version = "0.1.11"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8fdf3fce3ce863539ec1d7fd1b6dcc3c645663376b43ed376bbf887733e4f772"
+dependencies = [
+ "data-encoding",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "derive_builder"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8d67778784b508018359cbc8696edb3db78160bab2c2a28ba7f56ef6932997f8"
@@ -512,17 +653,17 @@
 dependencies = [
  "derive_builder_core",
  "syn 1.0.109",
 ]
 
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
 name = "dlv-list"
@@ -540,25 +681,14 @@
 name = "either"
 version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "errno"
-version = "0.2.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f639046355ee4f37944e44f60642c6f3a7efa3cf6b78c78a0d989a8ce6c396a1"
-dependencies = [
- "errno-dragonfly",
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "errno"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4bcfec3a70f97c962c307b2d2c56e358cf1d00b558d74262b5f929ee8cc7e73a"
 dependencies = [
  "errno-dragonfly",
  "libc",
  "windows-sys 0.48.0",
@@ -581,15 +711,15 @@
 checksum = "0206175f82b8d6bf6652ff7d71a1e27fd2e4efde587fd368662814d6ec1d9ce0"
 
 [[package]]
 name = "examples"
 version = "0.0.0"
 dependencies = [
  "serde_json",
- "summa-proto",
+ "summa-proto 0.26.0",
  "tokio",
  "tonic",
 ]
 
 [[package]]
 name = "fail"
 version = "0.5.1"
@@ -610,33 +740,51 @@
 [[package]]
 name = "fasteval2"
 version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "693f2d239802e51c2b7381927eef77061c64fbef1cf2582ab66ffb326c1b52f8"
 
 [[package]]
+name = "fastmurmur3"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d922f481ae01f2a3f1fff7b9e0e789f18f0c755a38ec983a3e6f37762cdcc2a2"
+
+[[package]]
 name = "fastrand"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
+name = "filetime"
+version = "0.2.21"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5cbc844cecaee9d4443931972e1289c8ff485cb4cc2767cb03ca139ed6885153"
+dependencies = [
+ "cfg-if",
+ "libc",
+ "redox_syscall 0.2.16",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "fixedbitset"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ce7134b9999ecaf8bcd65542e436736ef32ddca1b3e06094cb6ec5755203b80"
 
 [[package]]
 name = "flate2"
-version = "1.0.25"
+version = "1.0.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8a2db397cb1c8772f31494cb8917e48cd1e64f0fa7efac59fbd741a0a8ce841"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "fnv"
@@ -656,31 +804,66 @@
 [[package]]
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
-name = "fs4"
-version = "0.6.3"
+name = "format-bytes"
+version = "0.3.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "48942366ef93975da38e175ac9e10068c6fc08ca9e85930d4f098f4d5b14c2fd"
+dependencies = [
+ "format-bytes-macros",
+]
+
+[[package]]
+name = "format-bytes-macros"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8ea55201cc351fdb478217c0fb641b59813da9b4efe4c414a9d8f989a657d149"
+checksum = "203aadebefcc73d12038296c228eabf830f99cba991b0032adf20e9fa6ce7e4f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
+name = "fs2"
+version = "0.4.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9564fc758e15025b46aa6643b1b77d047d1a56a1aea6e01002ac0c7026876213"
 dependencies = [
  "libc",
- "rustix 0.35.13",
  "winapi",
 ]
 
 [[package]]
+name = "fs4"
+version = "0.6.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a7f5b6908aecca5812a4569056285e58c666588c9573ee59765bf1d3692699e2"
+dependencies = [
+ "rustix",
+ "windows-sys 0.48.0",
+]
+
+[[package]]
 name = "fuchsia-cprng"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a06f77d526c1a601b7c4cdd98f54b5eaabffc14d5f2f0296febdc7f357c6d3ba"
 
 [[package]]
+name = "funty"
+version = "2.0.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
+
+[[package]]
 name = "futures"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23342abe12aba583913b2e62f22225ff9c950774065e4bfb61a19cd9770fec40"
 dependencies = [
  "futures-channel",
  "futures-core",
@@ -728,15 +911,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -762,14 +945,23 @@
  "memchr",
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
+name = "fxhash"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
+dependencies = [
+ "byteorder",
+]
+
+[[package]]
 name = "generator"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3e123d9ae7c02966b4d892e550bdc32164f05853cd40ab570650ad600596a8a"
 dependencies = [
  "cc",
  "libc",
@@ -799,17 +991,17 @@
  "libc",
  "wasi",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.18"
+version = "0.3.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17f8a914c2987b688368b5138aa05321db91f4090cf26118185672ad588bce21"
+checksum = "d357c7ae988e7d2182f7d7871d0b963962420b0678b0997ce7de72001aeab782"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -1017,38 +1209,63 @@
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "io-lifetimes"
-version = "0.7.5"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "59ce5ef949d49ee85593fc4d3f3f95ad61657076395cbbce23e2121fc5542074"
-
-[[package]]
-name = "io-lifetimes"
-version = "1.0.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c66c74d2ae7e79a5a8f7ac924adbe38ee42a859c6539ad869eb51f0b52dc220"
+checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
 dependencies = [
  "hermit-abi 0.3.1",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "ipfs-hamt-directory"
+version = "0.1.0"
+dependencies = [
+ "anyhow",
+ "bincode",
+ "bitvec",
+ "cid 0.10.1",
+ "fastmurmur3",
+ "format-bytes",
+ "minicbor",
+ "multihash 0.18.1",
+ "prost",
+ "rayon",
+ "rust-unixfs",
+ "serde_json",
+ "sled",
+ "summa-proto 0.26.0 (registry+https://github.com/rust-lang/crates.io-index)",
+ "unsigned-varint",
+]
+
+[[package]]
+name = "ipfs-hamt-directory-py"
+version = "0.1.0"
+dependencies = [
+ "cid 0.10.1",
+ "ipfs-hamt-directory",
+ "multihash 0.18.1",
+ "pyo3",
+]
+
+[[package]]
 name = "is-terminal"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adcf93614601c8129ddf72e2d5633df827ba6551541c6d8c59520a371475be1f"
 dependencies = [
  "hermit-abi 0.3.1",
- "io-lifetimes 1.0.10",
- "rustix 0.37.15",
+ "io-lifetimes",
+ "rustix",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1081,17 +1298,17 @@
 checksum = "936cfd212a0155903bcbc060e316fb6cc7cbf2e1907329391ebadc1fe0ce77c2"
 dependencies = [
  "libc",
 ]
 
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
 name = "json5"
 version = "0.4.1"
@@ -1100,36 +1317,133 @@
 dependencies = [
  "pest",
  "pest_derive",
  "serde",
 ]
 
 [[package]]
+name = "keccak"
+version = "0.1.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8f6d5ed8676d904364de097082f4e7d240b571b67989ced0240f08b7f966f940"
+dependencies = [
+ "cpufeatures",
+]
+
+[[package]]
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "levenshtein_automata"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2cdeb66e45e9f36bfad5bbdb4d2384e70936afbee843c6f6543f0c551ebb25"
 
 [[package]]
 name = "libc"
-version = "0.2.142"
+version = "0.2.144"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
+
+[[package]]
+name = "libipld"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a20e38e0ad9a2fd600476691fa0780421931a198279985e398a3a0851903e1b2"
+dependencies = [
+ "fnv",
+ "libipld-cbor",
+ "libipld-cbor-derive",
+ "libipld-core",
+ "libipld-json",
+ "libipld-macro",
+ "libipld-pb",
+ "log",
+ "multihash 0.17.0",
+ "thiserror",
+]
+
+[[package]]
+name = "libipld-cbor"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4b75370e27e0745910a9991c83f365cdae58027acf0502aa7987ac538a8a4744"
+dependencies = [
+ "byteorder",
+ "libipld-core",
+ "thiserror",
+]
+
+[[package]]
+name = "libipld-cbor-derive"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4515686b6bffd663a1fbdd87408ced5b612751910a9e309042e9efef9dbdb324"
+dependencies = [
+ "proc-macro-crate",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "synstructure",
+]
+
+[[package]]
+name = "libipld-core"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b7a704ba3b25dee9e7a2361fae2c7c19defae2a92e69ae96ffb203996705cd7c"
+dependencies = [
+ "anyhow",
+ "cid 0.9.0",
+ "core2",
+ "multibase",
+ "multihash 0.17.0",
+ "thiserror",
+]
+
+[[package]]
+name = "libipld-json"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "fc549d7c70f9a401031fcb6d3bf7eccfe91bcad938f7485f71ee8ba9f79c1e79"
+dependencies = [
+ "libipld-core",
+ "multihash 0.17.0",
+ "serde",
+ "serde_json",
+]
+
+[[package]]
+name = "libipld-macro"
+version = "0.15.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d4c7ccd89e54f2796cf3f99aabeea7a7751d418df504926544f28348d3c890c7"
+dependencies = [
+ "libipld-core",
+]
+
+[[package]]
+name = "libipld-pb"
+version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
+checksum = "dd84ee8b7e283c81b28ecf46e07c31a524a2cd35ec4e87833733a18218c17ccb"
+dependencies = [
+ "libipld-core",
+ "prost",
+ "thiserror",
+]
 
 [[package]]
 name = "libz-sys"
-version = "1.1.8"
+version = "1.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9702761c3935f8cc2f101793272e202c72b99da8f4224a19ddcf1279a6450bbf"
+checksum = "56ee889ecc9568871456d42f603d6a0ce59ff328d291063a45cbdf0036baf6db"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1137,23 +1451,17 @@
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.0.46"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d4d2456c373231a208ad294c33dc5bff30051eafd954cd4caae83a712b12854d"
-
-[[package]]
-name = "linux-raw-sys"
-version = "0.3.4"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "36eb31c1778188ae1e64398743890d0877fef36d11521ac60406b42016e8c2cf"
+checksum = "ef53942eb7bf7ff43a617b3e2c1c4a5ecf5944a7c1bc12d7ee39bbb15e5c1519"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -1228,17 +1536,17 @@
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memmap2"
-version = "0.5.10"
+version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "83faa42c0a078c393f6b29d5db232d8be22776a891f8f56e5284faee4a20b327"
+checksum = "6d28bba84adfe6646737845bc5ebbfa2c08424eb1c37e94a1fd2a82adb56a872"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.8.0"
@@ -1251,24 +1559,44 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "minicbor"
+version = "0.19.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d7005aaf257a59ff4de471a9d5538ec868a21586534fff7f85dd97d4043a6139"
+dependencies = [
+ "minicbor-derive",
+]
+
+[[package]]
+name = "minicbor-derive"
+version = "0.13.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1154809406efdb7982841adb6311b3d095b46f78342dd646736122fe6b19e267"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+]
+
+[[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.6.2"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b275950c28b37e794e8c55d88aeb5e139d0ce23fdbbeda68f8d7174abdf9e8fa"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
 version = "0.8.6"
@@ -1278,14 +1606,73 @@
  "libc",
  "log",
  "wasi",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
+name = "multibase"
+version = "0.9.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9b3539ec3c1f04ac9748a260728e855f261b4977f5c3406612c884564f329404"
+dependencies = [
+ "base-x",
+ "data-encoding",
+ "data-encoding-macro",
+]
+
+[[package]]
+name = "multihash"
+version = "0.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "835d6ff01d610179fbce3de1694d007e500bf33a7f29689838941d6bf783ae40"
+dependencies = [
+ "blake2b_simd",
+ "blake2s_simd",
+ "blake3",
+ "core2",
+ "digest",
+ "multihash-derive",
+ "sha2",
+ "sha3",
+ "unsigned-varint",
+]
+
+[[package]]
+name = "multihash"
+version = "0.18.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "cfd8a792c1694c6da4f68db0a9d707c72bd260994da179e6030a5dcee00bb815"
+dependencies = [
+ "blake2b_simd",
+ "blake2s_simd",
+ "blake3",
+ "core2",
+ "digest",
+ "multihash-derive",
+ "sha2",
+ "sha3",
+ "unsigned-varint",
+]
+
+[[package]]
+name = "multihash-derive"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1d6d4752e6230d8ef7adf7bd5d8c4b1f6561c1014c5ba9a37445ccefe18aa1db"
+dependencies = [
+ "proc-macro-crate",
+ "proc-macro-error",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "synstructure",
+]
+
+[[package]]
 name = "multimap"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e5ce46fe64a9d73be07dcbe690a38ce1b293be448fd8ce1e6c1b8062c9f72c6a"
 
 [[package]]
 name = "murmurhash32"
@@ -1396,15 +1783,15 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
@@ -1505,27 +1892,52 @@
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b15813163c1d831bf4a13c3610c05c0d03b39feb07f7e09fa234dac9b15aaf39"
 
 [[package]]
 name = "ownedbytes"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "stable_deref_trait",
 ]
 
 [[package]]
 name = "parking_lot"
+version = "0.11.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7d17b78036a60663b797adeaee46f5c9dfebb86948d1255007a1d6be0271ff99"
+dependencies = [
+ "instant",
+ "lock_api",
+ "parking_lot_core 0.8.6",
+]
+
+[[package]]
+name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
- "parking_lot_core",
+ "parking_lot_core 0.9.7",
+]
+
+[[package]]
+name = "parking_lot_core"
+version = "0.8.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "60a2cfe6f0ad2bfc16aefa463b497d5c7a5ecd44a23efa72aa342d90177356dc"
+dependencies = [
+ "cfg-if",
+ "instant",
+ "libc",
+ "redox_syscall 0.2.16",
+ "smallvec",
+ "winapi",
 ]
 
 [[package]]
 name = "parking_lot_core"
 version = "0.9.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9069cbb9f99e3a5083476ccb29ceb1de18b9118cafa53e90c9551235de2b9521"
@@ -1535,26 +1947,26 @@
  "redox_syscall 0.2.16",
  "smallvec",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "path-absolutize"
-version = "3.0.14"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f1d4993b16f7325d90c18c3c6a3327db7808752db8d208cea0acee0abd52c52"
+checksum = "43eb3595c63a214e1b37b44f44b0a84900ef7ae0b4c5efce59e123d246d7a0de"
 dependencies = [
  "path-dedot",
 ]
 
 [[package]]
 name = "path-dedot"
-version = "3.0.18"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a81540d94551664b72b72829b12bd167c73c9d25fbac0e04fafa8023f7e4901"
+checksum = "9d55e486337acb9973cdea3ec5638c1b3bcb22e573b2b7b41969e0c744d5a15e"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "pathdiff"
 version = "0.2.1"
@@ -1565,50 +1977,50 @@
 name = "percent-encoding"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "478c572c3d73181ff3c2539045f6eb99e5491218eae919370993b890cdbdd98e"
 
 [[package]]
 name = "pest"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b1403e8401ad5dedea73c626b99758535b342502f8d1e361f4a2dd952749122"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_derive"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "be99c4c1d2fc2769b1d00239431d711d08f6efedcecb8b6e30707160aee99c15"
+checksum = "6b79d4c71c865a25a4322296122e3924d30bc8ee0834c8bfc8b95f7f054afbfb"
 dependencies = [
  "pest",
  "pest_generator",
 ]
 
 [[package]]
 name = "pest_generator"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e56094789873daa36164de2e822b3888c6ae4b4f9da555a1103587658c805b1e"
+checksum = "6c435bf1076437b851ebc8edc3a18442796b30f1728ffea6262d59bbe28b077e"
 dependencies = [
  "pest",
  "pest_meta",
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.7"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6733073c7cff3d8459fda0e42f13a047870242aed8b509fe98000928975f359e"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
 dependencies = [
  "once_cell",
  "pest",
  "sha2",
 ]
 
 [[package]]
@@ -1619,30 +2031,30 @@
 dependencies = [
  "fixedbitset",
  "indexmap",
 ]
 
 [[package]]
 name = "pin-project"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad29a609b6bcd67fee905812e544992d216af9d755757c05ed2d0e15a74c6ecc"
+checksum = "c95a7476719eab1e366eaf73d0260af3021184f18177925b07f54b30089ceead"
 dependencies = [
  "pin-project-internal",
 ]
 
 [[package]]
 name = "pin-project-internal"
-version = "1.0.12"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "069bdb1e05adc7a8990dce9cc75370895fbe4e3d58b9b73bf1aee56359344a55"
+checksum = "39407670928234ebc5e6e580247dd567ad73a3578460c5990f9503df207e8f07"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "pin-project-lite"
 version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e0a7ae3ac2f1173085d398531c705756c94a4c56843785df85a60c1a0afac116"
@@ -1651,17 +2063,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.26"
+version = "0.3.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6ac9a59f73473f1b8d852421e59e64809f025994837ef743615c6d0c5b305160"
+checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
 
 [[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
@@ -1673,42 +2085,66 @@
 dependencies = [
  "proc-macro2",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "proc-macro-crate"
-version = "1.3.1"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
+checksum = "e17d47ce914bf4de440332250b0edd23ce48c005f59fab39d3335866b114f11a"
 dependencies = [
- "once_cell",
- "toml_edit",
+ "thiserror",
+ "toml",
+]
+
+[[package]]
+name = "proc-macro-error"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
+dependencies = [
+ "proc-macro-error-attr",
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "version_check",
+]
+
+[[package]]
+name = "proc-macro-error-attr"
+version = "1.0.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a1be40180e52ecc98ad80b184934baf3d0d29f979574e439af5a55274b35f869"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "version_check",
 ]
 
 [[package]]
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
 name = "prometheus"
 version = "0.13.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "449811d15fbdf5ceb5c1144416066429cf82316e2ec8ce0c1f6f8a02e7bbcf8c"
 dependencies = [
  "cfg-if",
  "fnv",
  "lazy_static",
  "memchr",
- "parking_lot",
+ "parking_lot 0.12.1",
  "protobuf",
  "thiserror",
 ]
 
 [[package]]
 name = "prost"
 version = "0.11.9"
@@ -1825,15 +2261,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "serde",
  "unindent",
 ]
 
@@ -1912,23 +2348,38 @@
 checksum = "9a0e1bbcd2a3856284bf4f4ef09ccb1157e9467847792754556f153ea3fe6b42"
 dependencies = [
  "pyo3",
  "serde",
 ]
 
 [[package]]
+name = "quick-protobuf"
+version = "0.8.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d6da84cc204722a989e01ba2f6e1e276e190f22263d0cb6ce8526fcdb0d2e1f"
+dependencies = [
+ "byteorder",
+]
+
+[[package]]
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
+name = "radium"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "dc33ff2d4973d518d823d61aa239014831e521c75da58e3df4840d3f47749d09"
+
+[[package]]
 name = "rand"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "552840b97013b1a26992c11eac34bdd778e464601a4c2054b5f0bff7c6761293"
 dependencies = [
  "fuchsia-cprng",
  "libc",
@@ -2020,17 +2471,17 @@
  "serde_json",
  "slab",
  "tokio",
 ]
 
 [[package]]
 name = "rdkafka-sys"
-version = "4.3.0+1.9.2"
+version = "4.4.0+1.9.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d222a401698c7f2010e3967353eae566d9934dcda49c29910da922414ab4e3f4"
+checksum = "87ac9d87c3aba1748e3112318459f2ac8bff80bfff7359e338e0463549590249"
 dependencies = [
  "libc",
  "libz-sys",
  "num_enum",
  "pkg-config",
 ]
 
@@ -2059,19 +2510,19 @@
 checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.8.1"
+version = "1.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af83e617f331cc6ae2da5443c602dfa5af81e517212d9d611a5b3ba1777b5370"
+checksum = "81ca098a9821bd52d6b24fd8b10bd081f47d39c22778cafaa75a2857a62c6390"
 dependencies = [
- "regex-syntax 0.7.1",
+ "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
@@ -2083,17 +2534,17 @@
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
 name = "regex-syntax"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a5996294f19bd3aae0453a862ad728f60e6600695733dd5df01da90c54363a3c"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "remove_dir_all"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3acd125665422973a33ac9d3dd2df85edad0f4ae9b00dafb1a05e43a9f5ef8e7"
 dependencies = [
@@ -2137,44 +2588,43 @@
 checksum = "e46a2036019fdb888131db7a4c847a1063a7493f971ed94ea82c67eada63ca54"
 dependencies = [
  "serde",
  "serde_derive",
 ]
 
 [[package]]
-name = "rustc-hash"
-version = "1.1.0"
+name = "rust-unixfs"
+version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
+checksum = "3901fadba88ea7f088778241c0e16a5508ea7e0828e962310776166dd4be8fc3"
+dependencies = [
+ "either",
+ "filetime",
+ "libipld",
+ "quick-protobuf",
+ "sha2",
+]
 
 [[package]]
-name = "rustix"
-version = "0.35.13"
+name = "rustc-hash"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "727a1a6d65f786ec22df8a81ca3121107f235970dc1705ed681d3e6e8b9cd5f9"
-dependencies = [
- "bitflags",
- "errno 0.2.8",
- "io-lifetimes 0.7.5",
- "libc",
- "linux-raw-sys 0.0.46",
- "windows-sys 0.42.0",
-]
+checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
 name = "rustix"
-version = "0.37.15"
+version = "0.37.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0661814f891c57c930a610266415528da53c4933e6dea5fb350cbfe048a9ece"
+checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
 dependencies = [
  "bitflags",
- "errno 0.3.1",
- "io-lifetimes 1.0.10",
+ "errno",
+ "io-lifetimes",
  "libc",
- "linux-raw-sys 0.3.4",
+ "linux-raw-sys",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2252,40 +2702,40 @@
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
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
 name = "serde"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
+checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.4.5"
@@ -2314,21 +2764,21 @@
 dependencies = [
  "half",
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.160"
+version = "1.0.163"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
+checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
 version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
@@ -2369,14 +2819,24 @@
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
+name = "sha3"
+version = "0.10.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "75872d278a8f37ef87fa0ddbda7802605cb18344497949862c0d4dcb291eba60"
+dependencies = [
+ "digest",
+ "keccak",
+]
+
+[[package]]
 name = "sharded-slab"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "900fba806f70c630b0a382d0d825e17a0f19fcd059a2ade1ff237bcddf446b31"
 dependencies = [
  "lazy_static",
 ]
@@ -2387,23 +2847,48 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "sketches-ddsketch"
+version = "0.2.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "68a406c1882ed7f29cd5e248c9848a80e7cb6ae0fea82346d2746f2f941c07e1"
+dependencies = [
+ "serde",
+]
+
+[[package]]
 name = "slab"
 version = "0.4.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6528351c9bc8ab22353f9d776db39a20288e8d6c37ef8cfe3317cf875eecfc2d"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
+name = "sled"
+version = "0.34.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7f96b4737c2ce5987354855aed3797279def4ebf734436c6aa4552cf8e169935"
+dependencies = [
+ "crc32fast",
+ "crossbeam-epoch",
+ "crossbeam-utils",
+ "fs2",
+ "fxhash",
+ "libc",
+ "log",
+ "parking_lot 0.11.2",
+]
+
+[[package]]
 name = "smallvec"
 version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a507befe795404456341dfab10cef66ead4c041f62b8b11bbb92bffe5d0953e0"
 
 [[package]]
 name = "socket2"
@@ -2431,118 +2916,135 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "summa-core"
-version = "0.14.3"
+version = "0.15.0"
 dependencies = [
  "anyhow",
  "async-trait",
- "base64 0.21.0",
+ "base64 0.21.2",
  "bytes",
  "config",
  "derive_builder",
  "downcast-rs",
  "fasteval2",
  "futures",
  "hyper",
  "hyper-tls",
  "instant",
  "itertools",
  "lru",
  "matches",
  "oneshot",
  "opentelemetry",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pest",
  "pest_derive",
  "prost",
  "rand 0.8.5",
  "rayon",
  "rustc-hash",
  "safe-regex",
  "serde",
  "serde_bytes",
  "serde_cbor",
  "serde_json",
  "serde_yaml",
  "strfmt",
- "summa-proto",
+ "summa-proto 0.26.0",
  "take_mut",
  "tantivy",
  "tantivy-common",
  "tantivy-query-grammar",
  "thiserror",
  "time",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "summa-embed-py"
-version = "0.1.3"
+version = "0.15.0"
 dependencies = [
  "futures",
  "pyo3",
  "pyo3-asyncio",
  "pythonize",
  "serde_json",
  "summa-core",
- "summa-proto",
+ "summa-proto 0.26.0",
  "tantivy",
  "tokio",
 ]
 
 [[package]]
 name = "summa-proto"
-version = "0.25.0"
+version = "0.26.0"
 dependencies = [
  "prost",
  "prost-build",
  "prost-types",
  "protoc-bin-vendored",
  "serde",
  "tokio",
  "tonic",
  "tonic-build",
  "tonic-reflection",
 ]
 
 [[package]]
+name = "summa-proto"
+version = "0.26.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "11800e4c382bb5e8b6756e4fcaeb37a966e75f9c9796912e5066799587d81d00"
+dependencies = [
+ "prost",
+ "prost-build",
+ "prost-types",
+ "protoc-bin-vendored",
+ "serde",
+ "tonic",
+ "tonic-build",
+ "tonic-reflection",
+]
+
+[[package]]
 name = "summa-server"
-version = "0.14.3"
+version = "0.15.0"
 dependencies = [
  "anyhow",
  "async-broadcast",
  "async-trait",
  "clap",
  "config",
  "derive_builder",
  "futures",
  "futures-util",
  "headers",
  "hyper",
  "itertools",
+ "libz-sys",
  "opentelemetry",
  "opentelemetry-prometheus",
  "path-absolutize",
  "prometheus",
  "prost",
  "prost-types",
  "rand 0.8.5",
  "rdkafka",
  "rlimit",
  "serde",
  "serde_derive",
  "serde_json",
  "serde_yaml",
  "summa-core",
- "summa-proto",
+ "summa-proto 0.26.0",
  "take_mut",
  "tantivy",
  "tantivy-fst",
  "tempdir",
  "thiserror",
  "tikv-jemallocator",
  "time",
@@ -2559,28 +3061,28 @@
  "tracing-appender",
  "tracing-futures",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "summa-wasm"
-version = "0.122.6"
+version = "0.123.0"
 dependencies = [
  "async-trait",
  "console_error_panic_hook",
  "futures",
  "getrandom",
  "instant",
  "js-sys",
- "parking_lot",
+ "parking_lot 0.12.1",
  "serde",
  "serde-wasm-bindgen",
  "strfmt",
  "summa-core",
- "summa-proto",
+ "summa-proto 0.26.0",
  "tantivy",
  "thiserror",
  "tokio",
  "tracing",
  "tracing-wasm",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -2596,54 +3098,67 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.15"
+version = "2.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "sync_wrapper"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
 
 [[package]]
+name = "synstructure"
+version = "0.12.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f36bdaa60a83aca3921b5259d5400cbf5e90fc51931376a9bd4a0eb79aa7210f"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "syn 1.0.109",
+ "unicode-xid",
+]
+
+[[package]]
 name = "take_mut"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f764005d11ee5f36500a149ace24e00e3da98b0158b3e2d53a7495660d3f4d60"
 
 [[package]]
 name = "tantivy"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "aho-corasick",
  "arc-swap",
  "async-trait",
- "base64 0.21.0",
+ "base64 0.21.2",
  "bitpacking",
  "byteorder",
  "census",
  "crc32fast",
  "crossbeam-channel",
  "downcast-rs",
  "fail",
  "fastdivide",
  "fs4",
  "futures",
+ "futures-util",
  "htmlescape",
  "itertools",
  "izihawa-fst",
  "levenshtein_automata",
  "log",
  "lru",
  "measure_time",
@@ -2654,14 +3169,15 @@
  "oneshot",
  "rayon",
  "regex",
  "rust-stemmers",
  "rustc-hash",
  "serde",
  "serde_json",
+ "sketches-ddsketch",
  "smallvec",
  "tantivy-bitpacker",
  "tantivy-columnar",
  "tantivy-common",
  "tantivy-query-grammar",
  "tantivy-sstable",
  "tantivy-stacker",
@@ -2674,39 +3190,38 @@
  "winapi",
  "zstd",
 ]
 
 [[package]]
 name = "tantivy-bitpacker"
 version = "0.3.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "bitpacking",
 ]
 
 [[package]]
 name = "tantivy-columnar"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "fastdivide",
  "fnv",
  "itertools",
- "log",
  "serde",
  "tantivy-bitpacker",
  "tantivy-common",
  "tantivy-sstable",
  "tantivy-stacker",
 ]
 
 [[package]]
 name = "tantivy-common"
 version = "0.5.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "async-trait",
  "byteorder",
  "ownedbytes",
  "serde",
  "time",
 ]
@@ -2721,49 +3236,55 @@
  "regex-syntax 0.6.29",
  "utf8-ranges",
 ]
 
 [[package]]
 name = "tantivy-query-grammar"
 version = "0.19.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "combine",
  "once_cell",
  "regex",
 ]
 
 [[package]]
 name = "tantivy-sstable"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "izihawa-fst",
  "tantivy-common",
+ "zstd",
 ]
 
 [[package]]
 name = "tantivy-stacker"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
- "byteorder",
  "murmurhash32",
  "tantivy-common",
 ]
 
 [[package]]
 name = "tantivy-tokenizer-api"
 version = "0.1.0"
-source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#e614364c88531db0e77867156901f2699193b494"
+source = "git+https://github.com/izihawa/tantivy?branch=feature/summa#500a6d1a14e377415046c959f1c1d1c912a3732c"
 dependencies = [
  "serde",
 ]
 
 [[package]]
+name = "tap"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
+
+[[package]]
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tempdir"
@@ -2780,15 +3301,15 @@
 version = "3.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9fbec84f381d5795b08656e4912bec604d162bff9291d6189a78f4c8ab87998"
 dependencies = [
  "cfg-if",
  "fastrand",
  "redox_syscall 0.3.5",
- "rustix 0.37.15",
+ "rustix",
  "windows-sys 0.45.0",
 ]
 
 [[package]]
 name = "thiserror"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2801,15 +3322,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "thread_local"
 version = "1.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdd6f064ccff2d6567adcb3873ca630700f00b5ad3f060c25b5dcfd9a4ce152"
@@ -2836,52 +3357,52 @@
 dependencies = [
  "libc",
  "tikv-jemalloc-sys",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.20"
+version = "0.3.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cd0cbfecb4d19b5ea75bb31ad904eb5b9fa13f21079c3b92017ebdf4999a5890"
+checksum = "8f3403384eaacbca9923fa06940178ac13e4edb725486d70e8e15881d0c836cc"
 dependencies = [
  "itoa",
  "js-sys",
  "serde",
  "time-core",
  "time-macros",
 ]
 
 [[package]]
 name = "time-core"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2e153e1f1acaef8acc537e68b44906d2db6436e2b35ac2c6b42640fff91f00fd"
+checksum = "7300fbefb4dadc1af235a9cef3737cea692a9d97e1b9cbcd4ebdae6f8868e6fb"
 
 [[package]]
 name = "time-macros"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fd80a657e71da814b8e5d60d3374fc6d35045062245d80224748ae522dd76f36"
+checksum = "372950940a5f07bf38dbe211d7283c9e6d7327df53794992d293e534c733d09b"
 dependencies = [
  "time-core",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.28.0"
+version = "1.28.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c3c786bf8134e5a3a166db9b29ab8f48134739014a3eca7bc6bfa95d673b136f"
+checksum = "94d7b1cfd2aa4011f2de74c2c4c63665e27a71006b0a192dcd2710272e73dfa2"
 dependencies = [
  "autocfg",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
- "parking_lot",
+ "parking_lot 0.12.1",
  "pin-project-lite",
  "signal-hook-registry",
  "socket2",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
@@ -2899,15 +3420,15 @@
 name = "tokio-macros"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "630bdcf245f78637c13ec01ffae6187cca34625e8c63150d424b59e55af2675e"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -2948,31 +3469,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
 dependencies = [
  "serde",
 ]
 
 [[package]]
-name = "toml_datetime"
-version = "0.6.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ab8ed2edee10b50132aed5f331333428b011c99402b5a534154ed15746f9622"
-
-[[package]]
-name = "toml_edit"
-version = "0.19.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "239410c8609e8125456927e6707163a3b1fdb40561e4b803bc041f466ccfdc13"
-dependencies = [
- "indexmap",
- "toml_datetime",
- "winnow",
-]
-
-[[package]]
 name = "tonic"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f219fad3b929bef19b1f86fbc0358d35daed8f2cac972037ac0dc10bbb8d5fb"
 dependencies = [
  "async-stream",
  "async-trait",
@@ -3097,18 +3601,19 @@
 name = "tower-service"
 version = "0.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b6bc1c9ce2b5135ac7f93c72918fc37feb872bdc6a5533a8b85eb4b86bfdae52"
 
 [[package]]
 name = "tracing"
-version = "0.1.38"
+version = "0.1.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9cf6a813d3f40c88b0b6b6f29a5c95c6cdbf97c1f9cc53fb820200f5ad814d"
+checksum = "8ce8c33a8d48bd45d624a6e523445fd21ec13d3653cd51f681abf67418f54eb8"
 dependencies = [
+ "cfg-if",
  "log",
  "pin-project-lite",
  "tracing-attributes",
  "tracing-core",
 ]
 
 [[package]]
@@ -3126,22 +3631,22 @@
 name = "tracing-attributes"
 version = "0.1.24"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f57e3ca2a01450b1a921183a9c9cbfda207fd822cef4ccb00a65402cbba7a74"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.15",
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
 name = "tracing-futures"
@@ -3222,47 +3727,53 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-xid"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f962df74c8c05a667b5ee8bcf162993134c104e96440b663c8daa176dc772d8c"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
 
 [[package]]
+name = "unsigned-varint"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d86a8dc7f45e4c1b0d30e43038c38f274e77af056aa5f74b93c2cf9eb3c1c836"
+
+[[package]]
 name = "utf8-ranges"
 version = "1.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7fcfc827f90e53a02eaef5e535ee14266c1d569214c6aa70133a624d8a3164ba"
 
 [[package]]
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.3.1"
+version = "1.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b55a3fef2a1e3b3a00ce878640918820d3c51081576ac657d23af9fc7928fdb"
+checksum = "345444e32442451b267fc254ae85a209c64be56d2890e601a0c37ff0c3c5ecd2"
 dependencies = [
  "getrandom",
  "serde",
 ]
 
 [[package]]
 name = "valuable"
@@ -3296,83 +3807,83 @@
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
- "syn 1.0.109",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.34"
+version = "0.4.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f219e0d211ba40266969f6dbdd90636da12f75bee4fc9d6c23d1260dadb51454"
+checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
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
- "syn 1.0.109",
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
 name = "which"
@@ -3560,20 +4071,20 @@
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
 
 [[package]]
-name = "winnow"
-version = "0.4.1"
+name = "wyz"
+version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ae8970b36c66498d8ff1d66685dc86b91b29db0c7739899012f63a63814b4b28"
+checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
- "memchr",
+ "tap",
 ]
 
 [[package]]
 name = "yaml-rust"
 version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56c1936c4cc7a1c9ab21a1ebb602eb942ba868cbd44a99cb7cdc5892335e1c85"
```

