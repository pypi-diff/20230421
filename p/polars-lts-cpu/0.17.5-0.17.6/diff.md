# Comparing `tmp/polars_lts_cpu-0.17.5.tar.gz` & `tmp/polars_lts_cpu-0.17.6.tar.gz`

## Comparing `polars_lts_cpu-0.17.5.tar` & `polars_lts_cpu-0.17.6.tar`

### file list

```diff
@@ -1,1100 +1,1098 @@
--rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/LICENSE
--rw-r--r--   0     1001      123     3565 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/date.rs
--rw-r--r--   0     1001      123     6465 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/datetime.rs
--rw-r--r--   0     1001      123     3305 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/duration.rs
--rw-r--r--   0     1001      123     5607 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/kernels.rs
--rw-r--r--   0     1001      123     1062 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/mod.rs
--rw-r--r--   0     1001      123     7302 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
--rw-r--r--   0     1001      123     2582 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
--rw-r--r--   0     1001      123    10476 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
--rw-r--r--   0     1001      123      428 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
--rw-r--r--   0     1001      123     7368 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
--rw-r--r--   0     1001      123     4143 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/time.rs
--rw-r--r--   0     1001      123    21192 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
--rw-r--r--   0     1001      123    20108 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
--rw-r--r--   0     1001      123     4115 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
--rw-r--r--   0     1001      123     9692 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
--rw-r--r--   0     1001      123     2960 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/date_range.rs
--rw-r--r--   0     1001      123    31306 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/groupby/dynamic.rs
--rw-r--r--   0     1001      123       88 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/groupby/mod.rs
--rw-r--r--   0     1001      123      535 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/lib.rs
--rw-r--r--   0     1001      123      320 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/prelude.rs
--rw-r--r--   0     1001      123     1568 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/round.rs
--rw-r--r--   0     1001      123     4028 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/_trait.rs
--rw-r--r--   0     1001      123      136 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123      140 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/categoricals.rs
--rw-r--r--   0     1001      123      133 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/date.rs
--rw-r--r--   0     1001      123      137 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123      137 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123     1863 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     1792 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/integers.rs
--rw-r--r--   0     1001      123      133 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/list.rs
--rw-r--r--   0     1001      123      486 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123      155 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/object.rs
--rw-r--r--   0     1001      123      135 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123      133 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/time.rs
--rw-r--r--   0     1001      123      133 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123    12466 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/mod.rs
--rw-r--r--   0     1001      123     1630 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/truncate.rs
--rw-r--r--   0     1001      123     7059 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/upsample.rs
--rw-r--r--   0     1001      123     2567 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/utils.rs
--rw-r--r--   0     1001      123     1524 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/bounds.rs
--rw-r--r--   0     1001      123     2008 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/calendar.rs
--rw-r--r--   0     1001      123    23538 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/duration.rs
--rw-r--r--   0     1001      123    20089 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/groupby.rs
--rw-r--r--   0     1001      123      503 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/mod.rs
--rw-r--r--   0     1001      123    24202 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/test.rs
--rw-r--r--   0     1001      123    11624 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/window.rs
--rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-algo/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-algo/LICENSE
--rw-r--r--   0     1001      123     7265 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-algo/src/algo.rs
--rw-r--r--   0     1001      123       88 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-algo/src/lib.rs
--rw-r--r--   0     1001      123       28 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-algo/src/prelude.rs
--rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/LICENSE
--rw-r--r--   0     1001      123     2645 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/arena.rs
--rw-r--r--   0     1001      123     1373 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/atomic.rs
--rw-r--r--   0     1001      123     2659 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/cell.rs
--rw-r--r--   0     1001      123     1015 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/contention_pool.rs
--rw-r--r--   0     1001      123      509 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/error.rs
--rw-r--r--   0     1001      123      271 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/fmt.rs
--rw-r--r--   0     1001      123      763 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/functions.rs
--rw-r--r--   0     1001      123      514 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/hash.rs
--rw-r--r--   0     1001      123     2709 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
--rw-r--r--   0     1001      123       61 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/iter/mod.rs
--rw-r--r--   0     1001      123      583 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/lib.rs
--rw-r--r--   0     1001      123      573 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/macros.rs
--rw-r--r--   0     1001      123      282 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/mem.rs
--rw-r--r--   0     1001      123     1792 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/slice.rs
--rw-r--r--   0     1001      123     2467 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/sort.rs
--rw-r--r--   0     1001      123     1114 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/sync.rs
--rw-r--r--   0     1001      123      504 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/sys.rs
--rw-r--r--   0     1001      123      697 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/unwrap.rs
--rw-r--r--   0     1001      123      616 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/wasm.rs
--rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/LICENSE
--rw-r--r--   0     1001      123      234 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
--rw-r--r--   0     1001      123     3549 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
--rw-r--r--   0     1001      123    11023 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
--rw-r--r--   0     1001      123     1679 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/count.rs
--rw-r--r--   0     1001      123     2452 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
--rw-r--r--   0     1001      123     7861 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
--rw-r--r--   0     1001      123      511 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    22005 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
--rw-r--r--   0     1001      123     5269 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
--rw-r--r--   0     1001      123     2435 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
--rw-r--r--   0     1001      123      489 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     9380 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
--rw-r--r--   0     1001      123     6795 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/set.rs
--rw-r--r--   0     1001      123     7490 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
--rw-r--r--   0     1001      123     8251 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
--rw-r--r--   0     1001      123     2345 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
--rw-r--r--   0     1001      123      514 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
--rw-r--r--   0     1001      123    14731 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
--rw-r--r--   0     1001      123     4053 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
--rw-r--r--   0     1001      123     2486 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/top_k.rs
--rw-r--r--   0     1001      123     7727 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
--rw-r--r--   0     1001      123    18025 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/join/mod.rs
--rw-r--r--   0     1001      123     4174 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/mod.rs
--rw-r--r--   0     1001      123    10257 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/pivot/mod.rs
--rw-r--r--   0     1001      123    13486 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
--rw-r--r--   0     1001      123      217 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/lib.rs
--rw-r--r--   0     1001      123      290 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/prelude.rs
--rw-r--r--   0     1001      123       25 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/mod.rs
--rw-r--r--   0     1001      123     9623 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
--rw-r--r--   0     1001      123      118 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
--rw-r--r--   0     1001      123    11872 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
--rw-r--r--   0     1001      123     3680 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
--rw-r--r--   0     1001      123     3423 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/is_first.rs
--rw-r--r--   0     1001      123     2975 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/is_unique.rs
--rw-r--r--   0     1001      123     3626 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/log.rs
--rw-r--r--   0     1001      123     1106 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     1769 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/rolling.rs
--rw-r--r--   0     1001      123     7642 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
--rw-r--r--   0     1001      123     2500 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
--rw-r--r--   0     1001      123     2067 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/various.rs
--rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/LICENSE
--rw-r--r--   0     1001      123    19606 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
--rw-r--r--   0     1001      123     8679 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/bitwise.rs
--rw-r--r--   0     1001      123     2298 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
--rw-r--r--   0     1001      123     1207 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
--rw-r--r--   0     1001      123     1556 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/from.rs
--rw-r--r--   0     1001      123    19782 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/list.rs
--rw-r--r--   0     1001      123     8845 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
--rw-r--r--   0     1001      123     1410 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
--rw-r--r--   0     1001      123     2291 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
--rw-r--r--   0     1001      123    13129 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/cast.rs
--rw-r--r--   0     1001      123    48300 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
--rw-r--r--   0     1001      123     9463 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
--rw-r--r--   0     1001      123      551 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/drop.rs
--rw-r--r--   0     1001      123      963 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/float.rs
--rw-r--r--   0     1001      123     5069 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/from.rs
--rw-r--r--   0     1001      123    38411 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
--rw-r--r--   0     1001      123     1395 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
--rw-r--r--   0     1001      123       28 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
--rw-r--r--   0     1001      123     1129 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
--rw-r--r--   0     1001      123       21 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
--rw-r--r--   0     1001      123     2986 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
--rw-r--r--   0     1001      123     7230 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
--rw-r--r--   0     1001      123     2802 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/list/mod.rs
--rw-r--r--   0     1001      123    19456 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
--rw-r--r--   0     1001      123     3688 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
--rw-r--r--   0     1001      123     4270 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
--rw-r--r--   0     1001      123    10220 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
--rw-r--r--   0     1001      123     1400 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
--rw-r--r--   0     1001      123      358 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
--rw-r--r--   0     1001      123      192 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
--rw-r--r--   0     1001      123     2731 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
--rw-r--r--   0     1001      123     2172 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
--rw-r--r--   0     1001      123      925 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
--rw-r--r--   0     1001      123     6453 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
--rw-r--r--   0     1001      123     1604 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/date.rs
--rw-r--r--   0     1001      123     4105 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
--rw-r--r--   0     1001      123     4443 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
--rw-r--r--   0     1001      123     2434 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
--rw-r--r--   0     1001      123     2549 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
--rw-r--r--   0     1001      123      476 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
--rw-r--r--   0     1001      123    14266 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/time.rs
--rw-r--r--   0     1001      123    23524 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/mod.rs
--rw-r--r--   0     1001      123     7200 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ndarray.rs
--rw-r--r--   0     1001      123     4484 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/builder.rs
--rw-r--r--   0     1001      123     1547 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
--rw-r--r--   0     1001      123     3124 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
--rw-r--r--   0     1001      123     7054 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
--rw-r--r--   0     1001      123     3410 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
--rw-r--r--   0     1001      123      137 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
--rw-r--r--   0     1001      123     4419 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
--rw-r--r--   0     1001      123     4826 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/mod.rs
--rw-r--r--   0     1001      123     2517 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/registry.rs
--rw-r--r--   0     1001      123      272 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
--rw-r--r--   0     1001      123    32120 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
--rw-r--r--   0     1001      123     9946 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
--rw-r--r--   0     1001      123     2875 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
--rw-r--r--   0     1001      123     9391 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
--rw-r--r--   0     1001      123     2365 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/append.rs
--rw-r--r--   0     1001      123    27269 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
--rw-r--r--   0     1001      123    12799 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
--rw-r--r--   0     1001      123     6214 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
--rw-r--r--   0     1001      123    11537 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
--rw-r--r--   0     1001      123     1737 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
--rw-r--r--   0     1001      123     4801 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
--rw-r--r--   0     1001      123     6264 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
--rw-r--r--   0     1001      123    24977 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
--rw-r--r--   0     1001      123     8339 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
--rw-r--r--   0     1001      123    13777 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
--rw-r--r--   0     1001      123     5308 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
--rw-r--r--   0     1001      123     4436 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/full.rs
--rw-r--r--   0     1001      123        1 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
--rw-r--r--   0     1001      123    15089 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
--rw-r--r--   0     1001      123        1 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/len.rs
--rw-r--r--   0     1001      123    22261 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
--rw-r--r--   0     1001      123     2403 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
--rw-r--r--   0     1001      123      593 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
--rw-r--r--   0     1001      123     2585 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
--rw-r--r--   0     1001      123     1539 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
--rw-r--r--   0     1001      123    10234 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
--rw-r--r--   0     1001      123    12518 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/set.rs
--rw-r--r--   0     1001      123     6151 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
--rw-r--r--   0     1001      123     2299 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
--rw-r--r--   0     1001      123     5467 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
--rw-r--r--   0     1001      123     7430 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
--rw-r--r--   0     1001      123    30762 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
--rw-r--r--   0     1001      123      380 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
--rw-r--r--   0     1001      123    20472 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
--rw-r--r--   0     1001      123     6630 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
--rw-r--r--   0     1001      123     1859 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
--rw-r--r--   0     1001      123    16256 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
--rw-r--r--   0     1001      123     5041 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
--rw-r--r--   0     1001      123     6064 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
--rw-r--r--   0     1001      123    11229 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
--rw-r--r--   0     1001      123    14620 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
--rw-r--r--   0     1001      123     7753 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
--rw-r--r--   0     1001      123     9093 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/random.rs
--rw-r--r--   0     1001      123     1959 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
--rw-r--r--   0     1001      123     2501 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
--rw-r--r--   0     1001      123    11998 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
--rw-r--r--   0     1001      123     3201 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
--rw-r--r--   0     1001      123      533 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
--rw-r--r--   0     1001      123     1592 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
--rw-r--r--   0     1001      123      872 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/to_vec.rs
--rw-r--r--   0     1001      123     8113 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
--rw-r--r--   0     1001      123    25934 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
--rw-r--r--   0     1001      123     7689 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/cloud.rs
--rw-r--r--   0     1001      123     1549 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/config.rs
--rw-r--r--   0     1001      123     3946 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/_serde.rs
--rw-r--r--   0     1001      123     2701 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/aliases.rs
--rw-r--r--   0     1001      123    42410 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/any_value.rs
--rw-r--r--   0     1001      123    12083 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/dtype.rs
--rw-r--r--   0     1001      123     5532 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/field.rs
--rw-r--r--   0     1001      123     7675 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/mod.rs
--rw-r--r--   0     1001      123     2016 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/time_unit.rs
--rw-r--r--   0     1001      123      118 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/mod.rs
--rw-r--r--   0     1001      123      898 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
--rw-r--r--   0     1001      123      481 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
--rw-r--r--   0     1001      123      293 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
--rw-r--r--   0     1001      123      499 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
--rw-r--r--   0     1001      123      288 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
--rw-r--r--   0     1001      123     1071 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
--rw-r--r--   0     1001      123      819 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
--rw-r--r--   0     1001      123      596 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
--rw-r--r--   0     1001      123       43 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/mod.rs
--rw-r--r--   0     1001      123       25 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/error.rs
--rw-r--r--   0     1001      123      433 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/export.rs
--rw-r--r--   0     1001      123    36116 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/fmt.rs
--rw-r--r--   0     1001      123     5177 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/arithmetic.rs
--rw-r--r--   0     1001      123     7874 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/asof_join/asof.rs
--rw-r--r--   0     1001      123    33715 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/asof_join/groups.rs
--rw-r--r--   0     1001      123     6561 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/asof_join/mod.rs
--rw-r--r--   0     1001      123      559 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/chunks.rs
--rw-r--r--   0     1001      123     5179 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/cross_join.rs
--rw-r--r--   0     1001      123    16609 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/explode.rs
--rw-r--r--   0     1001      123     1019 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/from.rs
--rw-r--r--   0     1001      123    16518 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
--rw-r--r--   0     1001      123     4115 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
--rw-r--r--   0     1001      123     7643 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
--rw-r--r--   0     1001      123    39255 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
--rw-r--r--   0     1001      123     5636 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
--rw-r--r--   0     1001      123      218 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/expr.rs
--rw-r--r--   0     1001      123    12291 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/hashing.rs
--rw-r--r--   0     1001      123    14048 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
--rw-r--r--   0     1001      123    39434 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/mod.rs
--rw-r--r--   0     1001      123    10535 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/perfect.rs
--rw-r--r--   0     1001      123    17027 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/proxy.rs
--rw-r--r--   0     1001      123    18264 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/mod.rs
--rw-r--r--   0     1001      123    22392 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
--rw-r--r--   0     1001      123     2413 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
--rw-r--r--   0     1001      123    16352 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
--rw-r--r--   0     1001      123     2953 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
--rw-r--r--   0     1001      123     6076 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
--rw-r--r--   0     1001      123     4247 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
--rw-r--r--   0     1001      123     3913 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
--rw-r--r--   0     1001      123    11879 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
--rw-r--r--   0     1001      123   124247 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/mod.rs
--rw-r--r--   0     1001      123    27392 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/av_buffer.rs
--rw-r--r--   0     1001      123     3732 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/dataframe.rs
--rw-r--r--   0     1001      123     5950 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/mod.rs
--rw-r--r--   0     1001      123     8795 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/transpose.rs
--rw-r--r--   0     1001      123     2183 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/top_k.rs
--rw-r--r--   0     1001      123     1388 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/upstream_traits.rs
--rw-r--r--   0     1001      123    10935 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/functions.rs
--rw-r--r--   0     1001      123     2149 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/fx.rs
--rw-r--r--   0     1001      123     1503 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/identity.rs
--rw-r--r--   0     1001      123      457 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/mod.rs
--rw-r--r--   0     1001      123     2684 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/partition.rs
--rw-r--r--   0     1001      123    17653 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/vector_hasher.rs
--rw-r--r--   0     1001      123     1896 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/lib.rs
--rw-r--r--   0     1001      123    15766 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/named_from.rs
--rw-r--r--   0     1001      123     2411 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/prelude.rs
--rw-r--r--   0     1001      123     8247 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/schema.rs
--rw-r--r--   0     1001      123     4218 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/serde/chunked_array.rs
--rw-r--r--   0     1001      123     6551 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/serde/mod.rs
--rw-r--r--   0     1001      123     9929 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/serde/series.rs
--rw-r--r--   0     1001      123    18441 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/any_value.rs
--rw-r--r--   0     1001      123    28511 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
--rw-r--r--   0     1001      123      222 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/arithmetic/mod.rs
--rw-r--r--   0     1001      123     3546 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/arithmetic/owned.rs
--rw-r--r--   0     1001      123    13187 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/comparison.rs
--rw-r--r--   0     1001      123    24323 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/from.rs
--rw-r--r--   0     1001      123     9217 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/binary.rs
--rw-r--r--   0     1001      123    10850 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/boolean.rs
--rw-r--r--   0     1001      123    12938 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/categorical.rs
--rw-r--r--   0     1001      123    17994 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/dates_time.rs
--rw-r--r--   0     1001      123    15242 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/datetime.rs
--rw-r--r--   0     1001      123     5718 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/decimal.rs
--rw-r--r--   0     1001      123    15106 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/duration.rs
--rw-r--r--   0     1001      123    14223 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/floats.rs
--rw-r--r--   0     1001      123     6207 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/list.rs
--rw-r--r--   0     1001      123    18305 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/mod.rs
--rw-r--r--   0     1001      123     5246 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/null.rs
--rw-r--r--   0     1001      123     7817 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/object.rs
--rw-r--r--   0     1001      123    11029 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/struct_.rs
--rw-r--r--   0     1001      123     9735 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/utf8.rs
--rw-r--r--   0     1001      123     4257 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/into.rs
--rw-r--r--   0     1001      123     6297 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/iterator.rs
--rw-r--r--   0     1001      123    37180 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/mod.rs
--rw-r--r--   0     1001      123      853 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/diff.rs
--rw-r--r--   0     1001      123     5204 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/downcast.rs
--rw-r--r--   0     1001      123     3601 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/ewm.rs
--rw-r--r--   0     1001      123      413 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/extend.rs
--rw-r--r--   0     1001      123      562 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/mod.rs
--rw-r--r--   0     1001      123     5974 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/moment.rs
--rw-r--r--   0     1001      123     2908 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/null.rs
--rw-r--r--   0     1001      123     1347 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/pct_change.rs
--rw-r--r--   0     1001      123     4247 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/round.rs
--rw-r--r--   0     1001      123     5072 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/to_list.rs
--rw-r--r--   0     1001      123     1476 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/unique.rs
--rw-r--r--   0     1001      123    18263 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/series_trait.rs
--rw-r--r--   0     1001      123     2840 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/unstable.rs
--rw-r--r--   0     1001      123     8117 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/testing.rs
--rw-r--r--   0     1001      123      508 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/tests.rs
--rw-r--r--   0     1001      123    32703 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/utils/mod.rs
--rw-r--r--   0     1001      123     1181 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/utils/series.rs
--rw-r--r--   0     1001      123    13773 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/utils/supertype.rs
--rw-r--r--   0        0        0    10472 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/LICENSE
--rw-r--r--   0     1001      123     3275 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/Makefile
--rw-r--r--   0     1001      123      215 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/build.rs
--rw-r--r--   0     1001      123       78 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/clippy.toml
--rw-r--r--   0     1001      123    17602 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/eager.rs
--rw-r--r--   0     1001      123     8778 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/lazy.rs
--rw-r--r--   0     1001      123       50 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/mod.rs
--rw-r--r--   0     1001      123     3797 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/performance.rs
--rw-r--r--   0     1001      123       59 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/export.rs
--rw-r--r--   0     1001      123    20212 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/lib.rs
--rw-r--r--   0     1001      123      387 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/prelude.rs
--rw-r--r--   0     1001      123       32 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/src/sql.rs
--rw-r--r--   0     1001      123     4272 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/date_like.rs
--rw-r--r--   0     1001      123     2401 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/groupby.rs
--rw-r--r--   0     1001      123    17826 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/joins.rs
--rw-r--r--   0     1001      123      545 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/list.rs
--rw-r--r--   0     1001      123      189 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/mod.rs
--rw-r--r--   0     1001      123     6258 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/pivot.rs
--rw-r--r--   0     1001      123     1102 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/random.rs
--rw-r--r--   0     1001      123    10844 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/rolling_window.rs
--rw-r--r--   0     1001      123     1093 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/series.rs
--rw-r--r--   0     1001      123      370 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/utils.rs
--rw-r--r--   0     1001      123    30142 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/csv.rs
--rw-r--r--   0     1001      123     4490 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/ipc_stream.rs
--rw-r--r--   0     1001      123     7044 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/json.rs
--rw-r--r--   0     1001      123      378 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/mod.rs
--rw-r--r--   0     1001      123      988 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/parquet.rs
--rw-r--r--   0     1001      123     1530 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/joins.rs
--rw-r--r--   0     1001      123     2452 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/aggregation.rs
--rw-r--r--   0     1001      123      702 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/cse.rs
--rw-r--r--   0     1001      123      500 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/explodes.rs
--rw-r--r--   0     1001      123     2279 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
--rw-r--r--   0     1001      123    10815 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
--rw-r--r--   0     1001      123     1064 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
--rw-r--r--   0     1001      123     1008 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
--rw-r--r--   0     1001      123      428 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
--rw-r--r--   0     1001      123      121 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
--rw-r--r--   0     1001      123      659 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
--rw-r--r--   0     1001      123    10139 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/window.rs
--rw-r--r--   0     1001      123      579 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/folds.rs
--rw-r--r--   0     1001      123      557 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/functions.rs
--rw-r--r--   0     1001      123     4482 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/groupby.rs
--rw-r--r--   0     1001      123     1655 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
--rw-r--r--   0     1001      123      691 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/mod.rs
--rw-r--r--   0     1001      123     5381 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
--rw-r--r--   0     1001      123     4476 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/projection_queries.rs
--rw-r--r--   0     1001      123     6444 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/queries.rs
--rw-r--r--   0     1001      123      141 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/main.rs
--rw-r--r--   0     1001      123      552 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/schema.rs
--rw-r--r--   0        0        0     6007 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/LICENSE
--rw-r--r--   0     1001      123     1796 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dot.rs
--rw-r--r--   0     1001      123     4359 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/eval.rs
--rw-r--r--   0     1001      123     4505 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/functions.rs
--rw-r--r--   0     1001      123      164 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/into.rs
--rw-r--r--   0     1001      123     6768 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/list.rs
--rw-r--r--   0     1001      123     2899 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/mod.rs
--rw-r--r--   0     1001      123     1182 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
--rw-r--r--   0     1001      123     9288 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/csv.rs
--rw-r--r--   0     1001      123     4309 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
--rw-r--r--   0     1001      123     2261 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/ipc.rs
--rw-r--r--   0     1001      123    47111 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/mod.rs
--rw-r--r--   0     1001      123     3414 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/ndjson.rs
--rw-r--r--   0     1001      123     3440 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/parquet.rs
--rw-r--r--   0     1001      123     2892 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/pivot.rs
--rw-r--r--   0     1001      123      416 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/python.rs
--rw-r--r--   0     1001      123     6376 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/lib.rs
--rw-r--r--   0     1001      123     1049 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
--rw-r--r--   0     1001      123      776 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
--rw-r--r--   0     1001      123      670 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
--rw-r--r--   0     1001      123     1284 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
--rw-r--r--   0     1001      123     3908 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
--rw-r--r--   0     1001      123     3577 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
--rw-r--r--   0     1001      123    13439 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
--rw-r--r--   0     1001      123     4335 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
--rw-r--r--   0     1001      123     6058 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
--rw-r--r--   0     1001      123     7074 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
--rw-r--r--   0     1001      123     2045 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
--rw-r--r--   0     1001      123     1677 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
--rw-r--r--   0     1001      123     2986 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
--rw-r--r--   0     1001      123     1963 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
--rw-r--r--   0     1001      123     4184 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
--rw-r--r--   0     1001      123     1211 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
--rw-r--r--   0     1001      123     2421 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
--rw-r--r--   0     1001      123      548 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
--rw-r--r--   0     1001      123     2197 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
--rw-r--r--   0     1001      123     1922 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
--rw-r--r--   0     1001      123      663 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
--rw-r--r--   0     1001      123     3702 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
--rw-r--r--   0     1001      123      838 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
--rw-r--r--   0     1001      123     1284 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
--rw-r--r--   0     1001      123    21864 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
--rw-r--r--   0     1001      123     2689 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
--rw-r--r--   0     1001      123    17432 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
--rw-r--r--   0     1001      123    18857 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
--rw-r--r--   0     1001      123     3153 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
--rw-r--r--   0     1001      123     6326 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
--rw-r--r--   0     1001      123     2003 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
--rw-r--r--   0     1001      123     5809 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
--rw-r--r--   0     1001      123     4131 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
--rw-r--r--   0     1001      123     5304 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
--rw-r--r--   0     1001      123    21103 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
--rw-r--r--   0     1001      123    10091 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
--rw-r--r--   0     1001      123     3929 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
--rw-r--r--   0     1001      123    11541 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
--rw-r--r--   0     1001      123     8331 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
--rw-r--r--   0     1001      123    14360 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
--rw-r--r--   0     1001      123    31819 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
--rw-r--r--   0     1001      123     2044 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
--rw-r--r--   0     1001      123      419 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/mod.rs
--rw-r--r--   0     1001      123     2005 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
--rw-r--r--   0     1001      123    27335 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
--rw-r--r--   0     1001      123    18867 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
--rw-r--r--   0     1001      123       87 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
--rw-r--r--   0     1001      123     9470 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/state.rs
--rw-r--r--   0     1001      123    20901 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
--rw-r--r--   0     1001      123      219 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
--rw-r--r--   0     1001      123     3333 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
--rw-r--r--   0     1001      123      722 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/prelude.rs
--rw-r--r--   0     1001      123    14990 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/aggregations.rs
--rw-r--r--   0     1001      123     2339 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/arity.rs
--rw-r--r--   0     1001      123     7031 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/cse.rs
--rw-r--r--   0     1001      123    12749 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/io.rs
--rw-r--r--   0     1001      123     4207 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/logical.rs
--rw-r--r--   0     1001      123     4293 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/mod.rs
--rw-r--r--   0     1001      123    14819 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
--rw-r--r--   0     1001      123     6799 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
--rw-r--r--   0     1001      123     3158 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/projection_queries.rs
--rw-r--r--   0     1001      123    47907 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/queries.rs
--rw-r--r--   0     1001      123     8358 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/streaming.rs
--rw-r--r--   0     1001      123     2953 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/tpch.rs
--rw-r--r--   0     1001      123     1033 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/utils.rs
--rw-r--r--   0        0        0     4346 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/LICENSE
--rw-r--r--   0     1001      123     2383 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/avro/mod.rs
--rw-r--r--   0     1001      123     3604 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/avro/read.rs
--rw-r--r--   0     1001      123     2622 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/avro/write.rs
--rw-r--r--   0     1001      123     4505 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/cloud/adaptors.rs
--rw-r--r--   0     1001      123     9506 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/cloud/glob.rs
--rw-r--r--   0     1001      123     3089 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/cloud/mod.rs
--rw-r--r--   0     1001      123    28675 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/buffer.rs
--rw-r--r--   0     1001      123     1898 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/mod.rs
--rw-r--r--   0     1001      123    19709 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/parser.rs
--rw-r--r--   0     1001      123    21349 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read.rs
--rw-r--r--   0     1001      123    10817 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
--rw-r--r--   0     1001      123    13909 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
--rw-r--r--   0     1001      123    31233 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read_impl/mod.rs
--rw-r--r--   0     1001      123    11466 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/splitfields.rs
--rw-r--r--   0     1001      123    25218 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/utils.rs
--rw-r--r--   0     1001      123     2796 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/write.rs
--rw-r--r--   0     1001      123    12866 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/write_impl.rs
--rw-r--r--   0     1001      123      184 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/export.rs
--rw-r--r--   0     1001      123     7580 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/ipc_file.rs
--rw-r--r--   0     1001      123     9218 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/ipc_stream.rs
--rw-r--r--   0     1001      123     3253 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/mmap.rs
--rw-r--r--   0     1001      123      401 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/mod.rs
--rw-r--r--   0     1001      123     8282 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/write.rs
--rw-r--r--   0     1001      123     1471 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/write_async.rs
--rw-r--r--   0     1001      123     9974 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/json.rs
--rw-r--r--   0     1001      123     4879 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/lib.rs
--rw-r--r--   0     1001      123     1969 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/mmap.rs
--rw-r--r--   0     1001      123     7215 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ndjson_core/buffer.rs
--rw-r--r--   0     1001      123       39 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ndjson_core/mod.rs
--rw-r--r--   0     1001      123    12177 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
--rw-r--r--   0     1001      123      273 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/options.rs
--rw-r--r--   0     1001      123     7354 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/async_impl.rs
--rw-r--r--   0     1001      123     3093 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/mmap.rs
--rw-r--r--   0     1001      123     3132 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/mod.rs
--rw-r--r--   0     1001      123     4790 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/predicates.rs
--rw-r--r--   0     1001      123     9629 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/read.rs
--rw-r--r--   0     1001      123    16886 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/read_impl.rs
--rw-r--r--   0     1001      123    10106 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/write.rs
--rw-r--r--   0     1001      123     5334 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/partition.rs
--rw-r--r--   0     1001      123     1455 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/predicates.rs
--rw-r--r--   0     1001      123      633 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/prelude.rs
--rw-r--r--   0     1001      123      417 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/tests.rs
--rw-r--r--   0     1001      123     4467 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/utils.rs
--rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-error/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-error/LICENSE
--rw-r--r--   0     1001      123     6297 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-error/src/lib.rs
--rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/LICENSE
--rw-r--r--   0     1001      123     8985 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encode.rs
--rw-r--r--   0     1001      123     4591 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encodings/fixed.rs
--rw-r--r--   0     1001      123       47 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encodings/mod.rs
--rw-r--r--   0     1001      123     4508 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encodings/variable.rs
--rw-r--r--   0     1001      123    13678 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/lib.rs
--rw-r--r--   0     1001      123     2079 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/row.rs
--rw-r--r--   0     1001      123      682 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/utils.rs
--rw-r--r--   0        0        0     1411 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/LICENSE
--rw-r--r--   0     1001      123     4012 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/README.md
--rw-r--r--   0     1001      123     9096 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/assets/SQL.sublime-syntax
--rw-r--r--   0     1001      123    21158 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/assets/theme
--rw-r--r--   0     1001      123     1433 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/cli/highlighter.rs
--rw-r--r--   0     1001      123     5023 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/cli/mod.rs
--rw-r--r--   0     1001      123     1043 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/cli/prompt.rs
--rw-r--r--   0     1001      123    14453 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/context.rs
--rw-r--r--   0     1001      123    16610 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/functions.rs
--rw-r--r--   0     1001      123    27444 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/lib.rs
--rw-r--r--   0     1001      123      342 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/main.rs
--rw-r--r--   0     1001      123    13269 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/sql_expr.rs
--rw-r--r--   0     1001      123     3386 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/table_functions.rs
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/LICENSE
--rw-r--r--   0     1001      123     1975 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/default_arrays.rs
--rw-r--r--   0     1001      123     3160 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/get.rs
--rw-r--r--   0     1001      123     6171 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/list.rs
--rw-r--r--   0     1001      123     7771 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/mod.rs
--rw-r--r--   0     1001      123      878 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/null.rs
--rw-r--r--   0     1001      123     1125 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/slice.rs
--rw-r--r--   0     1001      123     1807 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/utf8.rs
--rw-r--r--   0     1001      123     2294 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/bit_util.rs
--rw-r--r--   0     1001      123       17 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/bitmap/mod.rs
--rw-r--r--   0     1001      123      819 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/bitmap/mutable.rs
--rw-r--r--   0     1001      123      232 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/compute/cast.rs
--rw-r--r--   0     1001      123       56 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/compute/mod.rs
--rw-r--r--   0     1001      123     2962 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/compute/take/boolean.rs
--rw-r--r--   0     1001      123    24907 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/compute/take/mod.rs
--rw-r--r--   0     1001      123     1042 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/conversion.rs
--rw-r--r--   0     1001      123     1609 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/data_types.rs
--rw-r--r--   0     1001      123       25 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/error.rs
--rw-r--r--   0     1001      123       28 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/export.rs
--rw-r--r--   0     1001      123       26 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/floats/mod.rs
--rw-r--r--   0     1001      123     2066 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/floats/ord.rs
--rw-r--r--   0     1001      123     1273 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/index.rs
--rw-r--r--   0     1001      123      915 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/is_valid.rs
--rw-r--r--   0     1001      123     4740 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
--rw-r--r--   0     1001      123     1015 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/concatenate.rs
--rw-r--r--   0     1001      123     5161 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
--rw-r--r--   0     1001      123     1808 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
--rw-r--r--   0     1001      123    25065 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
--rw-r--r--   0     1001      123     1406 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/float.rs
--rw-r--r--   0     1001      123     4907 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/list.rs
--rw-r--r--   0     1001      123     1895 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
--rw-r--r--   0     1001      123     9731 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/mod.rs
--rw-r--r--   0     1001      123     3703 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
--rw-r--r--   0     1001      123     2022 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
--rw-r--r--   0     1001      123    18684 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
--rw-r--r--   0     1001      123     3924 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
--rw-r--r--   0     1001      123    11659 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
--rw-r--r--   0     1001      123     5504 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
--rw-r--r--   0     1001      123     8683 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
--rw-r--r--   0     1001      123     1749 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
--rw-r--r--   0     1001      123    14367 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
--rw-r--r--   0     1001      123     9070 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
--rw-r--r--   0     1001      123    11609 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
--rw-r--r--   0     1001      123     4698 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
--rw-r--r--   0     1001      123     8335 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
--rw-r--r--   0     1001      123     8109 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
--rw-r--r--   0     1001      123     4752 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/set.rs
--rw-r--r--   0     1001      123     4529 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
--rw-r--r--   0     1001      123     2948 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
--rw-r--r--   0     1001      123     5974 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
--rw-r--r--   0     1001      123      231 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
--rw-r--r--   0     1001      123      841 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/string.rs
--rw-r--r--   0     1001      123     2310 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
--rw-r--r--   0     1001      123     4343 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
--rw-r--r--   0     1001      123     2606 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
--rw-r--r--   0     1001      123     4417 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/time.rs
--rw-r--r--   0     1001      123      341 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/lib.rs
--rw-r--r--   0     1001      123      434 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/prelude.rs
--rw-r--r--   0     1001      123      534 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/slice.rs
--rw-r--r--   0     1001      123      762 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/time_zone.rs
--rw-r--r--   0     1001      123      998 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
--rw-r--r--   0     1001      123     2716 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/mod.rs
--rw-r--r--   0     1001      123     2533 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
--rw-r--r--   0     1001      123      158 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/rev.rs
--rw-r--r--   0     1001      123     5020 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/utils.rs
--rw-r--r--   0        0        0     1780 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/LICENSE
--rw-r--r--   0     1001      123       98 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/mod.rs
--rw-r--r--   0     1001      123     1219 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/filter.rs
--rw-r--r--   0     1001      123     4103 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/function.rs
--rw-r--r--   0     1001      123      229 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/mod.rs
--rw-r--r--   0     1001      123      548 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
--rw-r--r--   0     1001      123     3247 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/projection.rs
--rw-r--r--   0     1001      123     2324 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
--rw-r--r--   0     1001      123     6479 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
--rw-r--r--   0     1001      123    10473 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
--rw-r--r--   0     1001      123     1207 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
--rw-r--r--   0     1001      123     1888 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
--rw-r--r--   0     1001      123     4554 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
--rw-r--r--   0     1001      123     1746 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
--rw-r--r--   0     1001      123     5413 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
--rw-r--r--   0     1001      123     4951 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
--rw-r--r--   0     1001      123      211 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
--rw-r--r--   0     1001      123      856 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
--rw-r--r--   0     1001      123     4294 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
--rw-r--r--   0     1001      123     3030 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
--rw-r--r--   0     1001      123     6275 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
--rw-r--r--   0     1001      123    13665 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
--rw-r--r--   0     1001      123     2681 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
--rw-r--r--   0     1001      123     2534 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
--rw-r--r--   0     1001      123     5961 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
--rw-r--r--   0     1001      123    10613 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
--rw-r--r--   0     1001      123     2164 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
--rw-r--r--   0     1001      123     4666 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
--rw-r--r--   0     1001      123     3906 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
--rw-r--r--   0     1001      123    20856 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
--rw-r--r--   0     1001      123    23518 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
--rw-r--r--   0     1001      123     2457 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
--rw-r--r--   0     1001      123     8395 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/io.rs
--rw-r--r--   0     1001      123     5485 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
--rw-r--r--   0     1001      123    14279 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
--rw-r--r--   0     1001      123    11824 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
--rw-r--r--   0     1001      123      178 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
--rw-r--r--   0     1001      123     2002 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
--rw-r--r--   0     1001      123      589 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
--rw-r--r--   0     1001      123     1492 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
--rw-r--r--   0     1001      123     1824 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
--rw-r--r--   0     1001      123     3108 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
--rw-r--r--   0     1001      123      130 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
--rw-r--r--   0     1001      123     3808 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
--rw-r--r--   0     1001      123     6295 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
--rw-r--r--   0     1001      123     5953 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
--rw-r--r--   0     1001      123     3801 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
--rw-r--r--   0     1001      123      635 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
--rw-r--r--   0     1001      123     5076 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/csv.rs
--rw-r--r--   0     1001      123     1231 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/frame.rs
--rw-r--r--   0     1001      123      987 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
--rw-r--r--   0     1001      123      376 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/mod.rs
--rw-r--r--   0     1001      123     3387 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
--rw-r--r--   0     1001      123     1146 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
--rw-r--r--   0     1001      123     1022 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/union.rs
--rw-r--r--   0     1001      123      448 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/expressions.rs
--rw-r--r--   0     1001      123      272 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/lib.rs
--rw-r--r--   0     1001      123      719 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/chunks.rs
--rw-r--r--   0     1001      123      474 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/context.rs
--rw-r--r--   0     1001      123      223 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/mod.rs
--rw-r--r--   0     1001      123      430 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/operator.rs
--rw-r--r--   0     1001      123      626 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/sink.rs
--rw-r--r--   0     1001      123      241 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/source.rs
--rw-r--r--   0     1001      123        1 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/config.rs
--rw-r--r--   0     1001      123    20488 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/convert.rs
--rw-r--r--   0     1001      123    13982 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
--rw-r--r--   0     1001      123     1237 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/mod.rs
--rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/Cargo.toml
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/LICENSE
--rw-r--r--   0     1001      123       45 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/constants.rs
--rw-r--r--   0     1001      123    17253 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dot.rs
--rw-r--r--   0     1001      123     4171 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/arithmetic.rs
--rw-r--r--   0     1001      123      935 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/binary.rs
--rw-r--r--   0     1001      123      650 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/cat.rs
--rw-r--r--   0     1001      123     9424 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/dt.rs
--rw-r--r--   0     1001      123    13169 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/expr.rs
--rw-r--r--   0     1001      123      753 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/from.rs
--rw-r--r--   0     1001      123       85 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
--rw-r--r--   0     1001      123     1431 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
--rw-r--r--   0     1001      123     1327 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
--rw-r--r--   0     1001      123     4221 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
--rw-r--r--   0     1001      123     1910 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
--rw-r--r--   0     1001      123     1216 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
--rw-r--r--   0     1001      123      344 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
--rw-r--r--   0     1001      123     1593 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
--rw-r--r--   0     1001      123    13227 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
--rw-r--r--   0     1001      123      810 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
--rw-r--r--   0     1001      123     1364 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
--rw-r--r--   0     1001      123     8119 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
--rw-r--r--   0     1001      123      581 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
--rw-r--r--   0     1001      123    19145 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
--rw-r--r--   0     1001      123      462 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
--rw-r--r--   0     1001      123     3132 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
--rw-r--r--   0     1001      123      152 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
--rw-r--r--   0     1001      123      260 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
--rw-r--r--   0     1001      123      200 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
--rw-r--r--   0     1001      123    13421 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
--rw-r--r--   0     1001      123      306 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
--rw-r--r--   0     1001      123     3812 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
--rw-r--r--   0     1001      123     1238 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
--rw-r--r--   0     1001      123      972 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
--rw-r--r--   0     1001      123    19590 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
--rw-r--r--   0     1001      123     1017 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
--rw-r--r--   0     1001      123     2700 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
--rw-r--r--   0     1001      123     5122 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
--rw-r--r--   0     1001      123      170 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
--rw-r--r--   0     1001      123    42541 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/functions.rs
--rw-r--r--   0     1001      123    10196 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/list.rs
--rw-r--r--   0     1001      123     2181 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/meta.rs
--rw-r--r--   0     1001      123    64804 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/mod.rs
--rw-r--r--   0     1001      123       40 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/names.rs
--rw-r--r--   0     1001      123     2094 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/options.rs
--rw-r--r--   0     1001      123    14993 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/string.rs
--rw-r--r--   0     1001      123     2715 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/struct_.rs
--rw-r--r--   0     1001      123       38 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/frame/mod.rs
--rw-r--r--   0     1001      123      933 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/frame/opt_state.rs
--rw-r--r--   0     1001      123      466 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/global.rs
--rw-r--r--   0     1001      123      175 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/lib.rs
--rw-r--r--   0     1001      123     6825 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
--rw-r--r--   0     1001      123    11393 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
--rw-r--r--   0     1001      123    25701 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/alp.rs
--rw-r--r--   0     1001      123     1622 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
--rw-r--r--   0     1001      123     1428 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/apply.rs
--rw-r--r--   0     1001      123    25056 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/builder.rs
--rw-r--r--   0     1001      123    29662 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/conversion.rs
--rw-r--r--   0     1001      123      301 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/debug.rs
--rw-r--r--   0     1001      123    15196 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/format.rs
--rw-r--r--   0     1001      123      895 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
--rw-r--r--   0     1001      123      137 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
--rw-r--r--   0     1001      123     1169 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
--rw-r--r--   0     1001      123    12019 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
--rw-r--r--   0     1001      123     1330 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
--rw-r--r--   0     1001      123     9752 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/iterator.rs
--rw-r--r--   0     1001      123    10463 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/lit.rs
--rw-r--r--   0     1001      123     8148 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/mod.rs
--rw-r--r--   0     1001      123     7416 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
--rw-r--r--   0     1001      123    15287 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
--rw-r--r--   0     1001      123     3260 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
--rw-r--r--   0     1001      123     3236 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
--rw-r--r--   0     1001      123     3994 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
--rw-r--r--   0     1001      123    14494 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
--rw-r--r--   0     1001      123     1556 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
--rw-r--r--   0     1001      123     6715 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
--rw-r--r--   0     1001      123     1222 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
--rw-r--r--   0     1001      123    28281 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
--rw-r--r--   0     1001      123     2571 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
--rw-r--r--   0     1001      123    15130 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
--rw-r--r--   0     1001      123     1755 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
--rw-r--r--   0     1001      123     3930 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
--rw-r--r--   0     1001      123     1799 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
--rw-r--r--   0     1001      123     3269 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
--rw-r--r--   0     1001      123     2638 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
--rw-r--r--   0     1001      123    15747 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
--rw-r--r--   0     1001      123    26507 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
--rw-r--r--   0     1001      123     2692 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
--rw-r--r--   0     1001      123     2639 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
--rw-r--r--   0     1001      123     3501 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
--rw-r--r--   0     1001      123    27332 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
--rw-r--r--   0     1001      123     3492 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
--rw-r--r--   0     1001      123    13850 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
--rw-r--r--   0     1001      123     3161 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
--rw-r--r--   0     1001      123     9725 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
--rw-r--r--   0     1001      123    19819 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
--rw-r--r--   0     1001      123    10197 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/options.rs
--rw-r--r--   0     1001      123    15273 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/projection.rs
--rw-r--r--   0     1001      123     4615 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
--rw-r--r--   0     1001      123    13048 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/schema.rs
--rw-r--r--   0     1001      123      809 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/prelude.rs
--rw-r--r--   0     1001      123    11955 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/utils.rs
--rw-r--r--   0        0        0     4403 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/Cargo.toml
--rw-r--r--   0     1001      123       76 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/.gitignore
--rw-r--r--   0     1001      123     1055 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/LICENSE
--rw-r--r--   0     1001      123     2414 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/Makefile
--rw-r--r--   0     1001      123    11845 2023-04-17 15:57:55.000000 polars_lts_cpu-0.17.5/README.md
--rw-r--r--   0     1001      123      651 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/build.rs
--rw-r--r--   0     1001      123       32 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/.gitignore
--rw-r--r--   0     1001      123      679 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/Makefile
--rw-r--r--   0     1001      123      318 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/api_redirect.html
--rw-r--r--   0     1001      123      151 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/autosummary/accessor.rst
--rw-r--r--   0     1001      123      160 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/autosummary/accessor_attribute.rst
--rw-r--r--   0     1001      123      168 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/autosummary/accessor_callable.rst
--rw-r--r--   0     1001      123      157 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/autosummary/accessor_method.rst
--rw-r--r--   0     1001      123      836 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/autosummary/class.rst
--rw-r--r--   0     1001      123       94 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/autosummary/class_without_autosummary.rst
--rw-r--r--   0     1001      123      406 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/_templates/sidebar-nav-bs.html
--rw-r--r--   0     1001      123      450 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/requirements-docs.txt
--rw-r--r--   0     1001      123     1567 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/_static/css/custom.css
--rw-r--r--   0     1001      123     7302 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/conf.py
--rw-r--r--   0     1001      123       51 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/index.rst
--rw-r--r--   0     1001      123     6767 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/api.rst
--rw-r--r--   0     1001      123     1339 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/config.rst
--rw-r--r--   0     1001      123      274 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/aggregation.rst
--rw-r--r--   0     1001      123      221 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/attributes.rst
--rw-r--r--   0     1001      123      142 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/computation.rst
--rw-r--r--   0     1001      123      319 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/descriptive.rst
--rw-r--r--   0     1001      123      319 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/export.rst
--rw-r--r--   0     1001      123      464 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/groupby.rst
--rw-r--r--   0     1001      123      379 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/index.rst
--rw-r--r--   0     1001      123      189 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/miscellaneous.rst
--rw-r--r--   0     1001      123     1513 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/dataframe/modify_select.rst
--rw-r--r--   0     1001      123      663 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/datatypes.rst
--rw-r--r--   0     1001      123      421 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/exceptions.rst
--rw-r--r--   0     1001      123      391 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/aggregation.rst
--rw-r--r--   0     1001      123      309 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/binary.rst
--rw-r--r--   0     1001      123      338 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/boolean.rst
--rw-r--r--   0     1001      123      237 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/categories.rst
--rw-r--r--   0     1001      123      221 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/columns.rst
--rw-r--r--   0     1001      123     1061 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/computation.rst
--rw-r--r--   0     1001      123     1114 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/functions.rst
--rw-r--r--   0     1001      123      461 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/index.rst
--rw-r--r--   0     1001      123      695 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/list.rst
--rw-r--r--   0     1001      123      374 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/meta.rst
--rw-r--r--   0     1001      123      125 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/miscellaneous.rst
--rw-r--r--   0     1001      123      977 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/modify_select.rst
--rw-r--r--   0     1001      123      639 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/operators.rst
--rw-r--r--   0     1001      123      860 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/string.rst
--rw-r--r--   0     1001      123      254 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/struct.rst
--rw-r--r--   0     1001      123      968 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/temporal.rst
--rw-r--r--   0     1001      123       98 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/expressions/window.rst
--rw-r--r--   0     1001      123      692 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/functions.rst
--rw-r--r--   0     1001      123      392 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/index.rst
--rw-r--r--   0     1001      123     1269 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/io.rst
--rw-r--r--   0     1001      123      252 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/aggregation.rst
--rw-r--r--   0     1001      123      179 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/attributes.rst
--rw-r--r--   0     1001      123      146 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/descriptive.rst
--rw-r--r--   0     1001      123      497 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/groupby.rst
--rw-r--r--   0     1001      123      354 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/index.rst
--rw-r--r--   0     1001      123      455 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/miscellaneous.rst
--rw-r--r--   0     1001      123      988 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/modify_select.rst
--rw-r--r--   0     1001      123      339 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/aggregation.rst
--rw-r--r--   0     1001      123      256 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/attributes.rst
--rw-r--r--   0     1001      123      321 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/binary.rst
--rw-r--r--   0     1001      123      117 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/boolean.rst
--rw-r--r--   0     1001      123      241 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/categories.rst
--rw-r--r--   0     1001      123     1103 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/computation.rst
--rw-r--r--   0     1001      123      722 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/descriptive.rst
--rw-r--r--   0     1001      123      240 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/export.rst
--rw-r--r--   0     1001      123      428 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/index.rst
--rw-r--r--   0     1001      123      749 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/list.rst
--rw-r--r--   0     1001      123      236 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/miscellaneous.rst
--rw-r--r--   0     1001      123     1077 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/modify_select.rst
--rw-r--r--   0     1001      123      922 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/string.rst
--rw-r--r--   0     1001      123      396 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/struct.rst
--rw-r--r--   0     1001      123     1118 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/series/temporal.rst
--rw-r--r--   0     1001      123      302 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/sql.rst
--rw-r--r--   0     1001      123      647 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/testing.rst
--rw-r--r--   0     1001      123      168 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/docs/source/reference/utils.rst
--rw-r--r--   0     1001      123     6283 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/__init__.py
--rw-r--r--   0     1001      123    13396 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/api.py
--rw-r--r--   0     1001      123    24553 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/config.py
--rw-r--r--   0     1001      123    25409 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/convert.py
--rw-r--r--   0     1001      123       77 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/dataframe/__init__.py
--rw-r--r--   0     1001      123     5057 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/dataframe/_html.py
--rw-r--r--   0     1001      123   303518 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/dataframe/frame.py
--rw-r--r--   0     1001      123    33240 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/dataframe/groupby.py
--rw-r--r--   0     1001      123     2588 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/datatypes/__init__.py
--rw-r--r--   0     1001      123    11189 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/datatypes/classes.py
--rw-r--r--   0     1001      123     1541 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/datatypes/constants.py
--rw-r--r--   0     1001      123     4430 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/datatypes/constructor.py
--rw-r--r--   0     1001      123    12688 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/datatypes/convert.py
--rw-r--r--   0     1001      123     7338 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/dependencies.py
--rw-r--r--   0     1001      123     2954 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/exceptions.py
--rw-r--r--   0     1001      123       61 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/__init__.py
--rw-r--r--   0     1001      123     2730 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/binary.py
--rw-r--r--   0     1001      123     1708 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/categorical.py
--rw-r--r--   0     1001      123    69359 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/datetime.py
--rw-r--r--   0     1001      123   251184 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/expr.py
--rw-r--r--   0     1001      123    22899 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/list.py
--rw-r--r--   0     1001      123     2059 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/meta.py
--rw-r--r--   0     1001      123    44707 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/string.py
--rw-r--r--   0     1001      123     5436 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/expr/struct.py
--rw-r--r--   0     1001      123     1981 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/functions/__init__.py
--rw-r--r--   0     1001      123    29688 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/functions/eager.py
--rw-r--r--   0     1001      123    90019 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/functions/lazy.py
--rw-r--r--   0     1001      123     6293 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/functions/whenthen.py
--rw-r--r--   0     1001      123      280 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/internals.py
--rw-r--r--   0     1001      123      978 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/__init__.py
--rw-r--r--   0     1001      123     6264 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/_utils.py
--rw-r--r--   0     1001      123      878 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/avro.py
--rw-r--r--   0     1001      123      144 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/csv/__init__.py
--rw-r--r--   0     1001      123     1082 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/csv/_utils.py
--rw-r--r--   0     1001      123     4691 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/csv/batched_reader.py
--rw-r--r--   0     1001      123    35533 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/csv/functions.py
--rw-r--r--   0     1001      123     8655 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/database.py
--rw-r--r--   0     1001      123    10988 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/delta.py
--rw-r--r--   0     1001      123       75 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/excel/__init__.py
--rw-r--r--   0     1001      123    18459 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/excel/_write_utils.py
--rw-r--r--   0     1001      123     5309 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/excel/functions.py
--rw-r--r--   0     1001      123      142 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/ipc/__init__.py
--rw-r--r--   0     1001      123     1271 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/ipc/anonymous_scan.py
--rw-r--r--   0     1001      123     5840 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/ipc/functions.py
--rw-r--r--   0     1001      123      519 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/json.py
--rw-r--r--   0     1001      123     2257 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/ndjson.py
--rw-r--r--   0     1001      123      170 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/parquet/__init__.py
--rw-r--r--   0     1001      123     1299 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/parquet/anonymous_scan.py
--rw-r--r--   0     1001      123     7212 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/parquet/functions.py
--rw-r--r--   0     1001      123      136 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/pyarrow_dataset/__init__.py
--rw-r--r--   0     1001      123     2331 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/pyarrow_dataset/anonymous_scan.py
--rw-r--r--   0     1001      123     3611 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/io/pyarrow_dataset/functions.py
--rw-r--r--   0     1001      123       77 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/lazyframe/__init__.py
--rw-r--r--   0     1001      123   166918 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/lazyframe/frame.py
--rw-r--r--   0     1001      123    24010 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/lazyframe/groupby.py
--rw-r--r--   0     1001      123        0 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/py.typed
--rw-r--r--   0     1001      123       69 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/__init__.py
--rw-r--r--   0     1001      123     1579 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/_numpy.py
--rw-r--r--   0     1001      123     1920 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/binary.py
--rw-r--r--   0     1001      123     1699 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/categorical.py
--rw-r--r--   0     1001      123    47287 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/datetime.py
--rw-r--r--   0     1001      123    12385 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/list.py
--rw-r--r--   0     1001      123   162618 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/series.py
--rw-r--r--   0     1001      123    27401 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/string.py
--rw-r--r--   0     1001      123     2287 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/struct.py
--rw-r--r--   0     1001      123     5375 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/series/utils.py
--rw-r--r--   0     1001      123     7638 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/slice.py
--rw-r--r--   0     1001      123       75 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/sql/__init__.py
--rw-r--r--   0     1001      123     1351 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/sql/context.py
--rw-r--r--   0     1001      123     4764 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/string_cache.py
--rw-r--r--   0     1001      123      362 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/__init__.py
--rw-r--r--   0     1001      123      929 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/_private.py
--rw-r--r--   0     1001      123     3689 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/_tempdir.py
--rw-r--r--   0     1001      123    13597 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/asserts.py
--rw-r--r--   0     1001      123     1380 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/parametric/__init__.py
--rw-r--r--   0     1001      123    23137 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/parametric/primitives.py
--rw-r--r--   0     1001      123     2860 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/testing/parametric/strategies.py
--rw-r--r--   0     1001      123     5681 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/type_aliases.py
--rw-r--r--   0     1001      123     1167 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/__init__.py
--rw-r--r--   0     1001      123    50687 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/_construction.py
--rw-r--r--   0     1001      123     2782 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/_parse_expr_input.py
--rw-r--r--   0     1001      123      721 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/_scan.py
--rw-r--r--   0     1001      123      687 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/_wrap.py
--rw-r--r--   0     1001      123      683 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/build_info.py
--rw-r--r--   0     1001      123     9483 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/convert.py
--rw-r--r--   0     1001      123     5789 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/decorators.py
--rw-r--r--   0     1001      123     1660 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/meta.py
--rw-r--r--   0     1001      123      514 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/polars_version.py
--rw-r--r--   0     1001      123     2339 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/show_versions.py
--rw-r--r--   0     1001      123    11592 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/polars/utils/various.py
--rw-r--r--   0     1001      123     5325 2023-04-17 15:57:55.000000 polars_lts_cpu-0.17.5/pyproject.toml
--rw-r--r--   0     1001      123      699 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/requirements-dev.txt
--rw-r--r--   0     1001      123       70 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/requirements-lint.txt
--rw-r--r--   0     1001      123     1640 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/scripts/check_stacklevels.py
--rw-r--r--   0     1001      123    10959 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/apply/dataframe.rs
--rw-r--r--   0     1001      123     8388 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/apply/mod.rs
--rw-r--r--   0     1001      123    71436 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/apply/series.rs
--rw-r--r--   0     1001      123       32 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/arrow_interop/mod.rs
--rw-r--r--   0     1001      123     1306 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/arrow_interop/to_py.rs
--rw-r--r--   0     1001      123     3906 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/arrow_interop/to_rust.rs
--rw-r--r--   0     1001      123     5214 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/batched_csv.rs
--rw-r--r--   0     1001      123    47168 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/conversion.rs
--rw-r--r--   0     1001      123    45433 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/dataframe.rs
--rw-r--r--   0     1001      123     3799 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/datatypes.rs
--rw-r--r--   0     1001      123     3288 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/error.rs
--rw-r--r--   0     1001      123     9482 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/file.rs
--rw-r--r--   0     1001      123     7468 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lazy/apply.rs
--rw-r--r--   0     1001      123    33479 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lazy/dataframe.rs
--rw-r--r--   0     1001      123    62595 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lazy/dsl.rs
--rw-r--r--   0     1001      123     1082 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lazy/meta.rs
--rw-r--r--   0     1001      123      727 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lazy/mod.rs
--rw-r--r--   0     1001      123      212 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lazy/utils.rs
--rw-r--r--   0     1001      123    21002 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/lib.rs
--rw-r--r--   0     1001      123     7902 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/npy.rs
--rw-r--r--   0     1001      123     1029 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/object.rs
--rw-r--r--   0     1001      123      122 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/prelude.rs
--rw-r--r--   0     1001      123      435 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/py_modules.rs
--rw-r--r--   0     1001      123    54504 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/series.rs
--rw-r--r--   0     1001      123     3478 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/set.rs
--rw-r--r--   0     1001      123      843 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/sql.rs
--rw-r--r--   0     1001      123     2335 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/src/utils.rs
--rw-r--r--   0     1001      123     6165 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/README.md
--rw-r--r--   0     1001      123     2189 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/benchmark/groupby-datagen.R
--rw-r--r--   0     1001      123     7945 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/benchmark/run_h2oai_benchmark.py
--rw-r--r--   0     1001      123     5721 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/benchmark/test_release.py
--rw-r--r--   0     1001      123     4589 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/docs/run_doctest.py
--rw-r--r--   0     1001      123     3707 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/parametric/test_dataframe.py
--rw-r--r--   0     1001      123     1692 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/parametric/test_lazyframe.py
--rw-r--r--   0     1001      123     5709 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/parametric/test_series.py
--rw-r--r--   0     1001      123     7395 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/parametric/test_testing.py
--rw-r--r--   0     1001      123        0 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/__init__.py
--rw-r--r--   0     1001      123     3382 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/conftest.py
--rw-r--r--   0     1001      123       86 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/__init__.py
--rw-r--r--   0     1001      123      351 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_binary.py
--rw-r--r--   0     1001      123     1420 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_bool.py
--rw-r--r--   0     1001      123    11730 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_categorical.py
--rw-r--r--   0     1001      123     2766 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_decimal.py
--rw-r--r--   0     1001      123      280 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_duration.py
--rw-r--r--   0     1001      123    14355 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_list.py
--rw-r--r--   0     1001      123      284 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_null.py
--rw-r--r--   0     1001      123     2801 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_object.py
--rw-r--r--   0     1001      123    29370 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_struct.py
--rw-r--r--   0     1001      123    91453 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/datatypes/test_temporal.py
--rw-r--r--   0     1001      123      218 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/conftest.py
--rw-r--r--   0     1001      123       16 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
--rw-r--r--   0     1001      123       16 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
--rw-r--r--   0     1001      123       16 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
--rw-r--r--   0     1001      123      905 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
--rw-r--r--   0     1001      123      936 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
--rw-r--r--   0     1001      123      972 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
--rw-r--r--   0     1001      123      690 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
--rw-r--r--   0     1001      123        0 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/empty.csv
--rw-r--r--   0     1001      123     5959 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/example.xlsx
--rw-r--r--   0     1001      123      457 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.csv
--rw-r--r--   0     1001      123     2351 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.ipc
--rw-r--r--   0     1001      123     1713 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.ndjson
--rw-r--r--   0     1001      123     1427 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.parquet
--rw-r--r--   0     1001      123      455 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.csv
--rw-r--r--   0     1001      123     2351 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.ipc
--rw-r--r--   0     1001      123     1711 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.ndjson
--rw-r--r--   0     1001      123     1916 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.parquet
--rw-r--r--   0     1001      123      455 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods3.csv
--rw-r--r--   0     1001      123      457 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods4.csv
--rw-r--r--   0     1001      123      452 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/foods5.csv
--rw-r--r--   0     1001      123       49 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/gzipped.csv
--rw-r--r--   0     1001      123       57 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/small.csv
--rw-r--r--   0     1001      123      756 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/files/small.parquet
--rw-r--r--   0     1001      123     1937 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_avro.py
--rw-r--r--   0     1001      123    39029 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_csv.py
--rw-r--r--   0     1001      123     6360 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_database.py
--rw-r--r--   0     1001      123     3456 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_delta.py
--rw-r--r--   0     1001      123    11067 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_excel.py
--rw-r--r--   0     1001      123     5919 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_ipc.py
--rw-r--r--   0     1001      123     3391 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_json.py
--rw-r--r--   0     1001      123     6849 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_csv.py
--rw-r--r--   0     1001      123     2060 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_ipc.py
--rw-r--r--   0     1001      123     2881 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_json.py
--rw-r--r--   0     1001      123    11849 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_parquet.py
--rw-r--r--   0     1001      123     2012 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_other.py
--rw-r--r--   0     1001      123    13315 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_parquet.py
--rw-r--r--   0     1001      123      612 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_pickle.py
--rw-r--r--   0     1001      123     3259 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/io/test_pyarrow_dataset.py
--rw-r--r--   0     1001      123      509 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/__init__.py
--rw-r--r--   0     1001      123     3218 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_binary.py
--rw-r--r--   0     1001      123     2489 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_categorical.py
--rw-r--r--   0     1001      123    15436 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_datetime.py
--rw-r--r--   0     1001      123    12750 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_list.py
--rw-r--r--   0     1001      123     1748 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_meta.py
--rw-r--r--   0     1001      123    23698 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_string.py
--rw-r--r--   0     1001      123    15767 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_strptime.py
--rw-r--r--   0     1001      123      982 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/namespaces/test_struct.py
--rw-r--r--   0     1001      123       85 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/__init__.py
--rw-r--r--   0     1001      123     6238 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_aggregations.py
--rw-r--r--   0     1001      123     9412 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_apply.py
--rw-r--r--   0     1001      123     4390 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_arithmetic.py
--rw-r--r--   0     1001      123      956 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_comparison.py
--rw-r--r--   0     1001      123     2906 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_drop.py
--rw-r--r--   0     1001      123     7840 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_explode.py
--rw-r--r--   0     1001      123     3908 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_filter.py
--rw-r--r--   0     1001      123     1801 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_folds.py
--rw-r--r--   0     1001      123    22696 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_groupby.py
--rw-r--r--   0     1001      123    16937 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_join.py
--rw-r--r--   0     1001      123    10467 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_join_asof.py
--rw-r--r--   0     1001      123      643 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_melt.py
--rw-r--r--   0     1001      123    10253 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_pivot.py
--rw-r--r--   0     1001      123    18639 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_rolling.py
--rw-r--r--   0     1001      123    19550 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_sort.py
--rw-r--r--   0     1001      123     3643 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_statistics.py
--rw-r--r--   0     1001      123     3631 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_transpose.py
--rw-r--r--   0     1001      123      771 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_unique.py
--rw-r--r--   0     1001      123     9814 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/operations/test_window.py
--rw-r--r--   0     1001      123     4775 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_api.py
--rw-r--r--   0     1001      123     1077 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_arity.py
--rw-r--r--   0     1001      123    19908 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_cfg.py
--rw-r--r--   0     1001      123    39286 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_constructors.py
--rw-r--r--   0     1001      123      454 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_context.py
--rw-r--r--   0     1001      123     1628 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_cse.py
--rw-r--r--   0     1001      123     3497 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_datatypes.py
--rw-r--r--   0     1001      123   120947 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_df.py
--rw-r--r--   0     1001      123     1009 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_empty.py
--rw-r--r--   0     1001      123    15839 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_errors.py
--rw-r--r--   0     1001      123     2387 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_expr_multi_cols.py
--rw-r--r--   0     1001      123    32643 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_exprs.py
--rw-r--r--   0     1001      123     3305 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_fmt.py
--rw-r--r--   0     1001      123    11301 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_functions.py
--rw-r--r--   0     1001      123     3763 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_interchange.py
--rw-r--r--   0     1001      123    32596 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_interop.py
--rw-r--r--   0     1001      123    49534 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_lazy.py
--rw-r--r--   0     1001      123     2369 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_polars_import.py
--rw-r--r--   0     1001      123     4014 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_predicates.py
--rw-r--r--   0     1001      123     6995 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_projections.py
--rw-r--r--   0     1001      123    11550 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_queries.py
--rw-r--r--   0     1001      123     4743 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_rows.py
--rw-r--r--   0     1001      123    10976 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_schema.py
--rw-r--r--   0     1001      123     2441 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_serde.py
--rw-r--r--   0     1001      123    83973 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_series.py
--rw-r--r--   0     1001      123     2561 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_sql.py
--rw-r--r--   0     1001      123    13877 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_streaming.py
--rw-r--r--   0     1001      123    10700 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/test_testing.py
--rw-r--r--   0     1001      123       41 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/utils/__init__.py
--rw-r--r--   0     1001      123      306 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/utils/test_build_info.py
--rw-r--r--   0     1001      123      247 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/utils/test_show_versions.py
--rw-r--r--   0     1001      123     4307 2023-04-17 15:57:54.000000 polars_lts_cpu-0.17.5/tests/unit/utils/test_utils.py
--rw-r--r--   0     1001      123    64032 2023-04-17 15:59:00.000000 polars_lts_cpu-0.17.5/Cargo.lock
--rw-r--r--   0        0        0    14383 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.5/PKG-INFO
+-rw-r--r--   0        0        0      940 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/LICENSE
+-rw-r--r--   0     1001      123     8985 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encode.rs
+-rw-r--r--   0     1001      123     4591 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encodings/fixed.rs
+-rw-r--r--   0     1001      123       47 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encodings/mod.rs
+-rw-r--r--   0     1001      123     4508 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encodings/variable.rs
+-rw-r--r--   0     1001      123    13678 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/lib.rs
+-rw-r--r--   0     1001      123     2079 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/row.rs
+-rw-r--r--   0     1001      123      682 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/utils.rs
+-rw-r--r--   0        0        0      476 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/LICENSE
+-rw-r--r--   0     1001      123     2645 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/arena.rs
+-rw-r--r--   0     1001      123     1373 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/atomic.rs
+-rw-r--r--   0     1001      123     2659 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/cell.rs
+-rw-r--r--   0     1001      123     1015 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/contention_pool.rs
+-rw-r--r--   0     1001      123      509 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/error.rs
+-rw-r--r--   0     1001      123      271 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/fmt.rs
+-rw-r--r--   0     1001      123      763 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/functions.rs
+-rw-r--r--   0     1001      123      514 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/hash.rs
+-rw-r--r--   0     1001      123     2709 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/iter/enumerate_idx.rs
+-rw-r--r--   0     1001      123       61 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/iter/mod.rs
+-rw-r--r--   0     1001      123      583 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/lib.rs
+-rw-r--r--   0     1001      123      573 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/macros.rs
+-rw-r--r--   0     1001      123      282 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/mem.rs
+-rw-r--r--   0     1001      123     1792 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/slice.rs
+-rw-r--r--   0     1001      123     2467 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/sort.rs
+-rw-r--r--   0     1001      123     1115 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/sync.rs
+-rw-r--r--   0     1001      123      504 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/sys.rs
+-rw-r--r--   0     1001      123      697 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/unwrap.rs
+-rw-r--r--   0     1001      123      616 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/wasm.rs
+-rw-r--r--   0        0        0     5241 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/LICENSE
+-rw-r--r--   0     1001      123       45 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/constants.rs
+-rw-r--r--   0     1001      123    17248 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dot.rs
+-rw-r--r--   0     1001      123     4171 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/arithmetic.rs
+-rw-r--r--   0     1001      123      935 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/binary.rs
+-rw-r--r--   0     1001      123      650 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/cat.rs
+-rw-r--r--   0     1001      123     9424 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/dt.rs
+-rw-r--r--   0     1001      123    13169 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/expr.rs
+-rw-r--r--   0     1001      123      753 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/from.rs
+-rw-r--r--   0     1001      123       85 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/abs.rs
+-rw-r--r--   0     1001      123     1431 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs
+-rw-r--r--   0     1001      123     1327 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs
+-rw-r--r--   0     1001      123     4221 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs
+-rw-r--r--   0     1001      123     1910 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs
+-rw-r--r--   0     1001      123     1216 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs
+-rw-r--r--   0     1001      123      344 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/clip.rs
+-rw-r--r--   0     1001      123     1593 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs
+-rw-r--r--   0     1001      123    13227 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs
+-rw-r--r--   0     1001      123      810 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs
+-rw-r--r--   0     1001      123     2541 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/fill_null.rs
+-rw-r--r--   0     1001      123     8119 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/list.rs
+-rw-r--r--   0     1001      123      581 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/log.rs
+-rw-r--r--   0     1001      123    19145 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs
+-rw-r--r--   0     1001      123      462 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/nan.rs
+-rw-r--r--   0     1001      123     3132 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs
+-rw-r--r--   0     1001      123      152 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/rolling.rs
+-rw-r--r--   0     1001      123      260 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/round.rs
+-rw-r--r--   0     1001      123      200 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/row_hash.rs
+-rw-r--r--   0     1001      123    13416 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs
+-rw-r--r--   0     1001      123      306 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/search_sorted.rs
+-rw-r--r--   0     1001      123     3812 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs
+-rw-r--r--   0     1001      123     1238 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs
+-rw-r--r--   0     1001      123      972 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs
+-rw-r--r--   0     1001      123    19641 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs
+-rw-r--r--   0     1001      123     1017 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs
+-rw-r--r--   0     1001      123     2700 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs
+-rw-r--r--   0     1001      123     5122 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs
+-rw-r--r--   0     1001      123      170 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/unique.rs
+-rw-r--r--   0     1001      123    43864 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/functions.rs
+-rw-r--r--   0     1001      123    10196 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2181 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/meta.rs
+-rw-r--r--   0     1001      123    64804 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/mod.rs
+-rw-r--r--   0     1001      123       40 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/names.rs
+-rw-r--r--   0     1001      123     2100 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/options.rs
+-rw-r--r--   0     1001      123    14993 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/string.rs
+-rw-r--r--   0     1001      123     2715 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/struct_.rs
+-rw-r--r--   0     1001      123       38 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/frame/mod.rs
+-rw-r--r--   0     1001      123      933 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/frame/opt_state.rs
+-rw-r--r--   0     1001      123      466 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/global.rs
+-rw-r--r--   0     1001      123      175 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/lib.rs
+-rw-r--r--   0     1001      123     6825 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs
+-rw-r--r--   0     1001      123    11393 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs
+-rw-r--r--   0     1001      123    25656 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/alp.rs
+-rw-r--r--   0     1001      123     1622 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs
+-rw-r--r--   0     1001      123     1428 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/apply.rs
+-rw-r--r--   0     1001      123    24898 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/builder.rs
+-rw-r--r--   0     1001      123    29652 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/conversion.rs
+-rw-r--r--   0     1001      123      301 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/debug.rs
+-rw-r--r--   0     1001      123    15191 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/format.rs
+-rw-r--r--   0     1001      123      895 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs
+-rw-r--r--   0     1001      123      137 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/explode.rs
+-rw-r--r--   0     1001      123     1169 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs
+-rw-r--r--   0     1001      123    11905 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs
+-rw-r--r--   0     1001      123     1330 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs
+-rw-r--r--   0     1001      123     9752 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/iterator.rs
+-rw-r--r--   0     1001      123    10463 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/lit.rs
+-rw-r--r--   0     1001      123     8115 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/mod.rs
+-rw-r--r--   0     1001      123     7416 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs
+-rw-r--r--   0     1001      123    15277 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs
+-rw-r--r--   0     1001      123     3250 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs
+-rw-r--r--   0     1001      123     3236 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs
+-rw-r--r--   0     1001      123     3994 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs
+-rw-r--r--   0     1001      123    14479 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs
+-rw-r--r--   0     1001      123     1556 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs
+-rw-r--r--   0     1001      123     6644 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs
+-rw-r--r--   0     1001      123     1222 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs
+-rw-r--r--   0     1001      123    28276 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2571 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs
+-rw-r--r--   0     1001      123    15130 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs
+-rw-r--r--   0     1001      123     1755 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs
+-rw-r--r--   0     1001      123     3930 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs
+-rw-r--r--   0     1001      123     1799 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs
+-rw-r--r--   0     1001      123     3269 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs
+-rw-r--r--   0     1001      123     2638 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs
+-rw-r--r--   0     1001      123    15747 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs
+-rw-r--r--   0     1001      123    26502 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs
+-rw-r--r--   0     1001      123     2692 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs
+-rw-r--r--   0     1001      123     2639 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs
+-rw-r--r--   0     1001      123     3501 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs
+-rw-r--r--   0     1001      123    27361 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs
+-rw-r--r--   0     1001      123     3492 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs
+-rw-r--r--   0     1001      123    13845 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs
+-rw-r--r--   0     1001      123     3161 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs
+-rw-r--r--   0     1001      123     9725 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs
+-rw-r--r--   0     1001      123    19820 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs
+-rw-r--r--   0     1001      123    10187 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/options.rs
+-rw-r--r--   0     1001      123    15276 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/projection.rs
+-rw-r--r--   0     1001      123     4615 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs
+-rw-r--r--   0     1001      123    13038 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/schema.rs
+-rw-r--r--   0     1001      123      809 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/prelude.rs
+-rw-r--r--   0     1001      123    11879 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/utils.rs
+-rw-r--r--   0        0        0      823 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-algo/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-algo/LICENSE
+-rw-r--r--   0     1001      123     7265 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-algo/src/algo.rs
+-rw-r--r--   0     1001      123       88 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-algo/src/lib.rs
+-rw-r--r--   0     1001      123       28 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-algo/src/prelude.rs
+-rw-r--r--   0        0        0      879 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-error/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-error/LICENSE
+-rw-r--r--   0     1001      123     6297 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-error/src/lib.rs
+-rw-r--r--   0        0        0     2055 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/LICENSE
+-rw-r--r--   0     1001      123     3565 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/date.rs
+-rw-r--r--   0     1001      123     6465 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/datetime.rs
+-rw-r--r--   0     1001      123     3305 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/duration.rs
+-rw-r--r--   0     1001      123     5607 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/kernels.rs
+-rw-r--r--   0     1001      123     1062 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/mod.rs
+-rw-r--r--   0     1001      123     7302 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs
+-rw-r--r--   0     1001      123     2582 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs
+-rw-r--r--   0     1001      123    10476 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs
+-rw-r--r--   0     1001      123      428 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/mod.rs
+-rw-r--r--   0     1001      123     7368 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs
+-rw-r--r--   0     1001      123     2717 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/time.rs
+-rw-r--r--   0     1001      123    21192 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs
+-rw-r--r--   0     1001      123    20108 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs
+-rw-r--r--   0     1001      123     4115 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs
+-rw-r--r--   0     1001      123     9692 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs
+-rw-r--r--   0     1001      123     2960 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/date_range.rs
+-rw-r--r--   0     1001      123    31413 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/groupby/dynamic.rs
+-rw-r--r--   0     1001      123       88 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/groupby/mod.rs
+-rw-r--r--   0     1001      123      535 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/lib.rs
+-rw-r--r--   0     1001      123      320 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/prelude.rs
+-rw-r--r--   0     1001      123     1568 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/round.rs
+-rw-r--r--   0     1001      123     4028 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/_trait.rs
+-rw-r--r--   0     1001      123      136 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123      140 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/categoricals.rs
+-rw-r--r--   0     1001      123      133 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/date.rs
+-rw-r--r--   0     1001      123      137 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123      137 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123     1863 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     1792 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/integers.rs
+-rw-r--r--   0     1001      123      133 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123      486 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123      155 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123      135 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123      133 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/time.rs
+-rw-r--r--   0     1001      123      133 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123    12466 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/mod.rs
+-rw-r--r--   0     1001      123     1630 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/truncate.rs
+-rw-r--r--   0     1001      123     7059 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/upsample.rs
+-rw-r--r--   0     1001      123     2567 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/utils.rs
+-rw-r--r--   0     1001      123     1524 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/bounds.rs
+-rw-r--r--   0     1001      123     2008 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/calendar.rs
+-rw-r--r--   0     1001      123    23538 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/duration.rs
+-rw-r--r--   0     1001      123    20089 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/groupby.rs
+-rw-r--r--   0     1001      123      503 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/mod.rs
+-rw-r--r--   0     1001      123    24202 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/test.rs
+-rw-r--r--   0     1001      123    11624 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/window.rs
+-rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/LICENSE
+-rw-r--r--   0     1001      123     1975 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/default_arrays.rs
+-rw-r--r--   0     1001      123     3160 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/get.rs
+-rw-r--r--   0     1001      123     6171 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/list.rs
+-rw-r--r--   0     1001      123     7771 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/mod.rs
+-rw-r--r--   0     1001      123      878 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/null.rs
+-rw-r--r--   0     1001      123     1125 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/slice.rs
+-rw-r--r--   0     1001      123     1807 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/utf8.rs
+-rw-r--r--   0     1001      123     2294 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/bit_util.rs
+-rw-r--r--   0     1001      123       17 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/bitmap/mod.rs
+-rw-r--r--   0     1001      123      819 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/bitmap/mutable.rs
+-rw-r--r--   0     1001      123      232 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/compute/cast.rs
+-rw-r--r--   0     1001      123       56 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/compute/mod.rs
+-rw-r--r--   0     1001      123     2962 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/compute/take/boolean.rs
+-rw-r--r--   0     1001      123    24907 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/compute/take/mod.rs
+-rw-r--r--   0     1001      123     1042 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/conversion.rs
+-rw-r--r--   0     1001      123     1609 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/data_types.rs
+-rw-r--r--   0     1001      123       25 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/error.rs
+-rw-r--r--   0     1001      123       28 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/export.rs
+-rw-r--r--   0     1001      123       26 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/floats/mod.rs
+-rw-r--r--   0     1001      123     2066 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/floats/ord.rs
+-rw-r--r--   0     1001      123     1273 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/index.rs
+-rw-r--r--   0     1001      123      915 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/is_valid.rs
+-rw-r--r--   0     1001      123     4740 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/agg_mean.rs
+-rw-r--r--   0     1001      123     1015 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/concatenate.rs
+-rw-r--r--   0     1001      123     5161 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/average.rs
+-rw-r--r--   0     1001      123     1808 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs
+-rw-r--r--   0     1001      123    25065 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs
+-rw-r--r--   0     1001      123     1406 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/float.rs
+-rw-r--r--   0     1001      123     4907 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/list.rs
+-rw-r--r--   0     1001      123     1895 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs
+-rw-r--r--   0     1001      123     9731 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/mod.rs
+-rw-r--r--   0     1001      123     3703 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs
+-rw-r--r--   0     1001      123     2022 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs
+-rw-r--r--   0     1001      123    18684 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs
+-rw-r--r--   0     1001      123     3924 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs
+-rw-r--r--   0     1001      123    11659 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs
+-rw-r--r--   0     1001      123     5504 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs
+-rw-r--r--   0     1001      123     8683 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs
+-rw-r--r--   0     1001      123     1749 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs
+-rw-r--r--   0     1001      123    14367 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs
+-rw-r--r--   0     1001      123     9070 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs
+-rw-r--r--   0     1001      123    11609 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs
+-rw-r--r--   0     1001      123     4698 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs
+-rw-r--r--   0     1001      123     8335 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs
+-rw-r--r--   0     1001      123     8109 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/window.rs
+-rw-r--r--   0     1001      123     4752 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/set.rs
+-rw-r--r--   0     1001      123     4529 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sort_partition.rs
+-rw-r--r--   0     1001      123     2948 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs
+-rw-r--r--   0     1001      123     5974 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs
+-rw-r--r--   0     1001      123      231 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/mod.rs
+-rw-r--r--   0     1001      123      841 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/string.rs
+-rw-r--r--   0     1001      123     2310 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs
+-rw-r--r--   0     1001      123     4343 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs
+-rw-r--r--   0     1001      123     2606 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs
+-rw-r--r--   0     1001      123     4417 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/time.rs
+-rw-r--r--   0     1001      123      341 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/lib.rs
+-rw-r--r--   0     1001      123      434 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/prelude.rs
+-rw-r--r--   0     1001      123      534 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/slice.rs
+-rw-r--r--   0     1001      123      762 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/time_zone.rs
+-rw-r--r--   0     1001      123      998 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/boolean.rs
+-rw-r--r--   0     1001      123     2821 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/mod.rs
+-rw-r--r--   0     1001      123     2533 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs
+-rw-r--r--   0     1001      123      158 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/rev.rs
+-rw-r--r--   0     1001      123     5020 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/utils.rs
+-rw-r--r--   0        0        0     4341 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/LICENSE
+-rw-r--r--   0     1001      123     2383 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/avro/mod.rs
+-rw-r--r--   0     1001      123     3608 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/avro/read.rs
+-rw-r--r--   0     1001      123     2622 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/avro/write.rs
+-rw-r--r--   0     1001      123     4505 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/cloud/adaptors.rs
+-rw-r--r--   0     1001      123     9506 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/cloud/glob.rs
+-rw-r--r--   0     1001      123     3089 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/cloud/mod.rs
+-rw-r--r--   0     1001      123    28678 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/buffer.rs
+-rw-r--r--   0     1001      123     1898 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/mod.rs
+-rw-r--r--   0     1001      123    19712 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/parser.rs
+-rw-r--r--   0     1001      123    21432 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read.rs
+-rw-r--r--   0     1001      123    10817 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs
+-rw-r--r--   0     1001      123    13909 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs
+-rw-r--r--   0     1001      123    31242 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read_impl/mod.rs
+-rw-r--r--   0     1001      123    11466 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/splitfields.rs
+-rw-r--r--   0     1001      123    25183 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/utils.rs
+-rw-r--r--   0     1001      123     2796 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/write.rs
+-rw-r--r--   0     1001      123    13265 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/write_impl.rs
+-rw-r--r--   0     1001      123      184 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/export.rs
+-rw-r--r--   0     1001      123     7586 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/ipc_file.rs
+-rw-r--r--   0     1001      123     9222 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/ipc_stream.rs
+-rw-r--r--   0     1001      123     3253 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/mmap.rs
+-rw-r--r--   0     1001      123      401 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/mod.rs
+-rw-r--r--   0     1001      123     8282 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/write.rs
+-rw-r--r--   0     1001      123     1471 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/write_async.rs
+-rw-r--r--   0     1001      123    11046 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/json.rs
+-rw-r--r--   0     1001      123     4864 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/lib.rs
+-rw-r--r--   0     1001      123     1969 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/mmap.rs
+-rw-r--r--   0     1001      123     7215 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ndjson_core/buffer.rs
+-rw-r--r--   0     1001      123       39 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ndjson_core/mod.rs
+-rw-r--r--   0     1001      123    12172 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ndjson_core/ndjson.rs
+-rw-r--r--   0     1001      123      273 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/options.rs
+-rw-r--r--   0     1001      123     7360 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/async_impl.rs
+-rw-r--r--   0     1001      123     3093 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/mmap.rs
+-rw-r--r--   0     1001      123     3132 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/mod.rs
+-rw-r--r--   0     1001      123     4784 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/predicates.rs
+-rw-r--r--   0     1001      123     9606 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/read.rs
+-rw-r--r--   0     1001      123    16886 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/read_impl.rs
+-rw-r--r--   0     1001      123    10106 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/write.rs
+-rw-r--r--   0     1001      123     5334 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/partition.rs
+-rw-r--r--   0     1001      123     1455 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/predicates.rs
+-rw-r--r--   0     1001      123      628 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/prelude.rs
+-rw-r--r--   0     1001      123      417 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/tests.rs
+-rw-r--r--   0     1001      123     4467 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/utils.rs
+-rw-r--r--   0        0        0     5407 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/LICENSE
+-rw-r--r--   0     1001      123    19606 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/arithmetic.rs
+-rw-r--r--   0     1001      123     8679 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/bitwise.rs
+-rw-r--r--   0     1001      123     2298 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/binary.rs
+-rw-r--r--   0     1001      123     1207 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs
+-rw-r--r--   0     1001      123     1556 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/from.rs
+-rw-r--r--   0     1001      123    20366 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/list.rs
+-rw-r--r--   0     1001      123     8845 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/mod.rs
+-rw-r--r--   0     1001      123     1410 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs
+-rw-r--r--   0     1001      123     2291 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs
+-rw-r--r--   0     1001      123    11560 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/cast.rs
+-rw-r--r--   0     1001      123    48300 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs
+-rw-r--r--   0     1001      123     9463 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs
+-rw-r--r--   0     1001      123      551 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/drop.rs
+-rw-r--r--   0     1001      123      963 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/float.rs
+-rw-r--r--   0     1001      123     5069 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/from.rs
+-rw-r--r--   0     1001      123    38411 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs
+-rw-r--r--   0     1001      123     1395 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs
+-rw-r--r--   0     1001      123       28 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/mod.rs
+-rw-r--r--   0     1001      123     1129 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs
+-rw-r--r--   0     1001      123       21 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/kernels/mod.rs
+-rw-r--r--   0     1001      123     2986 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/kernels/take.rs
+-rw-r--r--   0     1001      123     7728 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/list/iterator.rs
+-rw-r--r--   0     1001      123     2802 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    19796 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs
+-rw-r--r--   0     1001      123     3688 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs
+-rw-r--r--   0     1001      123     4270 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs
+-rw-r--r--   0     1001      123    10220 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs
+-rw-r--r--   0     1001      123     1400 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs
+-rw-r--r--   0     1001      123      358 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/full.rs
+-rw-r--r--   0     1001      123      192 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/mod.rs
+-rw-r--r--   0     1001      123     2731 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs
+-rw-r--r--   0     1001      123     2172 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs
+-rw-r--r--   0     1001      123      925 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs
+-rw-r--r--   0     1001      123     6453 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs
+-rw-r--r--   0     1001      123     1604 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/date.rs
+-rw-r--r--   0     1001      123     4105 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs
+-rw-r--r--   0     1001      123     4443 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs
+-rw-r--r--   0     1001      123     2434 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/duration.rs
+-rw-r--r--   0     1001      123     2549 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/mod.rs
+-rw-r--r--   0     1001      123      476 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/from.rs
+-rw-r--r--   0     1001      123    15081 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/time.rs
+-rw-r--r--   0     1001      123    23524 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     7200 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ndarray.rs
+-rw-r--r--   0     1001      123     4484 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/builder.rs
+-rw-r--r--   0     1001      123     1547 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs
+-rw-r--r--   0     1001      123     3124 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs
+-rw-r--r--   0     1001      123     7054 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs
+-rw-r--r--   0     1001      123     3410 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs
+-rw-r--r--   0     1001      123      137 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/is_valid.rs
+-rw-r--r--   0     1001      123     4419 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/iterator.rs
+-rw-r--r--   0     1001      123     4826 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/mod.rs
+-rw-r--r--   0     1001      123     2853 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/registry.rs
+-rw-r--r--   0     1001      123      272 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/abs.rs
+-rw-r--r--   0     1001      123    32120 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs
+-rw-r--r--   0     1001      123     9946 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs
+-rw-r--r--   0     1001      123     2875 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs
+-rw-r--r--   0     1001      123     9670 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs
+-rw-r--r--   0     1001      123     2365 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/append.rs
+-rw-r--r--   0     1001      123    27269 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/apply.rs
+-rw-r--r--   0     1001      123    12799 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs
+-rw-r--r--   0     1001      123     6214 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs
+-rw-r--r--   0     1001      123    11537 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs
+-rw-r--r--   0     1001      123     1737 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs
+-rw-r--r--   0     1001      123     4801 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs
+-rw-r--r--   0     1001      123     6264 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs
+-rw-r--r--   0     1001      123    25614 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/explode.rs
+-rw-r--r--   0     1001      123     8339 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/extend.rs
+-rw-r--r--   0     1001      123    13777 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs
+-rw-r--r--   0     1001      123     5308 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/filter.rs
+-rw-r--r--   0     1001      123     4436 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/full.rs
+-rw-r--r--   0     1001      123        1 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/interpolate.rs
+-rw-r--r--   0     1001      123    15385 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs
+-rw-r--r--   0     1001      123        1 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/len.rs
+-rw-r--r--   0     1001      123    22376 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/mod.rs
+-rw-r--r--   0     1001      123     2403 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs
+-rw-r--r--   0     1001      123      593 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs
+-rw-r--r--   0     1001      123     2585 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs
+-rw-r--r--   0     1001      123     1539 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs
+-rw-r--r--   0     1001      123    10234 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs
+-rw-r--r--   0     1001      123    12518 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/set.rs
+-rw-r--r--   0     1001      123     6151 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/shift.rs
+-rw-r--r--   0     1001      123     2299 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs
+-rw-r--r--   0     1001      123     5467 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs
+-rw-r--r--   0     1001      123     7430 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs
+-rw-r--r--   0     1001      123    30762 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs
+-rw-r--r--   0     1001      123      380 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/slice.rs
+-rw-r--r--   0     1001      123    20472 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs
+-rw-r--r--   0     1001      123     6630 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs
+-rw-r--r--   0     1001      123     1859 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs
+-rw-r--r--   0     1001      123    16256 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs
+-rw-r--r--   0     1001      123     5041 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs
+-rw-r--r--   0     1001      123     6064 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs
+-rw-r--r--   0     1001      123    11229 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs
+-rw-r--r--   0     1001      123    14620 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs
+-rw-r--r--   0     1001      123     7753 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/zip.rs
+-rw-r--r--   0     1001      123     9093 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/random.rs
+-rw-r--r--   0     1001      123     1959 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs
+-rw-r--r--   0     1001      123     2501 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/date.rs
+-rw-r--r--   0     1001      123    11998 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs
+-rw-r--r--   0     1001      123     3201 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs
+-rw-r--r--   0     1001      123      533 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs
+-rw-r--r--   0     1001      123     2724 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/time.rs
+-rw-r--r--   0     1001      123      872 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/to_vec.rs
+-rw-r--r--   0     1001      123     8113 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/trusted_len.rs
+-rw-r--r--   0     1001      123    25934 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs
+-rw-r--r--   0     1001      123     7689 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/cloud.rs
+-rw-r--r--   0     1001      123     1549 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/config.rs
+-rw-r--r--   0     1001      123     3946 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/_serde.rs
+-rw-r--r--   0     1001      123     2650 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/aliases.rs
+-rw-r--r--   0     1001      123    42410 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/any_value.rs
+-rw-r--r--   0     1001      123    12083 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/dtype.rs
+-rw-r--r--   0     1001      123     5422 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/field.rs
+-rw-r--r--   0     1001      123     7675 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/time_unit.rs
+-rw-r--r--   0     1001      123      118 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/mod.rs
+-rw-r--r--   0     1001      123      898 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs
+-rw-r--r--   0     1001      123      481 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_3.rs
+-rw-r--r--   0     1001      123      293 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_4.rs
+-rw-r--r--   0     1001      123      499 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_5.rs
+-rw-r--r--   0     1001      123      288 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_6.rs
+-rw-r--r--   0     1001      123     1071 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_7.rs
+-rw-r--r--   0     1001      123      819 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_8.rs
+-rw-r--r--   0     1001      123      596 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_9.rs
+-rw-r--r--   0     1001      123       43 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/mod.rs
+-rw-r--r--   0     1001      123       25 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/error.rs
+-rw-r--r--   0     1001      123      433 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/export.rs
+-rw-r--r--   0     1001      123    36116 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/fmt.rs
+-rw-r--r--   0     1001      123     5177 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/arithmetic.rs
+-rw-r--r--   0     1001      123     7874 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/asof_join/asof.rs
+-rw-r--r--   0     1001      123    33715 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/asof_join/groups.rs
+-rw-r--r--   0     1001      123     6634 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/asof_join/mod.rs
+-rw-r--r--   0     1001      123      559 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/chunks.rs
+-rw-r--r--   0     1001      123     5179 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/cross_join.rs
+-rw-r--r--   0     1001      123    16609 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/explode.rs
+-rw-r--r--   0     1001      123     1019 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/from.rs
+-rw-r--r--   0     1001      123    16518 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs
+-rw-r--r--   0     1001      123     4115 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs
+-rw-r--r--   0     1001      123     7643 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs
+-rw-r--r--   0     1001      123    39255 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs
+-rw-r--r--   0     1001      123     5636 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs
+-rw-r--r--   0     1001      123      218 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/expr.rs
+-rw-r--r--   0     1001      123    15470 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/hashing.rs
+-rw-r--r--   0     1001      123    14048 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/into_groups.rs
+-rw-r--r--   0     1001      123    39374 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/mod.rs
+-rw-r--r--   0     1001      123    10535 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/perfect.rs
+-rw-r--r--   0     1001      123    17214 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/proxy.rs
+-rw-r--r--   0     1001      123    18264 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/mod.rs
+-rw-r--r--   0     1001      123    22392 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs
+-rw-r--r--   0     1001      123     2413 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs
+-rw-r--r--   0     1001      123    16352 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs
+-rw-r--r--   0     1001      123     4295 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_inner.rs
+-rw-r--r--   0     1001      123     6076 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs
+-rw-r--r--   0     1001      123     4247 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs
+-rw-r--r--   0     1001      123     3913 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs
+-rw-r--r--   0     1001      123    11879 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs
+-rw-r--r--   0     1001      123   124236 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/mod.rs
+-rw-r--r--   0     1001      123    27513 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/av_buffer.rs
+-rw-r--r--   0     1001      123     3732 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/dataframe.rs
+-rw-r--r--   0     1001      123     5976 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/mod.rs
+-rw-r--r--   0     1001      123     8795 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/transpose.rs
+-rw-r--r--   0     1001      123     2183 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/top_k.rs
+-rw-r--r--   0     1001      123     1388 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/upstream_traits.rs
+-rw-r--r--   0     1001      123    10935 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/functions.rs
+-rw-r--r--   0     1001      123     2149 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/fx.rs
+-rw-r--r--   0     1001      123     1503 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/identity.rs
+-rw-r--r--   0     1001      123      457 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/mod.rs
+-rw-r--r--   0     1001      123     2684 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/partition.rs
+-rw-r--r--   0     1001      123    17653 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/vector_hasher.rs
+-rw-r--r--   0     1001      123     1896 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/lib.rs
+-rw-r--r--   0     1001      123    15733 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/named_from.rs
+-rw-r--r--   0     1001      123     2411 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/prelude.rs
+-rw-r--r--   0     1001      123    16406 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/schema.rs
+-rw-r--r--   0     1001      123     4218 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/serde/chunked_array.rs
+-rw-r--r--   0     1001      123     6551 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/serde/mod.rs
+-rw-r--r--   0     1001      123     9929 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/serde/series.rs
+-rw-r--r--   0     1001      123    18441 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/any_value.rs
+-rw-r--r--   0     1001      123    28511 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs
+-rw-r--r--   0     1001      123      222 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/arithmetic/mod.rs
+-rw-r--r--   0     1001      123     3546 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/arithmetic/owned.rs
+-rw-r--r--   0     1001      123    13187 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/comparison.rs
+-rw-r--r--   0     1001      123    25008 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/from.rs
+-rw-r--r--   0     1001      123     9217 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/binary.rs
+-rw-r--r--   0     1001      123    10850 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/boolean.rs
+-rw-r--r--   0     1001      123    12962 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/categorical.rs
+-rw-r--r--   0     1001      123    18304 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/dates_time.rs
+-rw-r--r--   0     1001      123    15242 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/datetime.rs
+-rw-r--r--   0     1001      123     5829 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/decimal.rs
+-rw-r--r--   0     1001      123    15106 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/duration.rs
+-rw-r--r--   0     1001      123    14223 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/floats.rs
+-rw-r--r--   0     1001      123     6207 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/list.rs
+-rw-r--r--   0     1001      123    18305 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/mod.rs
+-rw-r--r--   0     1001      123     5336 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/null.rs
+-rw-r--r--   0     1001      123     8004 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/object.rs
+-rw-r--r--   0     1001      123    11029 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/struct_.rs
+-rw-r--r--   0     1001      123     9735 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/utf8.rs
+-rw-r--r--   0     1001      123     4471 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/into.rs
+-rw-r--r--   0     1001      123     6297 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/iterator.rs
+-rw-r--r--   0     1001      123    37684 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/mod.rs
+-rw-r--r--   0     1001      123      853 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/diff.rs
+-rw-r--r--   0     1001      123     5204 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/downcast.rs
+-rw-r--r--   0     1001      123     3601 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/ewm.rs
+-rw-r--r--   0     1001      123      413 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/extend.rs
+-rw-r--r--   0     1001      123      562 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     5974 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/moment.rs
+-rw-r--r--   0     1001      123     2908 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/null.rs
+-rw-r--r--   0     1001      123     1347 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/pct_change.rs
+-rw-r--r--   0     1001      123     4247 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/round.rs
+-rw-r--r--   0     1001      123     5072 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/to_list.rs
+-rw-r--r--   0     1001      123     1476 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/unique.rs
+-rw-r--r--   0     1001      123    18204 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/series_trait.rs
+-rw-r--r--   0     1001      123     2840 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/unstable.rs
+-rw-r--r--   0     1001      123     8117 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/testing.rs
+-rw-r--r--   0     1001      123      508 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/tests.rs
+-rw-r--r--   0     1001      123     1396 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/flatten.rs
+-rw-r--r--   0     1001      123    31704 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/mod.rs
+-rw-r--r--   0     1001      123     1598 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/series.rs
+-rw-r--r--   0     1001      123    13773 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/supertype.rs
+-rw-r--r--   0        0        0     3268 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/LICENSE
+-rw-r--r--   0     1001      123      234 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/binary/mod.rs
+-rw-r--r--   0     1001      123     3549 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs
+-rw-r--r--   0     1001      123    11023 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/interpolate.rs
+-rw-r--r--   0     1001      123     1679 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/count.rs
+-rw-r--r--   0     1001      123     2452 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/hash.rs
+-rw-r--r--   0     1001      123     7861 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs
+-rw-r--r--   0     1001      123      511 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/mod.rs
+-rw-r--r--   0     1001      123    22005 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs
+-rw-r--r--   0     1001      123     5269 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs
+-rw-r--r--   0     1001      123     2435 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs
+-rw-r--r--   0     1001      123      489 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/mod.rs
+-rw-r--r--   0     1001      123     9380 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs
+-rw-r--r--   0     1001      123     6795 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/set.rs
+-rw-r--r--   0     1001      123     7490 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/case.rs
+-rw-r--r--   0     1001      123     8251 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs
+-rw-r--r--   0     1001      123     2345 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs
+-rw-r--r--   0     1001      123      514 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs
+-rw-r--r--   0     1001      123    14731 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs
+-rw-r--r--   0     1001      123     4053 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs
+-rw-r--r--   0     1001      123     2486 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/top_k.rs
+-rw-r--r--   0     1001      123     7727 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs
+-rw-r--r--   0     1001      123    18025 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/join/mod.rs
+-rw-r--r--   0     1001      123     4174 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/mod.rs
+-rw-r--r--   0     1001      123    10257 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/pivot/mod.rs
+-rw-r--r--   0     1001      123    13486 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/pivot/positioning.rs
+-rw-r--r--   0     1001      123      217 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/lib.rs
+-rw-r--r--   0     1001      123      290 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/prelude.rs
+-rw-r--r--   0     1001      123       25 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/mod.rs
+-rw-r--r--   0     1001      123     9623 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs
+-rw-r--r--   0     1001      123      118 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_algo/mod.rs
+-rw-r--r--   0     1001      123     2016 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_unique.rs
+-rw-r--r--   0     1001      123    11872 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs
+-rw-r--r--   0     1001      123     3680 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/floor_divide.rs
+-rw-r--r--   0     1001      123     3423 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/is_first.rs
+-rw-r--r--   0     1001      123     2975 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/is_unique.rs
+-rw-r--r--   0     1001      123     3626 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/log.rs
+-rw-r--r--   0     1001      123     1106 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/mod.rs
+-rw-r--r--   0     1001      123     1769 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/rolling.rs
+-rw-r--r--   0     1001      123     7642 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/search_sorted.rs
+-rw-r--r--   0     1001      123     2500 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/to_dummies.rs
+-rw-r--r--   0     1001      123     2067 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/various.rs
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/LICENSE
+-rw-r--r--   0     1001      123    15314 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/context.rs
+-rw-r--r--   0     1001      123    17592 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/functions.rs
+-rw-r--r--   0     1001      123     1920 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/keywords.rs
+-rw-r--r--   0     1001      123    28145 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/lib.rs
+-rw-r--r--   0     1001      123    15237 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/sql_expr.rs
+-rw-r--r--   0     1001      123     4572 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/table_functions.rs
+-rw-r--r--   0        0        0     5977 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/LICENSE
+-rw-r--r--   0     1001      123     1796 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dot.rs
+-rw-r--r--   0     1001      123     4359 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/eval.rs
+-rw-r--r--   0     1001      123     4505 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/functions.rs
+-rw-r--r--   0     1001      123      164 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/into.rs
+-rw-r--r--   0     1001      123     6754 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/list.rs
+-rw-r--r--   0     1001      123     2899 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/mod.rs
+-rw-r--r--   0     1001      123     1182 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs
+-rw-r--r--   0     1001      123     9278 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/csv.rs
+-rw-r--r--   0     1001      123     4309 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/file_list_reader.rs
+-rw-r--r--   0     1001      123     2261 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/ipc.rs
+-rw-r--r--   0     1001      123    47176 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/mod.rs
+-rw-r--r--   0     1001      123     3414 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/ndjson.rs
+-rw-r--r--   0     1001      123     3440 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/parquet.rs
+-rw-r--r--   0     1001      123     2892 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/pivot.rs
+-rw-r--r--   0     1001      123      416 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/python.rs
+-rw-r--r--   0     1001      123     6376 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/lib.rs
+-rw-r--r--   0     1001      123     1049 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs
+-rw-r--r--   0     1001      123      776 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs
+-rw-r--r--   0     1001      123      670 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs
+-rw-r--r--   0     1001      123     1284 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs
+-rw-r--r--   0     1001      123     3908 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs
+-rw-r--r--   0     1001      123     3577 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs
+-rw-r--r--   0     1001      123    13439 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs
+-rw-r--r--   0     1001      123     4335 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs
+-rw-r--r--   0     1001      123     6058 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs
+-rw-r--r--   0     1001      123     7074 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs
+-rw-r--r--   0     1001      123     2045 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs
+-rw-r--r--   0     1001      123     1677 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs
+-rw-r--r--   0     1001      123     2986 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs
+-rw-r--r--   0     1001      123     1963 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs
+-rw-r--r--   0     1001      123     4151 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs
+-rw-r--r--   0     1001      123     1208 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs
+-rw-r--r--   0     1001      123     2421 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs
+-rw-r--r--   0     1001      123      548 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs
+-rw-r--r--   0     1001      123     2197 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs
+-rw-r--r--   0     1001      123     1922 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs
+-rw-r--r--   0     1001      123      663 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs
+-rw-r--r--   0     1001      123     3702 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs
+-rw-r--r--   0     1001      123      838 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs
+-rw-r--r--   0     1001      123     1284 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/exotic.rs
+-rw-r--r--   0     1001      123    21873 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs
+-rw-r--r--   0     1001      123     2689 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs
+-rw-r--r--   0     1001      123    17432 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs
+-rw-r--r--   0     1001      123    17488 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs
+-rw-r--r--   0     1001      123     3153 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs
+-rw-r--r--   0     1001      123     6326 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs
+-rw-r--r--   0     1001      123     2003 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs
+-rw-r--r--   0     1001      123     5809 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs
+-rw-r--r--   0     1001      123     4131 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs
+-rw-r--r--   0     1001      123     5304 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs
+-rw-r--r--   0     1001      123    21103 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs
+-rw-r--r--   0     1001      123    10091 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs
+-rw-r--r--   0     1001      123     3929 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs
+-rw-r--r--   0     1001      123    11541 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs
+-rw-r--r--   0     1001      123     8331 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs
+-rw-r--r--   0     1001      123    14360 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs
+-rw-r--r--   0     1001      123    31819 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs
+-rw-r--r--   0     1001      123     2039 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs
+-rw-r--r--   0     1001      123      414 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/mod.rs
+-rw-r--r--   0     1001      123     2005 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs
+-rw-r--r--   0     1001      123    27366 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs
+-rw-r--r--   0     1001      123    18862 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs
+-rw-r--r--   0     1001      123       87 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/mod.rs
+-rw-r--r--   0     1001      123     9425 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/state.rs
+-rw-r--r--   0     1001      123    20891 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs
+-rw-r--r--   0     1001      123      219 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/mod.rs
+-rw-r--r--   0     1001      123     3333 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs
+-rw-r--r--   0     1001      123      722 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/prelude.rs
+-rw-r--r--   0     1001      123    14990 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/aggregations.rs
+-rw-r--r--   0     1001      123     2339 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/arity.rs
+-rw-r--r--   0     1001      123     7031 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/cse.rs
+-rw-r--r--   0     1001      123    12749 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/io.rs
+-rw-r--r--   0     1001      123     4207 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/logical.rs
+-rw-r--r--   0     1001      123     4288 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/mod.rs
+-rw-r--r--   0     1001      123    14812 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/optimization_checks.rs
+-rw-r--r--   0     1001      123     6799 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/predicate_queries.rs
+-rw-r--r--   0     1001      123     3158 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/projection_queries.rs
+-rw-r--r--   0     1001      123    47910 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/queries.rs
+-rw-r--r--   0     1001      123     8358 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/streaming.rs
+-rw-r--r--   0     1001      123     2886 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/tpch.rs
+-rw-r--r--   0     1001      123     1028 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/utils.rs
+-rw-r--r--   0        0        0    10541 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/LICENSE
+-rw-r--r--   0     1001      123     3249 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/Makefile
+-rw-r--r--   0     1001      123      215 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/build.rs
+-rw-r--r--   0     1001      123       78 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/clippy.toml
+-rw-r--r--   0     1001      123    17602 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/eager.rs
+-rw-r--r--   0     1001      123     8778 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/lazy.rs
+-rw-r--r--   0     1001      123       50 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/mod.rs
+-rw-r--r--   0     1001      123     3797 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/performance.rs
+-rw-r--r--   0     1001      123       59 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/export.rs
+-rw-r--r--   0     1001      123    20207 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/lib.rs
+-rw-r--r--   0     1001      123      387 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/prelude.rs
+-rw-r--r--   0     1001      123       44 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/src/sql.rs
+-rw-r--r--   0     1001      123     4272 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/date_like.rs
+-rw-r--r--   0     1001      123     2401 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/groupby.rs
+-rw-r--r--   0     1001      123    17826 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/joins.rs
+-rw-r--r--   0     1001      123      545 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/list.rs
+-rw-r--r--   0     1001      123      189 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/mod.rs
+-rw-r--r--   0     1001      123     6258 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/pivot.rs
+-rw-r--r--   0     1001      123     1102 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/random.rs
+-rw-r--r--   0     1001      123    10844 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/rolling_window.rs
+-rw-r--r--   0     1001      123     1093 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/series.rs
+-rw-r--r--   0     1001      123      370 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/utils.rs
+-rw-r--r--   0     1001      123    30013 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/csv.rs
+-rw-r--r--   0     1001      123     4490 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/ipc_stream.rs
+-rw-r--r--   0     1001      123     7044 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/json.rs
+-rw-r--r--   0     1001      123      378 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/mod.rs
+-rw-r--r--   0     1001      123      988 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/parquet.rs
+-rw-r--r--   0     1001      123     1530 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/joins.rs
+-rw-r--r--   0     1001      123     2452 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/aggregation.rs
+-rw-r--r--   0     1001      123      702 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/cse.rs
+-rw-r--r--   0     1001      123      500 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/explodes.rs
+-rw-r--r--   0     1001      123     2279 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/apply.rs
+-rw-r--r--   0     1001      123    10285 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/arity.rs
+-rw-r--r--   0     1001      123     1064 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/expand.rs
+-rw-r--r--   0     1001      123     1008 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/filter.rs
+-rw-r--r--   0     1001      123      428 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/is_in.rs
+-rw-r--r--   0     1001      123      121 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/mod.rs
+-rw-r--r--   0     1001      123      659 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/slice.rs
+-rw-r--r--   0     1001      123    10139 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/window.rs
+-rw-r--r--   0     1001      123      579 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/folds.rs
+-rw-r--r--   0     1001      123      557 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/functions.rs
+-rw-r--r--   0     1001      123     4482 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/groupby.rs
+-rw-r--r--   0     1001      123     1655 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs
+-rw-r--r--   0     1001      123      691 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/mod.rs
+-rw-r--r--   0     1001      123     5381 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/predicate_queries.rs
+-rw-r--r--   0     1001      123     4476 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/projection_queries.rs
+-rw-r--r--   0     1001      123     6444 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/queries.rs
+-rw-r--r--   0     1001      123      141 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/main.rs
+-rw-r--r--   0     1001      123    12591 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/schema.rs
+-rw-r--r--   0        0        0     1765 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/Cargo.toml
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/LICENSE
+-rw-r--r--   0     1001      123       98 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/mod.rs
+-rw-r--r--   0     1001      123     1219 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/filter.rs
+-rw-r--r--   0     1001      123     4103 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/function.rs
+-rw-r--r--   0     1001      123      229 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/mod.rs
+-rw-r--r--   0     1001      123      548 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs
+-rw-r--r--   0     1001      123     3247 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/projection.rs
+-rw-r--r--   0     1001      123     2324 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/reproject.rs
+-rw-r--r--   0     1001      123     6479 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs
+-rw-r--r--   0     1001      123    10473 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs
+-rw-r--r--   0     1001      123     1207 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs
+-rw-r--r--   0     1001      123     1888 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs
+-rw-r--r--   0     1001      123     4554 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs
+-rw-r--r--   0     1001      123     1746 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs
+-rw-r--r--   0     1001      123     5413 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs
+-rw-r--r--   0     1001      123     4951 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs
+-rw-r--r--   0     1001      123      211 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mod.rs
+-rw-r--r--   0     1001      123      856 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs
+-rw-r--r--   0     1001      123     4294 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs
+-rw-r--r--   0     1001      123     3030 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs
+-rw-r--r--   0     1001      123     6275 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs
+-rw-r--r--   0     1001      123    13665 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs
+-rw-r--r--   0     1001      123     2681 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs
+-rw-r--r--   0     1001      123     2534 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs
+-rw-r--r--   0     1001      123     5961 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs
+-rw-r--r--   0     1001      123    10673 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs
+-rw-r--r--   0     1001      123     2164 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs
+-rw-r--r--   0     1001      123     4666 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs
+-rw-r--r--   0     1001      123     3906 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs
+-rw-r--r--   0     1001      123    20859 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs
+-rw-r--r--   0     1001      123    23518 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs
+-rw-r--r--   0     1001      123     2457 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs
+-rw-r--r--   0     1001      123     8395 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/io.rs
+-rw-r--r--   0     1001      123     5485 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs
+-rw-r--r--   0     1001      123    14279 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs
+-rw-r--r--   0     1001      123    11824 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs
+-rw-r--r--   0     1001      123      178 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/mod.rs
+-rw-r--r--   0     1001      123     2002 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/memory.rs
+-rw-r--r--   0     1001      123      589 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/mod.rs
+-rw-r--r--   0     1001      123     1492 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs
+-rw-r--r--   0     1001      123     1824 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs
+-rw-r--r--   0     1001      123     3108 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/slice.rs
+-rw-r--r--   0     1001      123      130 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/mod.rs
+-rw-r--r--   0     1001      123     3808 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs
+-rw-r--r--   0     1001      123     6295 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs
+-rw-r--r--   0     1001      123     5953 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs
+-rw-r--r--   0     1001      123     3801 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs
+-rw-r--r--   0     1001      123      635 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/utils.rs
+-rw-r--r--   0     1001      123     5076 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/csv.rs
+-rw-r--r--   0     1001      123     1231 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/frame.rs
+-rw-r--r--   0     1001      123      987 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs
+-rw-r--r--   0     1001      123      366 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/mod.rs
+-rw-r--r--   0     1001      123     3387 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/parquet.rs
+-rw-r--r--   0     1001      123     1146 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/reproject.rs
+-rw-r--r--   0     1001      123     1022 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/union.rs
+-rw-r--r--   0     1001      123      448 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/expressions.rs
+-rw-r--r--   0     1001      123      272 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/lib.rs
+-rw-r--r--   0     1001      123      719 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/chunks.rs
+-rw-r--r--   0     1001      123      474 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/context.rs
+-rw-r--r--   0     1001      123      223 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/mod.rs
+-rw-r--r--   0     1001      123      430 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/operator.rs
+-rw-r--r--   0     1001      123      626 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/sink.rs
+-rw-r--r--   0     1001      123      241 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/source.rs
+-rw-r--r--   0     1001      123        1 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/config.rs
+-rw-r--r--   0     1001      123    20481 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/convert.rs
+-rw-r--r--   0     1001      123    13982 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs
+-rw-r--r--   0     1001      123     1237 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/mod.rs
+-rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/Cargo.toml
+-rw-r--r--   0     1001      123       76 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/.gitignore
+-rw-r--r--   0     1001      123     1055 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/LICENSE
+-rw-r--r--   0     1001      123     2414 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/Makefile
+-rw-r--r--   0     1001      123    12625 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/README.md
+-rw-r--r--   0     1001      123      651 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/build.rs
+-rw-r--r--   0     1001      123       32 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/.gitignore
+-rw-r--r--   0     1001      123      679 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/Makefile
+-rw-r--r--   0     1001      123      318 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/api_redirect.html
+-rw-r--r--   0     1001      123      151 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/autosummary/accessor.rst
+-rw-r--r--   0     1001      123      160 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/autosummary/accessor_attribute.rst
+-rw-r--r--   0     1001      123      168 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/autosummary/accessor_callable.rst
+-rw-r--r--   0     1001      123      157 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/autosummary/accessor_method.rst
+-rw-r--r--   0     1001      123      836 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/autosummary/class.rst
+-rw-r--r--   0     1001      123       94 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/autosummary/class_without_autosummary.rst
+-rw-r--r--   0     1001      123      406 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/_templates/sidebar-nav-bs.html
+-rw-r--r--   0     1001      123      450 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/requirements-docs.txt
+-rw-r--r--   0     1001      123     1567 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/_static/css/custom.css
+-rw-r--r--   0     1001      123     7302 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/conf.py
+-rw-r--r--   0     1001      123       51 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/index.rst
+-rw-r--r--   0     1001      123     6767 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/api.rst
+-rw-r--r--   0     1001      123     1694 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/config.rst
+-rw-r--r--   0     1001      123      274 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/aggregation.rst
+-rw-r--r--   0     1001      123      221 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/attributes.rst
+-rw-r--r--   0     1001      123      142 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/computation.rst
+-rw-r--r--   0     1001      123      319 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/descriptive.rst
+-rw-r--r--   0     1001      123      319 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/export.rst
+-rw-r--r--   0     1001      123      464 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/groupby.rst
+-rw-r--r--   0     1001      123      379 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/index.rst
+-rw-r--r--   0     1001      123      189 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/miscellaneous.rst
+-rw-r--r--   0     1001      123     1513 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/dataframe/modify_select.rst
+-rw-r--r--   0     1001      123      663 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/datatypes.rst
+-rw-r--r--   0     1001      123      421 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/exceptions.rst
+-rw-r--r--   0     1001      123      391 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/aggregation.rst
+-rw-r--r--   0     1001      123      309 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/binary.rst
+-rw-r--r--   0     1001      123      338 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/boolean.rst
+-rw-r--r--   0     1001      123      237 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/categories.rst
+-rw-r--r--   0     1001      123      221 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/columns.rst
+-rw-r--r--   0     1001      123     1061 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/computation.rst
+-rw-r--r--   0     1001      123     1114 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/functions.rst
+-rw-r--r--   0     1001      123      461 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/index.rst
+-rw-r--r--   0     1001      123      695 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/list.rst
+-rw-r--r--   0     1001      123      374 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/meta.rst
+-rw-r--r--   0     1001      123      125 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/miscellaneous.rst
+-rw-r--r--   0     1001      123      977 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/modify_select.rst
+-rw-r--r--   0     1001      123      639 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/operators.rst
+-rw-r--r--   0     1001      123      860 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/string.rst
+-rw-r--r--   0     1001      123      254 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/struct.rst
+-rw-r--r--   0     1001      123      968 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/temporal.rst
+-rw-r--r--   0     1001      123       98 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/expressions/window.rst
+-rw-r--r--   0     1001      123      692 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/functions.rst
+-rw-r--r--   0     1001      123      392 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/index.rst
+-rw-r--r--   0     1001      123     1269 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/io.rst
+-rw-r--r--   0     1001      123      252 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/aggregation.rst
+-rw-r--r--   0     1001      123      179 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/attributes.rst
+-rw-r--r--   0     1001      123      146 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/descriptive.rst
+-rw-r--r--   0     1001      123      497 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/groupby.rst
+-rw-r--r--   0     1001      123      354 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/index.rst
+-rw-r--r--   0     1001      123      455 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/miscellaneous.rst
+-rw-r--r--   0     1001      123      988 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/modify_select.rst
+-rw-r--r--   0     1001      123      358 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/aggregation.rst
+-rw-r--r--   0     1001      123      256 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/attributes.rst
+-rw-r--r--   0     1001      123      321 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/binary.rst
+-rw-r--r--   0     1001      123      117 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/boolean.rst
+-rw-r--r--   0     1001      123      241 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/categories.rst
+-rw-r--r--   0     1001      123     1103 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/computation.rst
+-rw-r--r--   0     1001      123      744 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/descriptive.rst
+-rw-r--r--   0     1001      123      240 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/export.rst
+-rw-r--r--   0     1001      123      428 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/index.rst
+-rw-r--r--   0     1001      123      749 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/list.rst
+-rw-r--r--   0     1001      123      236 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/miscellaneous.rst
+-rw-r--r--   0     1001      123     1077 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/modify_select.rst
+-rw-r--r--   0     1001      123      922 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/string.rst
+-rw-r--r--   0     1001      123      396 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/struct.rst
+-rw-r--r--   0     1001      123     1118 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/series/temporal.rst
+-rw-r--r--   0     1001      123      302 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/sql.rst
+-rw-r--r--   0     1001      123      647 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/testing.rst
+-rw-r--r--   0     1001      123      168 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/docs/source/reference/utils.rst
+-rw-r--r--   0     1001      123     6283 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/__init__.py
+-rw-r--r--   0     1001      123    13396 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/api.py
+-rw-r--r--   0     1001      123    25956 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/config.py
+-rw-r--r--   0     1001      123    25409 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/convert.py
+-rw-r--r--   0     1001      123       77 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/dataframe/__init__.py
+-rw-r--r--   0     1001      123     5057 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/dataframe/_html.py
+-rw-r--r--   0     1001      123   304087 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/dataframe/frame.py
+-rw-r--r--   0     1001      123    33240 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/dataframe/groupby.py
+-rw-r--r--   0     1001      123     2628 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/datatypes/__init__.py
+-rw-r--r--   0     1001      123    11480 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/datatypes/classes.py
+-rw-r--r--   0     1001      123     1577 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/datatypes/constants.py
+-rw-r--r--   0     1001      123     4430 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/datatypes/constructor.py
+-rw-r--r--   0     1001      123    14921 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/datatypes/convert.py
+-rw-r--r--   0     1001      123     7338 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/dependencies.py
+-rw-r--r--   0     1001      123     2954 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/exceptions.py
+-rw-r--r--   0     1001      123       61 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/__init__.py
+-rw-r--r--   0     1001      123     2730 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/binary.py
+-rw-r--r--   0     1001      123     1708 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/categorical.py
+-rw-r--r--   0     1001      123    69359 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/datetime.py
+-rw-r--r--   0     1001      123   250779 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/expr.py
+-rw-r--r--   0     1001      123    22899 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/list.py
+-rw-r--r--   0     1001      123     2059 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/meta.py
+-rw-r--r--   0     1001      123    44664 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/string.py
+-rw-r--r--   0     1001      123     5436 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/expr/struct.py
+-rw-r--r--   0     1001      123     1981 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/functions/__init__.py
+-rw-r--r--   0     1001      123    29688 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/functions/eager.py
+-rw-r--r--   0     1001      123    90827 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/functions/lazy.py
+-rw-r--r--   0     1001      123     6293 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/functions/whenthen.py
+-rw-r--r--   0     1001      123      280 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/internals.py
+-rw-r--r--   0     1001      123      978 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/__init__.py
+-rw-r--r--   0     1001      123     6264 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/_utils.py
+-rw-r--r--   0     1001      123      878 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/avro.py
+-rw-r--r--   0     1001      123      144 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/csv/__init__.py
+-rw-r--r--   0     1001      123     1082 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/csv/_utils.py
+-rw-r--r--   0     1001      123     4691 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/csv/batched_reader.py
+-rw-r--r--   0     1001      123    35533 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/csv/functions.py
+-rw-r--r--   0     1001      123     8655 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/database.py
+-rw-r--r--   0     1001      123    10988 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/delta.py
+-rw-r--r--   0     1001      123       75 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/excel/__init__.py
+-rw-r--r--   0     1001      123    18459 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/excel/_write_utils.py
+-rw-r--r--   0     1001      123     6476 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/excel/functions.py
+-rw-r--r--   0     1001      123      142 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/ipc/__init__.py
+-rw-r--r--   0     1001      123     1271 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/ipc/anonymous_scan.py
+-rw-r--r--   0     1001      123     5840 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/ipc/functions.py
+-rw-r--r--   0     1001      123      519 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/json.py
+-rw-r--r--   0     1001      123     2257 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/ndjson.py
+-rw-r--r--   0     1001      123      170 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/parquet/__init__.py
+-rw-r--r--   0     1001      123     1299 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/parquet/anonymous_scan.py
+-rw-r--r--   0     1001      123     7212 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/parquet/functions.py
+-rw-r--r--   0     1001      123      136 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/pyarrow_dataset/__init__.py
+-rw-r--r--   0     1001      123     2331 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/pyarrow_dataset/anonymous_scan.py
+-rw-r--r--   0     1001      123     3611 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/io/pyarrow_dataset/functions.py
+-rw-r--r--   0     1001      123       77 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/lazyframe/__init__.py
+-rw-r--r--   0     1001      123   166798 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/lazyframe/frame.py
+-rw-r--r--   0     1001      123    24178 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/lazyframe/groupby.py
+-rw-r--r--   0     1001      123        0 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/py.typed
+-rw-r--r--   0     1001      123       69 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/__init__.py
+-rw-r--r--   0     1001      123     1579 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/_numpy.py
+-rw-r--r--   0     1001      123     1920 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/binary.py
+-rw-r--r--   0     1001      123     1699 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/categorical.py
+-rw-r--r--   0     1001      123    47287 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/datetime.py
+-rw-r--r--   0     1001      123    12385 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/list.py
+-rw-r--r--   0     1001      123   163748 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/series.py
+-rw-r--r--   0     1001      123    27401 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/string.py
+-rw-r--r--   0     1001      123     2287 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/struct.py
+-rw-r--r--   0     1001      123     5375 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/series/utils.py
+-rw-r--r--   0     1001      123     7638 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/slice.py
+-rw-r--r--   0     1001      123       75 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/sql/__init__.py
+-rw-r--r--   0     1001      123     1351 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/sql/context.py
+-rw-r--r--   0     1001      123     4764 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/string_cache.py
+-rw-r--r--   0     1001      123      362 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/__init__.py
+-rw-r--r--   0     1001      123      929 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/_private.py
+-rw-r--r--   0     1001      123     3689 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/_tempdir.py
+-rw-r--r--   0     1001      123    13597 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/asserts.py
+-rw-r--r--   0     1001      123      684 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/parametric/__init__.py
+-rw-r--r--   0     1001      123    24543 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/parametric/primitives.py
+-rw-r--r--   0     1001      123     6907 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/testing/parametric/strategies.py
+-rw-r--r--   0     1001      123     5681 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/type_aliases.py
+-rw-r--r--   0     1001      123     1167 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/__init__.py
+-rw-r--r--   0     1001      123    50687 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/_construction.py
+-rw-r--r--   0     1001      123     2782 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/_parse_expr_input.py
+-rw-r--r--   0     1001      123      721 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/_scan.py
+-rw-r--r--   0     1001      123      687 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/_wrap.py
+-rw-r--r--   0     1001      123      683 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/build_info.py
+-rw-r--r--   0     1001      123     9184 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/convert.py
+-rw-r--r--   0     1001      123     5789 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/decorators.py
+-rw-r--r--   0     1001      123     1660 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/meta.py
+-rw-r--r--   0     1001      123      514 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/polars_version.py
+-rw-r--r--   0     1001      123     2339 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/show_versions.py
+-rw-r--r--   0     1001      123    11592 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/polars/utils/various.py
+-rw-r--r--   0     1001      123     5378 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/pyproject.toml
+-rw-r--r--   0     1001      123      699 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/requirements-dev.txt
+-rw-r--r--   0     1001      123       70 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/requirements-lint.txt
+-rw-r--r--   0     1001      123     1640 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/scripts/check_stacklevels.py
+-rw-r--r--   0     1001      123    11023 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/apply/dataframe.rs
+-rw-r--r--   0     1001      123     8388 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/apply/mod.rs
+-rw-r--r--   0     1001      123    71480 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/apply/series.rs
+-rw-r--r--   0     1001      123       32 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/arrow_interop/mod.rs
+-rw-r--r--   0     1001      123     1306 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/arrow_interop/to_py.rs
+-rw-r--r--   0     1001      123     3902 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/arrow_interop/to_rust.rs
+-rw-r--r--   0     1001      123     5250 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/batched_csv.rs
+-rw-r--r--   0     1001      123    47200 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/conversion.rs
+-rw-r--r--   0     1001      123    45472 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/dataframe.rs
+-rw-r--r--   0     1001      123     3799 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/datatypes.rs
+-rw-r--r--   0     1001      123     3288 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/error.rs
+-rw-r--r--   0     1001      123     9482 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/file.rs
+-rw-r--r--   0     1001      123     7468 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lazy/apply.rs
+-rw-r--r--   0     1001      123    33439 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lazy/dataframe.rs
+-rw-r--r--   0     1001      123    62664 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lazy/dsl.rs
+-rw-r--r--   0     1001      123     1082 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lazy/meta.rs
+-rw-r--r--   0     1001      123      727 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lazy/mod.rs
+-rw-r--r--   0     1001      123      212 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lazy/utils.rs
+-rw-r--r--   0     1001      123    20992 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/lib.rs
+-rw-r--r--   0     1001      123     8642 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/npy.rs
+-rw-r--r--   0     1001      123     1029 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/object.rs
+-rw-r--r--   0     1001      123      122 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/prelude.rs
+-rw-r--r--   0     1001      123      435 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/py_modules.rs
+-rw-r--r--   0     1001      123    54535 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/series.rs
+-rw-r--r--   0     1001      123     3478 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/set.rs
+-rw-r--r--   0     1001      123      843 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/sql.rs
+-rw-r--r--   0     1001      123     2335 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/src/utils.rs
+-rw-r--r--   0     1001      123     6165 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/README.md
+-rw-r--r--   0     1001      123     2189 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/benchmark/groupby-datagen.R
+-rw-r--r--   0     1001      123     7945 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/benchmark/run_h2oai_benchmark.py
+-rw-r--r--   0     1001      123     5721 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/benchmark/test_release.py
+-rw-r--r--   0     1001      123     4589 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/docs/run_doctest.py
+-rw-r--r--   0     1001      123     1633 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/parametric/conftest.py
+-rw-r--r--   0     1001      123     3823 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/parametric/test_dataframe.py
+-rw-r--r--   0     1001      123     1692 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/parametric/test_lazyframe.py
+-rw-r--r--   0     1001      123     6355 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/parametric/test_series.py
+-rw-r--r--   0     1001      123     8299 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/parametric/test_testing.py
+-rw-r--r--   0     1001      123        0 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/__init__.py
+-rw-r--r--   0     1001      123     3382 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/conftest.py
+-rw-r--r--   0     1001      123       86 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/__init__.py
+-rw-r--r--   0     1001      123      351 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_binary.py
+-rw-r--r--   0     1001      123     1420 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_bool.py
+-rw-r--r--   0     1001      123    12662 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_categorical.py
+-rw-r--r--   0     1001      123     2766 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_decimal.py
+-rw-r--r--   0     1001      123      280 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_duration.py
+-rw-r--r--   0     1001      123    15805 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_list.py
+-rw-r--r--   0     1001      123      284 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_null.py
+-rw-r--r--   0     1001      123     2801 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_object.py
+-rw-r--r--   0     1001      123    29644 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_struct.py
+-rw-r--r--   0     1001      123    92406 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_temporal.py
+-rw-r--r--   0     1001      123      418 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/datatypes/test_time.py
+-rw-r--r--   0     1001      123      218 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/conftest.py
+-rw-r--r--   0     1001      123       16 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/.part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/.part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet.crc
+-rw-r--r--   0     1001      123       16 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/_delta_log/.00000000000000000000.json.crc
+-rw-r--r--   0     1001      123       16 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/_delta_log/.00000000000000000001.json.crc
+-rw-r--r--   0     1001      123      905 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json
+-rw-r--r--   0     1001      123      936 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json
+-rw-r--r--   0     1001      123      972 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet
+-rw-r--r--   0     1001      123      690 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet
+-rw-r--r--   0     1001      123        0 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/empty.csv
+-rw-r--r--   0     1001      123     5959 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/example.xlsx
+-rw-r--r--   0     1001      123      457 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.csv
+-rw-r--r--   0     1001      123     2351 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.ipc
+-rw-r--r--   0     1001      123     1713 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.ndjson
+-rw-r--r--   0     1001      123     1427 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.parquet
+-rw-r--r--   0     1001      123      455 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.csv
+-rw-r--r--   0     1001      123     2351 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.ipc
+-rw-r--r--   0     1001      123     1711 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.ndjson
+-rw-r--r--   0     1001      123     1916 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.parquet
+-rw-r--r--   0     1001      123      455 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods3.csv
+-rw-r--r--   0     1001      123      457 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods4.csv
+-rw-r--r--   0     1001      123      452 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/foods5.csv
+-rw-r--r--   0     1001      123       49 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/gzipped.csv
+-rw-r--r--   0     1001      123       57 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/small.csv
+-rw-r--r--   0     1001      123      756 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/files/small.parquet
+-rw-r--r--   0     1001      123     1937 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_avro.py
+-rw-r--r--   0     1001      123    39498 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_csv.py
+-rw-r--r--   0     1001      123     6360 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_database.py
+-rw-r--r--   0     1001      123     3456 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_delta.py
+-rw-r--r--   0     1001      123    11169 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_excel.py
+-rw-r--r--   0     1001      123     5919 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_ipc.py
+-rw-r--r--   0     1001      123     3720 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_json.py
+-rw-r--r--   0     1001      123     6849 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_csv.py
+-rw-r--r--   0     1001      123     2060 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_ipc.py
+-rw-r--r--   0     1001      123     2881 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_json.py
+-rw-r--r--   0     1001      123    11849 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_parquet.py
+-rw-r--r--   0     1001      123     2012 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_other.py
+-rw-r--r--   0     1001      123    13735 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_parquet.py
+-rw-r--r--   0     1001      123      612 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_pickle.py
+-rw-r--r--   0     1001      123     3259 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/io/test_pyarrow_dataset.py
+-rw-r--r--   0     1001      123      509 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/__init__.py
+-rw-r--r--   0     1001      123     3218 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_binary.py
+-rw-r--r--   0     1001      123     2489 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_categorical.py
+-rw-r--r--   0     1001      123    15436 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_datetime.py
+-rw-r--r--   0     1001      123    12750 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_list.py
+-rw-r--r--   0     1001      123     1748 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_meta.py
+-rw-r--r--   0     1001      123    23698 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_string.py
+-rw-r--r--   0     1001      123    15776 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_strptime.py
+-rw-r--r--   0     1001      123      982 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/namespaces/test_struct.py
+-rw-r--r--   0     1001      123       85 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/__init__.py
+-rw-r--r--   0     1001      123     6238 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_aggregations.py
+-rw-r--r--   0     1001      123     9412 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_apply.py
+-rw-r--r--   0     1001      123     4390 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_arithmetic.py
+-rw-r--r--   0     1001      123      956 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_comparison.py
+-rw-r--r--   0     1001      123     2906 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_drop.py
+-rw-r--r--   0     1001      123     8252 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_explode.py
+-rw-r--r--   0     1001      123     3664 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_filter.py
+-rw-r--r--   0     1001      123     1801 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_folds.py
+-rw-r--r--   0     1001      123    22696 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_groupby.py
+-rw-r--r--   0     1001      123     2959 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_is_in.py
+-rw-r--r--   0     1001      123    16937 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_join.py
+-rw-r--r--   0     1001      123    10467 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_join_asof.py
+-rw-r--r--   0     1001      123      643 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_melt.py
+-rw-r--r--   0     1001      123    10253 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_pivot.py
+-rw-r--r--   0     1001      123    18639 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_rolling.py
+-rw-r--r--   0     1001      123    19550 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_sort.py
+-rw-r--r--   0     1001      123     3643 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_statistics.py
+-rw-r--r--   0     1001      123     3631 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_transpose.py
+-rw-r--r--   0     1001      123      771 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_unique.py
+-rw-r--r--   0     1001      123     9814 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/operations/test_window.py
+-rw-r--r--   0     1001      123     4775 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_api.py
+-rw-r--r--   0     1001      123     1077 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_arity.py
+-rw-r--r--   0     1001      123    19856 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_cfg.py
+-rw-r--r--   0     1001      123    39286 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_constructors.py
+-rw-r--r--   0     1001      123      454 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_context.py
+-rw-r--r--   0     1001      123     1628 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_cse.py
+-rw-r--r--   0     1001      123     3497 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_datatypes.py
+-rw-r--r--   0     1001      123   120890 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_df.py
+-rw-r--r--   0     1001      123     1196 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_empty.py
+-rw-r--r--   0     1001      123    16867 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_errors.py
+-rw-r--r--   0     1001      123     2387 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_expr_multi_cols.py
+-rw-r--r--   0     1001      123    32643 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_exprs.py
+-rw-r--r--   0     1001      123     3305 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_fmt.py
+-rw-r--r--   0     1001      123    11420 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_functions.py
+-rw-r--r--   0     1001      123     3763 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_interchange.py
+-rw-r--r--   0     1001      123    31618 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_interop.py
+-rw-r--r--   0     1001      123    49534 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_lazy.py
+-rw-r--r--   0     1001      123     2369 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_polars_import.py
+-rw-r--r--   0     1001      123     4014 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_predicates.py
+-rw-r--r--   0     1001      123     6995 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_projections.py
+-rw-r--r--   0     1001      123    11550 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_queries.py
+-rw-r--r--   0     1001      123     4743 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_rows.py
+-rw-r--r--   0     1001      123    13181 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_schema.py
+-rw-r--r--   0     1001      123     2634 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_serde.py
+-rw-r--r--   0     1001      123    83663 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_series.py
+-rw-r--r--   0     1001      123     2561 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_sql.py
+-rw-r--r--   0     1001      123    13877 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_streaming.py
+-rw-r--r--   0     1001      123    10700 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/test_testing.py
+-rw-r--r--   0     1001      123       41 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/utils/__init__.py
+-rw-r--r--   0     1001      123      306 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/utils/test_build_info.py
+-rw-r--r--   0     1001      123      247 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/utils/test_show_versions.py
+-rw-r--r--   0     1001      123     4307 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/tests/unit/utils/test_utils.py
+-rw-r--r--   0     1001      123    66145 2023-04-21 14:00:18.000000 polars_lts_cpu-0.17.6/Cargo.lock
+-rw-r--r--   0        0        0    15163 1970-01-01 00:00:00.000000 polars_lts_cpu-0.17.6/PKG-INFO
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 
 test = ["dtype-date", "dtype-datetime", "polars-core/fmt"]
 
 default = ["private"]
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/date.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/datetime.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/duration.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/kernels.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/kernels.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/ints.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/rolling_window/rolling_kernels/no_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/infer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/patterns.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/chunkedarray/utf8/strptime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/date_range.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/date_range.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/groupby/dynamic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/groupby/dynamic.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 use chrono_tz::Tz;
 use polars_arrow::time_zone::PolarsTimeZone;
 use polars_arrow::utils::CustomIterTools;
 use polars_core::export::rayon::prelude::*;
 use polars_core::frame::groupby::GroupsProxy;
 use polars_core::prelude::*;
 use polars_core::series::IsSorted;
+use polars_core::utils::ensure_sorted_arg;
 use polars_core::POOL;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 use smartstring::alias::String as SmartString;
 
 use crate::prelude::*;
 
@@ -234,14 +235,15 @@
         tu: TimeUnit,
         time_type: &DataType,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
         polars_ensure!(!options.every.negative, ComputeError: "'every' argument must be positive");
         if dt.is_empty() {
             return dt.cast(time_type).map(|s| (s, by, GroupsProxy::default()));
         }
+        ensure_sorted_arg(&dt);
 
         let sorted_set = matches!(dt.is_sorted_flag(), IsSorted::Ascending);
         // a requirement for the index
         // so we can set this such that downstream code has this info
         dt.set_sorted_flag(IsSorted::Ascending);
 
         let w = Window::new(options.every, options.period, options.offset);
@@ -457,14 +459,15 @@
         dt: Series,
         by: Vec<Series>,
         options: &RollingGroupOptions,
         tu: TimeUnit,
         tz: Option<impl PolarsTimeZone>,
         time_type: &DataType,
     ) -> PolarsResult<(Series, Vec<Series>, GroupsProxy)> {
+        ensure_sorted_arg(&dt);
         let mut dt = dt.rechunk();
         // a requirement for the index
         // so we can set this such that downstream code has this info
         dt.set_sorted_flag(IsSorted::Ascending);
 
         let groups = if by.is_empty() {
             let dt = dt.datetime().unwrap();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/round.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/_trait.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/_trait.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/implementations/integers.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/implementations/integers.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/series/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/series/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/truncate.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/truncate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/upsample.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/upsample.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/bounds.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/calendar.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/calendar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/duration.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/groupby.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/test.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/test.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-time/src/windows/window.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/src/windows/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-algo/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-algo/Cargo.toml`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-algo/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-algo/src/algo.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-algo/src/algo.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/arena.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/arena.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/atomic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/atomic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/cell.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/cell.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/contention_pool.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/contention_pool.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/hash.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/iter/enumerate_idx.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/iter/enumerate_idx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/macros.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/macros.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/sort.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/sync.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/sync.rs`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     }
 
     pub fn new_null() -> Self {
         Self(std::ptr::null_mut())
     }
 
     #[inline(always)]
-    pub fn get(self) -> *mut T {
+    pub fn get(&self) -> *mut T {
         self.0
     }
 
     pub fn is_null(&self) -> bool {
         self.0.is_null()
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/unwrap.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/unwrap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-utils/src/wasm.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-utils/src/wasm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -72,19 +72,19 @@
 chunked_ids = ["polars-core/chunked_ids"]
 asof_join = ["polars-core/asof_join"]
 semi_anti_join = ["polars-core/semi_anti_join"]
 list_take = []
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-algo/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/binary/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/interpolate.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/interpolate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/count.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/hash.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/hash.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/sum_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/list/to_struct.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/nan_propagating_aggregate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/set.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/case.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/case.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/json_path.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/justify.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/namespace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/strings/replace.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/chunked_array/top_k.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/chunked_array/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/join/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/join/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/pivot/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/pivot/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/frame/pivot/positioning.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/frame/pivot/positioning.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_algo/hyperloglogplus.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/approx_unique.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/approx_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/arg_min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/floor_divide.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/floor_divide.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/is_first.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/is_first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/is_unique.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/is_unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/log.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/rolling.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/search_sorted.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/search_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/to_dummies.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/to_dummies.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-ops/src/series/ops/various.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/src/series/ops/various.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -175,19 +175,19 @@
 smartstring= { version = "1" }
 thiserror= "^1"
 url = { version = "2.3.1", optional = true }
 xxhash-rust= { version = "0.8.6", features = ["xxh3"] }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-error/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/arithmetic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/bitwise.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/bitwise.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/binary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/list.rs`

 * *Files 6% similar despite different names*

```diff
@@ -441,44 +441,44 @@
                 DataType::List(Box::new(DataType::Null)),
             )
         }
     }
 }
 
 pub fn get_list_builder(
-    dt: &DataType,
+    inner_type_logical: &DataType,
     value_capacity: usize,
     list_capacity: usize,
     name: &str,
 ) -> PolarsResult<Box<dyn ListBuilderTrait>> {
-    let physical_type = dt.to_physical();
+    let physical_type = inner_type_logical.to_physical();
 
     match &physical_type {
         #[cfg(feature = "object")]
         DataType::Object(_) => polars_bail!(opq = list_builder, &physical_type),
         #[cfg(feature = "dtype-struct")]
         DataType::Struct(_) => Ok(Box::new(AnonymousOwnedListBuilder::new(
             name,
             list_capacity,
-            Some(physical_type),
+            Some(inner_type_logical.clone()),
         ))),
         DataType::Null => Ok(Box::new(LargeListNullBuilder::with_capacity(list_capacity))),
         DataType::List(_) => Ok(Box::new(AnonymousOwnedListBuilder::new(
             name,
             list_capacity,
-            Some(physical_type),
+            Some(inner_type_logical.clone()),
         ))),
         _ => {
             macro_rules! get_primitive_builder {
                 ($type:ty) => {{
                     let builder = ListPrimitiveChunkedBuilder::<$type>::new(
                         name,
                         list_capacity,
                         value_capacity,
-                        dt.clone(),
+                        inner_type_logical.clone(),
                     );
                     Box::new(builder)
                 }};
             }
             macro_rules! get_bool_builder {
                 () => {{
                     let builder =
@@ -511,30 +511,30 @@
     }
 }
 
 pub struct AnonymousListBuilder<'a> {
     name: String,
     builder: AnonymousBuilder<'a>,
     fast_explode: bool,
-    pub dtype: Option<DataType>,
+    inner_dtype: Option<DataType>,
 }
 
 impl Default for AnonymousListBuilder<'_> {
     fn default() -> Self {
         Self::new("", 0, None)
     }
 }
 
 impl<'a> AnonymousListBuilder<'a> {
     pub fn new(name: &str, capacity: usize, inner_dtype: Option<DataType>) -> Self {
         Self {
             name: name.into(),
             builder: AnonymousBuilder::new(capacity),
             fast_explode: true,
-            dtype: inner_dtype,
+            inner_dtype,
         }
     }
 
     pub fn append_opt_series(&mut self, opt_s: Option<&'a Series>) {
         match opt_s {
             Some(s) => self.append_series(s),
             None => {
@@ -587,26 +587,37 @@
         }
     }
 
     pub fn finish(&mut self) -> ListChunked {
         // don't use self from here on one
         let slf = std::mem::take(self);
         if slf.builder.is_empty() {
-            ListChunked::full_null_with_dtype(&slf.name, 0, &slf.dtype.unwrap_or(DataType::Null))
+            ListChunked::full_null_with_dtype(
+                &slf.name,
+                0,
+                &slf.inner_dtype.unwrap_or(DataType::Null),
+            )
         } else {
-            let dtype = slf.dtype.map(|dt| dt.to_physical().to_arrow());
-            let arr = slf.builder.finish(dtype.as_ref()).unwrap();
-            let dtype = DataType::from(arr.data_type());
+            let inner_dtype_physical = slf
+                .inner_dtype
+                .as_ref()
+                .map(|dt| dt.to_physical().to_arrow());
+            let arr = slf.builder.finish(inner_dtype_physical.as_ref()).unwrap();
+
+            let list_dtype_logical = match slf.inner_dtype {
+                None => DataType::from(arr.data_type()),
+                Some(dt) => DataType::List(Box::new(dt)),
+            };
             let mut ca = unsafe { ListChunked::from_chunks("", vec![Box::new(arr)]) };
 
             if slf.fast_explode {
                 ca.set_fast_explode();
             }
 
-            ca.field = Arc::new(Field::new(&slf.name, dtype));
+            ca.field = Arc::new(Field::new(&slf.name, list_dtype_logical));
             ca
         }
     }
 }
 
 pub struct AnonymousOwnedListBuilder {
     name: String,
@@ -653,25 +664,32 @@
         self.fast_explode = false;
         self.builder.push_null()
     }
 
     fn finish(&mut self) -> ListChunked {
         // don't use self from here on one
         let slf = std::mem::take(self);
-        let inner_dtype = slf.inner_dtype.map(|dt| dt.to_physical().to_arrow());
-        let arr = slf.builder.finish(inner_dtype.as_ref()).unwrap();
-        let dtype = DataType::from(arr.data_type());
+        let inner_dtype_physical = slf
+            .inner_dtype
+            .as_ref()
+            .map(|dt| dt.to_physical().to_arrow());
+        let arr = slf.builder.finish(inner_dtype_physical.as_ref()).unwrap();
+
+        let list_dtype_logical = match slf.inner_dtype {
+            None => DataType::from(arr.data_type()),
+            Some(dt) => DataType::List(Box::new(dt)),
+        };
         // safety: same type
         let mut ca = unsafe { ListChunked::from_chunks("", vec![Box::new(arr)]) };
 
         if slf.fast_explode {
             ca.set_fast_explode();
         }
 
-        ca.field = Arc::new(Field::new(&slf.name, dtype));
+        ca.field = Arc::new(Field::new(&slf.name, list_dtype_logical));
         ca
     }
 }
 
 impl AnonymousOwnedListBuilder {
     pub fn new(name: &str, capacity: usize, inner_dtype: Option<DataType>) -> Self {
         Self {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/primitive.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/builder/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/cast.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/cast.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 //! Implementations of the ChunkCast Trait.
 use std::convert::TryFrom;
 
 use arrow::compute::cast::CastOptions;
-use polars_arrow::compute::cast;
 
 #[cfg(feature = "dtype-categorical")]
 use crate::chunked_array::categorical::CategoricalChunkedBuilder;
 use crate::prelude::*;
 
 pub(crate) fn cast_chunks(
     chunks: &[ArrayRef],
@@ -246,72 +245,36 @@
     }
 
     unsafe fn cast_unchecked(&self, data_type: &DataType) -> PolarsResult<Series> {
         self.cast(data_type)
     }
 }
 
-fn cast_inner_list_type(list: &ListArray<i64>, child_type: &DataType) -> PolarsResult<ArrayRef> {
-    let child = list.values();
-    let offsets = list.offsets();
-    let child = cast::cast(child.as_ref(), &child_type.to_arrow())?;
-
-    let data_type = ListArray::<i64>::default_datatype(child_type.to_arrow());
-    let list = ListArray::new(data_type, offsets.clone(), child, list.validity().cloned());
-    Ok(Box::new(list) as ArrayRef)
-}
-
 /// We cannot cast anything to or from List/LargeList
 /// So this implementation casts the inner type
 impl ChunkCast for ListChunked {
     fn cast(&self, data_type: &DataType) -> PolarsResult<Series> {
         use DataType::*;
         match data_type {
             List(child_type) => {
-                let phys_child = child_type.to_physical();
-
                 match (self.inner_dtype(), &**child_type) {
                     #[cfg(feature = "dtype-categorical")]
-                    (Utf8, Categorical(_)) => {
-                        let (arr, child_type) = cast_list(self, child_type)?;
-                        Ok(unsafe {
-                            Series::from_chunks_and_dtype_unchecked(
-                                self.name(),
-                                vec![arr],
-                                &List(Box::new(child_type)),
-                            )
-                        })
-                    }
-                    #[cfg(feature = "dtype-categorical")]
-                    (dt, Categorical(None)) => {
+                    (dt, Categorical(None)) if !matches!(dt, Utf8) => {
                         polars_bail!(ComputeError: "cannot cast list inner type: '{:?}' to Categorical", dt)
                     }
-                    _ if phys_child.is_primitive() => {
-                        let mut ca = if child_type.to_physical() != self.inner_dtype().to_physical()
-                        {
-                            let chunks = self
-                                .downcast_iter()
-                                .map(|list| cast_inner_list_type(list, &phys_child))
-                                .collect::<PolarsResult<_>>()?;
-                            unsafe { ListChunked::from_chunks(self.name(), chunks) }
-                        } else {
-                            self.clone()
-                        };
-                        ca.set_inner_dtype(*child_type.clone());
-                        Ok(ca.into_series())
-                    }
                     _ => {
-                        let arr = cast_list(self, child_type)?.0;
+                        // ensure the inner logical type bubbles up
+                        let (arr, child_type) = cast_list(self, child_type)?;
                         // Safety: we just casted so the dtype matches.
                         // we must take this path to correct for physical types.
                         unsafe {
                             Ok(Series::from_chunks_and_dtype_unchecked(
                                 self.name(),
                                 vec![arr],
-                                data_type,
+                                &List(Box::new(child_type)),
                             ))
                         }
                     }
                 }
             }
             _ => polars_bail!(ComputeError: "cannot cast list type"),
         }
@@ -323,15 +286,18 @@
 }
 
 // Returns inner data type. This is needed because a cast can instantiate the dtype inner
 // values for instance with categoricals
 fn cast_list(ca: &ListChunked, child_type: &DataType) -> PolarsResult<(ArrayRef, DataType)> {
     let ca = ca.rechunk();
     let arr = ca.downcast_iter().next().unwrap();
-    let s = Series::try_from(("", arr.values().clone())).unwrap();
+    // safety: inner dtype is passed correctly
+    let s = unsafe {
+        Series::from_chunks_and_dtype_unchecked("", vec![arr.values().clone()], &ca.inner_dtype())
+    };
     let new_inner = s.cast(child_type)?;
 
     let inner_dtype = new_inner.dtype().clone();
     debug_assert_eq!(&inner_dtype, child_type);
 
     let new_values = new_inner.array_ref(0).clone();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/comparison/scalar.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/drop.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/float.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/iterator/par/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/kernels/take.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/kernels/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/list/iterator.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/list/iterator.rs`

 * *Files 16% similar despite different names*

```diff
@@ -29,16 +29,18 @@
                 if matches!(self.inner_dtype, DataType::Struct(_)) {
                     // Safety
                     // dtype is known
                     unsafe {
                         let mut s = Series::from_chunks_and_dtype_unchecked(
                             "",
                             vec![array_ref],
-                            &self.inner_dtype,
-                        );
+                            &self.inner_dtype.to_physical(),
+                        )
+                        .cast_unchecked(&self.inner_dtype)
+                        .unwrap();
                         // swap the new series with the container
                         std::mem::swap(&mut *self.series_container, &mut s);
                         // return a reference to the container
                         // this lifetime is now bound to 'a
                         return UnstableSeries::new(
                             &mut *(&mut *self.series_container as *mut Series),
                         );
@@ -101,33 +103,43 @@
         name: &str,
     ) -> AmortizedListIter<impl Iterator<Item = Option<ArrayBox>> + '_> {
         // we create the series container from the inner array
         // so that the container has the proper dtype.
         let arr = self.downcast_iter().next().unwrap();
         let inner_values = arr.values();
 
+        let inner_dtype = self.inner_dtype();
+        let iter_dtype = match inner_dtype {
+            #[cfg(feature = "dtype-struct")]
+            DataType::Struct(_) => inner_dtype.to_physical(),
+            // TODO: figure out how to deal with physical/logical distinction
+            // physical primitives like time, date etc. work
+            // physical nested need more
+            _ => inner_dtype.clone(),
+        };
+
         // Safety:
-        // inner types logical type fits physical type
+        // inner type passed as physical type
         let series_container = unsafe {
             Box::new(Series::from_chunks_and_dtype_unchecked(
                 name,
                 vec![inner_values.clone()],
-                &self.inner_dtype(),
+                &iter_dtype,
             ))
         };
 
         let ptr = series_container.array_ref(0) as *const ArrayRef as *mut ArrayRef;
 
         AmortizedListIter {
             len: self.len(),
             series_container,
             inner: NonNull::new(ptr).unwrap(),
             lifetime: PhantomData,
             iter: self.downcast_iter().flat_map(|arr| arr.iter()),
-            inner_dtype: self.inner_dtype(),
+            inner_dtype,
         }
     }
 
     /// Apply a closure `F` elementwise.
     #[cfg(feature = "private")]
     #[must_use]
     pub fn apply_amortized<'a, F>(&'a self, mut f: F) -> Self
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/list/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/list/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/builder.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+use std::fmt::{Debug, Formatter};
 use std::hash::{Hash, Hasher};
 
 use arrow::array::*;
 use hashbrown::hash_map::{Entry, RawEntryMut};
 use polars_arrow::trusted_len::PushUnchecked;
 use polars_utils::HashSingle;
 
@@ -42,23 +43,36 @@
         match self {
             Local(b) => RevMapping::Local(b.into()),
             GlobalFinished(map, b, uuid) => RevMapping::Global(map, b, uuid),
         }
     }
 }
 
-#[derive(Clone, Debug)]
+#[derive(Clone)]
 pub enum RevMapping {
     /// Hashmap: maps the indexes from the global cache/categorical array to indexes in the local Utf8Array
     /// Utf8Array: caches the string values
     Global(PlHashMap<u32, u32>, Utf8Array<i64>, u128),
     /// Utf8Array: caches the string values
     Local(Utf8Array<i64>),
 }
 
+impl Debug for RevMapping {
+    fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
+        match self {
+            RevMapping::Global(_, _, _) => {
+                write!(f, "global")
+            }
+            RevMapping::Local(_) => {
+                write!(f, "local")
+            }
+        }
+    }
+}
+
 impl Default for RevMapping {
     fn default() -> Self {
         let slice: &[Option<&str>] = &[];
         let cats = Utf8Array::<i64>::from(slice);
         if using_string_cache() {
             let cache = &mut crate::STRING_CACHE.lock_map();
             let id = cache.uuid;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/categorical/stringcache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/date.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/decimal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/duration.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/struct_/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -275,52 +275,30 @@
         let new_fields = arrays_to_fields(&values, &self.fields);
         Box::new(StructArray::new(
             ArrowDataType::Struct(new_fields),
             values,
             None,
         ))
     }
-}
-
-impl LogicalType for StructChunked {
-    fn dtype(&self) -> &DataType {
-        self.field.data_type()
-    }
-
-    /// Gets AnyValue from LogicalType
-    fn get_any_value(&self, i: usize) -> PolarsResult<AnyValue<'_>> {
-        polars_ensure!(i < self.len(), oob = i, self.len());
-        unsafe { Ok(self.get_any_value_unchecked(i)) }
-    }
-
-    unsafe fn get_any_value_unchecked(&self, i: usize) -> AnyValue<'_> {
-        let (chunk_idx, idx) = index_to_chunked_index2(&self.chunks, i);
-        if let DataType::Struct(flds) = self.dtype() {
-            // safety: we already have a single chunk and we are
-            // guarded by the type system.
-            unsafe {
-                let arr = &**self.chunks.get_unchecked(chunk_idx);
-                let arr = &*(arr as *const dyn Array as *const StructArray);
-                AnyValue::Struct(idx, arr, flds)
-            }
-        } else {
-            unreachable!()
-        }
-    }
 
-    // in case of a struct, a cast will coerce the inner types
-    fn cast(&self, dtype: &DataType) -> PolarsResult<Series> {
+    unsafe fn cast_impl(&self, dtype: &DataType, unchecked: bool) -> PolarsResult<Series> {
         match dtype {
             DataType::Struct(dtype_fields) => {
                 let map = BTreeMap::from_iter(self.fields().iter().map(|s| (s.name(), s)));
                 let struct_len = self.len();
                 let new_fields = dtype_fields
                     .iter()
                     .map(|new_field| match map.get(new_field.name().as_str()) {
-                        Some(s) => s.cast(&new_field.dtype),
+                        Some(s) => {
+                            if unchecked {
+                                s.cast_unchecked(&new_field.dtype)
+                            } else {
+                                s.cast(&new_field.dtype)
+                            }
+                        }
                         None => Ok(Series::full_null(
                             new_field.name(),
                             struct_len,
                             &new_field.dtype,
                         )),
                     })
                     .collect::<PolarsResult<Vec<_>>>()?;
@@ -380,20 +358,65 @@
                     Series::try_from((ca.name().as_str(), array))
                 }
             }
             _ => {
                 let fields = self
                     .fields
                     .iter()
-                    .map(|s| s.cast(dtype))
+                    .map(|s| {
+                        if unchecked {
+                            s.cast_unchecked(dtype)
+                        } else {
+                            s.cast(dtype)
+                        }
+                    })
                     .collect::<PolarsResult<Vec<_>>>()?;
                 Ok(Self::new_unchecked(self.field.name(), &fields).into_series())
             }
         }
     }
+
+    pub(crate) unsafe fn cast_unchecked(&self, dtype: &DataType) -> PolarsResult<Series> {
+        if dtype == self.dtype() {
+            return Ok(self.clone().into_series());
+        }
+        self.cast_impl(dtype, true)
+    }
+}
+
+impl LogicalType for StructChunked {
+    fn dtype(&self) -> &DataType {
+        self.field.data_type()
+    }
+
+    /// Gets AnyValue from LogicalType
+    fn get_any_value(&self, i: usize) -> PolarsResult<AnyValue<'_>> {
+        polars_ensure!(i < self.len(), oob = i, self.len());
+        unsafe { Ok(self.get_any_value_unchecked(i)) }
+    }
+
+    unsafe fn get_any_value_unchecked(&self, i: usize) -> AnyValue<'_> {
+        let (chunk_idx, idx) = index_to_chunked_index2(&self.chunks, i);
+        if let DataType::Struct(flds) = self.dtype() {
+            // safety: we already have a single chunk and we are
+            // guarded by the type system.
+            unsafe {
+                let arr = &**self.chunks.get_unchecked(chunk_idx);
+                let arr = &*(arr as *const dyn Array as *const StructArray);
+                AnyValue::Struct(idx, arr, flds)
+            }
+        } else {
+            unreachable!()
+        }
+    }
+
+    // in case of a struct, a cast will coerce the inner types
+    fn cast(&self, dtype: &DataType) -> PolarsResult<Series> {
+        unsafe { self.cast_impl(dtype, false) }
+    }
 }
 
 #[cfg(feature = "object")]
 impl Drop for StructChunked {
     fn drop(&mut self) {
         use crate::chunked_array::object::extension::drop::drop_object_array;
         use crate::chunked_array::object::extension::EXTENSION_NAME;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/logical/time.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/logical/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ndarray.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ndarray.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/builder.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/builder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/extension/polars_extension.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/iterator.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/object/registry.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/object/registry.rs`

 * *Files 17% similar despite different names*

```diff
@@ -22,19 +22,25 @@
     // A function that converts AnyValue to Box<dyn Any> of the object type
     object_converter: ObjectConverter,
 }
 
 static GLOBAL_OBJECT_REGISTRY: Lazy<RwLock<Option<GlobalObjectRegistry>>> =
     Lazy::new(Default::default);
 
+/// This trait can be registers and then that global registration
+/// can be used to materialize object types
 pub trait AnonymousObjectBuilder {
+    /// Append a `null` value.
     fn append_null(&mut self);
 
+    /// Append a `T` of [`ObjectChunked<T>`] made generic via the [`Any`] trait.
     fn append_value(&mut self, value: &dyn Any);
 
+    /// Take the current state and materialize as a [`Series`]
+    /// the builder should not be used after that.
     fn to_series(&mut self) -> Series;
 }
 
 impl<T: PolarsObject> AnonymousObjectBuilder for ObjectChunkedBuilder<T> {
     fn append_null(&mut self) {
         self.append_null()
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/aggregate/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/any_value.rs`

 * *Files 1% similar despite different names*

```diff
@@ -42,16 +42,23 @@
         DataType::Int16 => downcast_and_pack!(Int16Array, Int16),
         DataType::Int32 => downcast_and_pack!(Int32Array, Int32),
         DataType::Int64 => downcast_and_pack!(Int64Array, Int64),
         DataType::Float32 => downcast_and_pack!(Float32Array, Float32),
         DataType::Float64 => downcast_and_pack!(Float64Array, Float64),
         DataType::List(dt) => {
             let v: ArrayRef = downcast!(LargeListArray);
-            let s = Series::from_chunks_and_dtype_unchecked("", vec![v], dt);
-            AnyValue::List(s)
+            if dt.is_primitive() {
+                let s = Series::from_chunks_and_dtype_unchecked("", vec![v], dt);
+                AnyValue::List(s)
+            } else {
+                let s = Series::from_chunks_and_dtype_unchecked("", vec![v], &dt.to_physical())
+                    .cast_unchecked(dt)
+                    .unwrap();
+                AnyValue::List(s)
+            }
         }
         #[cfg(feature = "dtype-categorical")]
         DataType::Categorical(rev_map) => {
             let arr = &*(arr as *const dyn Array as *const UInt32Array);
             let v = arr.value_unchecked(idx);
             AnyValue::Categorical(v, rev_map.as_ref().unwrap().as_ref(), SyncPtr::new_null())
         }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/append.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/append.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/apply.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/bit_repr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/chunkops.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/compare_inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/concat_str.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/cum_agg.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/explode.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/explode.rs`

 * *Files 4% similar despite different names*

```diff
@@ -371,15 +371,22 @@
             if !offsets.is_empty() {
                 let start = offsets[0] as usize;
                 let len = offsets[offsets.len() - 1] as usize - start;
                 // safety:
                 // we are in bounds
                 values = unsafe { values.sliced_unchecked(start, len) };
             }
-            Series::try_from((self.name(), values)).unwrap()
+            // safety: inner_dtype should be correct
+            unsafe {
+                Series::from_chunks_and_dtype_unchecked(
+                    self.name(),
+                    vec![values],
+                    &self.inner_dtype().to_physical(),
+                )
+            }
         } else {
             // during tests
             // test that this code branch is not hit with list arrays that could be fast exploded
             #[cfg(test)]
             {
                 let mut last = offsets[0];
                 let mut has_empty = false;
@@ -390,40 +397,51 @@
                     last = o;
                 }
                 if !has_empty && offsets[0] == 0 {
                     panic!("could have fast exploded")
                 }
             }
 
-            let values = Series::try_from((self.name(), values)).unwrap();
+            // safety: inner_dtype should be correct
+            let values = unsafe {
+                Series::from_chunks_and_dtype_unchecked(
+                    self.name(),
+                    vec![values],
+                    &self.inner_dtype().to_physical(),
+                )
+            };
             values.explode_by_offsets(offsets)
         };
         debug_assert_eq!(s.name(), self.name());
-        // make sure we restore the logical type
-        match self.inner_dtype() {
-            #[cfg(feature = "dtype-categorical")]
-            DataType::Categorical(rev_map) => {
-                let cats = s.u32().unwrap().clone();
-                // safety:
-                // rev_map is from same array, so we are still in bounds
-                s = unsafe {
-                    CategoricalChunked::from_cats_and_rev_map_unchecked(cats, rev_map.unwrap())
-                        .into_series()
-                };
-            }
-            #[cfg(feature = "dtype-date")]
-            DataType::Date => s = s.into_date(),
-            #[cfg(feature = "dtype-datetime")]
-            DataType::Datetime(tu, tz) => s = s.into_datetime(tu, tz),
-            #[cfg(feature = "dtype-duration")]
-            DataType::Duration(tu) => s = s.into_duration(tu),
-            #[cfg(feature = "dtype-time")]
-            DataType::Time => s = s.into_time(),
-            _ => {}
+        // restore logical type
+        unsafe {
+            s = s.cast_unchecked(&self.inner_dtype()).unwrap();
         }
+        // // make sure we restore the logical type
+        // match self.inner_dtype() {
+        //     #[cfg(feature = "dtype-categorical")]
+        //     DataType::Categorical(rev_map) => {
+        //         let cats = s.u32().unwrap().clone();
+        //         // safety:
+        //         // rev_map is from same array, so we are still in bounds
+        //         s = unsafe {
+        //             CategoricalChunked::from_cats_and_rev_map_unchecked(cats, rev_map.unwrap())
+        //                 .into_series()
+        //         };
+        //     }
+        //     #[cfg(feature = "dtype-date")]
+        //     DataType::Date => s = s.into_date(),
+        //     #[cfg(feature = "dtype-datetime")]
+        //     DataType::Datetime(tu, tz) => s = s.into_datetime(tu, tz),
+        //     #[cfg(feature = "dtype-duration")]
+        //     DataType::Duration(tu) => s = s.into_duration(tu),
+        //     #[cfg(feature = "dtype-time")]
+        //     DataType::Time => s = s.into_time(),
+        //     _ => {}
+        // }
 
         Ok((s, offsets_buf))
     }
 }
 
 impl ChunkExplode for Utf8Chunked {
     fn explode_and_offsets(&self) -> PolarsResult<(Series, OffsetsBuffer<i64>)> {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/extend.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/extend.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/fill_null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/filter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/full.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/full.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/is_in.rs`

 * *Files 3% similar despite different names*

```diff
@@ -315,14 +315,15 @@
                         })
                         .collect()
                 };
                 ca.rename(self.name());
                 Ok(ca)
             }
             _ => {
+                let other = other.cast(&other.dtype().to_physical()).unwrap();
                 let other = other.struct_()?;
 
                 polars_ensure!(
                     self.fields().len() == other.fields().len(),
                     ComputeError: "`is_in`: mismatch in the number of struct fields: {} and {}",
                     self.fields().len(), other.fields().len()
                 );
@@ -336,17 +337,23 @@
                 });
 
                 // then we fill the set
                 let mut set = PlHashSet::with_capacity(other.len());
                 for key in anyvalues.chunks_exact(other.fields().len()) {
                     set.insert(key);
                 }
+                // physical self
+                let self_ca = self.cast(&self.dtype().to_physical()).unwrap();
+                let self_ca = self_ca.struct_().unwrap();
+
                 // and then we check for membership
-                let mut ca: BooleanChunked =
-                    self.into_iter().map(|vals| set.contains(&vals)).collect();
+                let mut ca: BooleanChunked = self_ca
+                    .into_iter()
+                    .map(|vals| set.contains(&vals))
+                    .collect();
                 ca.rename(self.name());
                 Ok(ca)
             }
         }
     }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -624,15 +624,19 @@
     }
 }
 
 impl ChunkExpandAtIndex<ListType> for ListChunked {
     fn new_from_index(&self, index: usize, length: usize) -> ListChunked {
         let opt_val = self.get(index);
         match opt_val {
-            Some(val) => ListChunked::full(self.name(), &val, length),
+            Some(val) => {
+                let mut ca = ListChunked::full(self.name(), &val, length);
+                ca.to_logical(self.inner_dtype());
+                ca
+            }
             None => ListChunked::full_null_with_dtype(self.name(), length, &self.inner_dtype()),
         }
     }
 }
 
 #[cfg(feature = "object")]
 impl<T: PolarsObject> ChunkExpandAtIndex<ObjectType<T>> for ObjectChunked<T> {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/peaks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/repeat_by.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/reverse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/set.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/shift.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/shift.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/arg_sort_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/categorical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/sort/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_chunked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_every.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/take_single.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/take/traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/unique/rank.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/ops/zip.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/ops/zip.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/random.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/date.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/date.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/temporal/time.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/temporal/time.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+use std::fmt::Write;
+
 use arrow::temporal_conversions::{time64ns_to_time, NANOSECONDS};
 use chrono::Timelike;
 
 use super::*;
 use crate::prelude::*;
 
 const SECONDS_IN_MINUTE: i64 = 60;
@@ -12,14 +14,44 @@
         + time.minute() as i64 * SECONDS_IN_MINUTE
         + time.second() as i64)
         * NANOSECONDS
         + time.nanosecond() as i64
 }
 
 impl TimeChunked {
+    /// Format Time with a `format` rule. See [chrono strftime/strptime](https://docs.rs/chrono/0.4.19/chrono/format/strftime/index.html).
+    pub fn strftime(&self, format: &str) -> Utf8Chunked {
+        let time = NaiveTime::from_hms_opt(0, 0, 0).unwrap();
+        let fmted = format!("{}", time.format(format));
+
+        let mut ca: Utf8Chunked = self.apply_kernel_cast(&|arr| {
+            let mut buf = String::new();
+            let mut mutarr =
+                MutableUtf8Array::with_capacities(arr.len(), arr.len() * fmted.len() + 1);
+
+            for opt in arr.into_iter() {
+                match opt {
+                    None => mutarr.push_null(),
+                    Some(v) => {
+                        buf.clear();
+                        let timefmt = time64ns_to_time(*v).format(format);
+                        write!(buf, "{timefmt}").unwrap();
+                        mutarr.push(Some(&buf))
+                    }
+                }
+            }
+
+            let arr: Utf8Array<i64> = mutarr.into();
+            Box::new(arr)
+        });
+
+        ca.rename(self.name());
+        ca
+    }
+
     pub fn as_time_iter(&self) -> impl Iterator<Item = Option<NaiveTime>> + TrustedLen + '_ {
         // we know the iterators len
         unsafe {
             self.downcast_iter()
                 .flat_map(|iter| {
                     iter.into_iter()
                         .map(|opt_v| opt_v.copied().map(time64ns_to_time))
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/to_vec.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/to_vec.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/trusted_len.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/trusted_len.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/chunked_array/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/cloud.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/cloud.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/config.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/config.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/_serde.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/_serde.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/aliases.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/aliases.rs`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 pub const IDX_DTYPE: DataType = DataType::UInt64;
 
 #[cfg(not(feature = "bigidx"))]
 pub type IdxType = UInt32Type;
 #[cfg(feature = "bigidx")]
 pub type IdxType = UInt64Type;
 
-pub const NULL_DTYPE: DataType = DataType::Int32;
-
 #[cfg(feature = "private")]
 pub type PlHashMap<K, V> = hashbrown::HashMap<K, V, RandomState>;
 #[cfg(feature = "private")]
 
 /// This hashmap has the uses an IdHasher
 pub type PlIdHashMap<K, V> = hashbrown::HashMap<K, V, IdBuildHasher>;
 #[cfg(feature = "private")]
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/any_value.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/dtype.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/dtype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/field.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/field.rs`

 * *Files 2% similar despite different names*

```diff
@@ -120,29 +120,27 @@
             ArrowDataType::Int8 => DataType::Int8,
             ArrowDataType::Int16 => DataType::Int16,
             ArrowDataType::Int32 => DataType::Int32,
             ArrowDataType::Int64 => DataType::Int64,
             ArrowDataType::Boolean => DataType::Boolean,
             ArrowDataType::Float32 => DataType::Float32,
             ArrowDataType::Float64 => DataType::Float64,
-            ArrowDataType::LargeList(f) => DataType::List(Box::new(f.data_type().into())),
-            ArrowDataType::List(f) => DataType::List(Box::new(f.data_type().into())),
+            ArrowDataType::LargeList(f) | ArrowDataType::List(f) => DataType::List(Box::new(f.data_type().into())),
             ArrowDataType::Date32 => DataType::Date,
             ArrowDataType::Timestamp(tu, tz) => DataType::Datetime(tu.into(), tz.clone()),
             ArrowDataType::Duration(tu) => DataType::Duration(tu.into()),
             ArrowDataType::Date64 => DataType::Datetime(TimeUnit::Milliseconds, None),
             ArrowDataType::LargeUtf8 | ArrowDataType::Utf8 => DataType::Utf8,
             ArrowDataType::LargeBinary | ArrowDataType::Binary => DataType::Binary,
             ArrowDataType::Time64(_) | ArrowDataType::Time32(_) => DataType::Time,
             #[cfg(feature = "dtype-categorical")]
             ArrowDataType::Dictionary(_, _, _) => DataType::Categorical(None),
             #[cfg(feature = "dtype-struct")]
             ArrowDataType::Struct(fields) => {
-                let fields: Vec<Field> = fields.iter().map(|fld| fld.into()).collect();
-                DataType::Struct(fields)
+                DataType::Struct(fields.iter().map(|fld| fld.into()).collect())
             }
             ArrowDataType::Extension(name, _, _) if name == "POLARS_EXTENSION_TYPE" => {
                 #[cfg(feature = "object")]
                 {
                     DataType::Object("extension")
                 }
                 #[cfg(not(feature = "object"))]
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/datatypes/time_unit.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/datatypes/time_unit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_10_0_11.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_7.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_7.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_8.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/doc/changelog/v0_9.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/doc/changelog/v0_9.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/fmt.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/fmt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/arithmetic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/asof_join/asof.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/asof_join/asof.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/asof_join/groups.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/asof_join/groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/asof_join/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/asof_join/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use asof::*;
 use num_traits::Bounded;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 use smartstring::alias::String as SmartString;
 
 use crate::prelude::*;
-use crate::utils::slice_slice;
+use crate::utils::{ensure_sorted_arg, slice_slice};
 
 #[derive(Clone, Debug, PartialEq, Eq, Default)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub struct AsOfOptions {
     pub strategy: AsofStrategy,
     /// A tolerance in the same unit as the asof column
     pub tolerance: Option<AnyValue<'static>>,
@@ -35,14 +35,16 @@
         ComputeError: "mismatching key dtypes in asof-join: `{}` and `{}`",
         a.dtype(), b.dtype()
     );
     polars_ensure!(
         a.null_count() == 0 && b.null_count() == 0,
         ComputeError: "asof join must not have null values in 'on' arguments"
     );
+    ensure_sorted_arg(a);
+    ensure_sorted_arg(b);
     Ok(())
 }
 
 #[derive(Clone, Copy, Debug, PartialEq, Eq, Default)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub enum AsofStrategy {
     /// selects the last row in the right DataFrame whose ‘on’ key is less than or equal to the left’s key
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/chunks.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/cross_join.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/cross_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/explode.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/explode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/agg_list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/aggregations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/hashing.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/hashing.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,52 +1,83 @@
 use std::hash::{BuildHasher, Hash};
 
 use hashbrown::hash_map::{Entry, RawEntryMut};
 use hashbrown::HashMap;
-use polars_utils::{flatten, HashSingle};
+use polars_utils::sync::SyncPtr;
+use polars_utils::HashSingle;
 use rayon::prelude::*;
 
 use super::GroupsProxy;
 use crate::datatypes::PlHashMap;
-use crate::frame::groupby::{GroupsIdx, IdxItem};
+use crate::frame::groupby::GroupsIdx;
 use crate::hashing::{
     df_rows_to_hashes_threaded_vertical, this_partition, AsU64, IdBuildHasher, IdxHash,
 };
 use crate::prelude::compare_inner::PartialEqInner;
 use crate::prelude::*;
 use crate::utils::{split_df, CustomIterTools};
 use crate::POOL;
 
-fn finish_group_order(mut out: Vec<Vec<IdxItem>>, sorted: bool) -> GroupsProxy {
+fn finish_group_order_vecs(
+    mut vecs: Vec<(Vec<IdxSize>, Vec<Vec<IdxSize>>)>,
+    sorted: bool,
+) -> GroupsProxy {
     if sorted {
-        // we can just take the first value, no need to flatten
-        let mut out = if out.len() == 1 {
-            out.pop().unwrap()
-        } else {
-            // pre-sort every array
-            // this will make the final single threaded sort much faster
-            POOL.install(|| {
-                out.par_iter_mut()
-                    .for_each(|g| g.sort_unstable_by_key(|g| g.0))
-            });
-
-            flatten(&out, None)
-        };
-        out.sort_unstable_by_key(|g| g.0);
-        let mut idx = GroupsIdx::from_iter(out.into_iter());
+        if vecs.len() == 1 {
+            let (first, all) = vecs.pop().unwrap();
+            return GroupsProxy::Idx(GroupsIdx::new(first, all, true));
+        }
+
+        let cap = vecs.iter().map(|v| v.0.len()).sum::<usize>();
+        let offsets = vecs
+            .iter()
+            .scan(0_usize, |acc, v| {
+                let out = *acc;
+                *acc += v.0.len();
+                Some(out)
+            })
+            .collect::<Vec<_>>();
+
+        // we write (first, all) tuple because of sorting
+        let mut items = Vec::with_capacity(cap);
+        let items_ptr = unsafe { SyncPtr::new(items.as_mut_ptr()) };
+
+        POOL.install(|| {
+            vecs.into_par_iter()
+                .zip(offsets)
+                .for_each(|((first, all), offset)| {
+                    // pre-sort every array not needed as items are already sorted
+                    // this is due to using an index hashmap
+
+                    unsafe {
+                        let mut items_ptr: *mut (IdxSize, Vec<IdxSize>) = items_ptr.get();
+                        items_ptr = items_ptr.add(offset);
+
+                        // give the compiler some info
+                        // maybe it may elide some loop counters
+                        assert_eq!(first.len(), all.len());
+                        for (i, (first, all)) in first.into_iter().zip(all.into_iter()).enumerate()
+                        {
+                            std::ptr::write(items_ptr.add(i), (first, all))
+                        }
+                    }
+                });
+        });
+        unsafe {
+            items.set_len(cap);
+        }
+        // sort again
+        items.sort_unstable_by_key(|g| g.0);
+
+        let mut idx = GroupsIdx::from_iter(items.into_iter());
         idx.sorted = true;
         GroupsProxy::Idx(idx)
     } else {
-        // we can just take the first value, no need to flatten
-        if out.len() == 1 {
-            GroupsProxy::Idx(GroupsIdx::from(out.pop().unwrap()))
-        } else {
-            // flattens
-            GroupsProxy::Idx(GroupsIdx::from(out))
-        }
+        // this materialization is parallel in the from impl.
+        GroupsProxy::Idx(GroupsIdx::from(vecs))
     }
 }
 
 // We must strike a balance between cache coherence and resizing costs.
 // Overallocation seems a lot more expensive than resizing so we start reasonable small.
 pub(crate) const HASHMAP_INIT_SIZE: usize = 512;
 
@@ -97,60 +128,67 @@
     T: Send + Hash + Eq + Sync + Copy + AsU64,
 {
     assert!(n_partitions.is_power_of_two());
 
     // We will create a hashtable in every thread.
     // We use the hash to partition the keys to the matching hashtable.
     // Every thread traverses all keys/hashes and ignores the ones that doesn't fall in that partition.
-    let out = POOL.install(|| {
+    let v = POOL.install(|| {
         (0..n_partitions)
             .into_par_iter()
             .map(|thread_no| {
-                let mut hash_tbl: PlHashMap<T, (IdxSize, Vec<IdxSize>)> =
+                let mut hash_tbl: PlHashMap<T, IdxSize> =
                     PlHashMap::with_capacity(HASHMAP_INIT_SIZE);
+                let mut first_vals = Vec::with_capacity(HASHMAP_INIT_SIZE);
+                let mut all_vals = Vec::with_capacity(HASHMAP_INIT_SIZE);
 
                 let mut offset = 0;
                 for keys in keys {
                     let keys = keys.into_iter();
                     let len = keys.len() as IdxSize;
                     let hasher = hash_tbl.hasher().clone();
 
                     let mut cnt = 0;
                     keys.for_each(|k| {
-                        let idx = cnt + offset;
+                        let row_idx = cnt + offset;
                         cnt += 1;
 
                         if this_partition(k.as_u64(), thread_no, n_partitions) {
                             let hash = hasher.hash_single(k);
                             let entry = hash_tbl.raw_entry_mut().from_key_hashed_nocheck(hash, &k);
 
                             match entry {
                                 RawEntryMut::Vacant(entry) => {
-                                    let tuples = vec![idx];
-                                    entry.insert_with_hasher(hash, k, (idx, tuples), |k| {
+                                    let offset_idx = first_vals.len() as IdxSize;
+
+                                    let tuples = vec![row_idx];
+                                    all_vals.push(tuples);
+                                    first_vals.push(row_idx);
+
+                                    entry.insert_with_hasher(hash, k, offset_idx, |k| {
                                         hasher.hash_single(k)
                                     });
                                 }
-                                RawEntryMut::Occupied(mut entry) => {
-                                    let v = entry.get_mut();
-                                    v.1.push(idx);
+                                RawEntryMut::Occupied(entry) => {
+                                    let offset_idx = *entry.get();
+                                    unsafe {
+                                        let buf = all_vals.get_unchecked_mut(offset_idx as usize);
+                                        buf.push(row_idx)
+                                    }
                                 }
                             }
                         }
                     });
                     offset += len;
                 }
-                hash_tbl
-                    .into_iter()
-                    .map(|(_k, v)| v)
-                    .collect_trusted::<Vec<_>>()
+                (first_vals, all_vals)
             })
             .collect::<Vec<_>>()
     });
-    finish_group_order(out, sorted)
+    finish_group_order_vecs(v, sorted)
 }
 
 /// Utility function used as comparison function in the hashmap.
 /// The rationale is that equality is an AND operation and therefore its probability of success
 /// declines rapidly with the number of keys. Instead of first copying an entire row from both
 /// sides and then do the comparison, we do the comparison value by value catching early failures
 /// eagerly.
@@ -180,18 +218,18 @@
     original_h: u64,
     // keys of the hash table (will not be inserted, the indexes will be used)
     // the keys are needed for the equality check
     keys: &DataFrame,
     // value to insert
     vacant_fn: G,
     // function that gets a mutable ref to the occupied value in the hash table
-    occupied_fn: F,
+    mut occupied_fn: F,
 ) where
     G: Fn() -> V,
-    F: Fn(&mut V),
+    F: FnMut(&mut V),
     H: BuildHasher,
 {
     let entry = hash_tbl
         .raw_entry_mut()
         // uses the idx to probe rows in the original DataFrame with keys
         // to check equality to find an entry
         // this does not invalidate the hashmap as this equality function is not used
@@ -294,48 +332,74 @@
         .iter()
         .map(|s| s.into_partial_eq_inner())
         .collect::<Vec<_>>();
 
     // We will create a hashtable in every thread.
     // We use the hash to partition the keys to the matching hashtable.
     // Every thread traverses all keys/hashes and ignores the ones that doesn't fall in that partition.
-    let groups = POOL.install(|| {
+    let v = POOL.install(|| {
         (0..n_partitions)
             .into_par_iter()
             .map(|thread_no| {
                 let hashes = &hashes;
 
-                let mut hash_tbl: HashMap<IdxHash, (IdxSize, Vec<IdxSize>), IdBuildHasher> =
+                let mut hash_tbl: HashMap<IdxHash, IdxSize, IdBuildHasher> =
                     HashMap::with_capacity_and_hasher(HASHMAP_INIT_SIZE, Default::default());
+                let mut first_vals = Vec::with_capacity(HASHMAP_INIT_SIZE);
+                let mut all_vals = Vec::with_capacity(HASHMAP_INIT_SIZE);
+
+                // put the buffers behind a pointer so we can access them from as the bchk doesn't allow
+                // 2 mutable borrows (this is safe as we don't alias)
+                // even if the vecs reallocate, we have a pointer to the stack vec, and thus always
+                // access the proper data.
+                let all_buf_ptr =
+                    &mut all_vals as *mut Vec<Vec<IdxSize>> as *const Vec<Vec<IdxSize>>;
+                let first_buf_ptr = &mut first_vals as *mut Vec<IdxSize> as *const Vec<IdxSize>;
 
                 let mut offset = 0;
                 for hashes in hashes {
                     let len = hashes.len() as IdxSize;
 
                     let mut idx = 0;
                     for hashes_chunk in hashes.data_views() {
                         for &h in hashes_chunk {
                             // partition hashes by thread no.
                             // So only a part of the hashes go to this hashmap
                             if this_partition(h, thread_no, n_partitions) {
-                                let idx = idx + offset;
+                                let row_idx = idx + offset;
                                 populate_multiple_key_hashmap2(
                                     &mut hash_tbl,
-                                    idx,
+                                    row_idx,
                                     h,
                                     &keys_cmp,
-                                    || (idx, vec![idx]),
-                                    |v| v.1.push(idx),
+                                    || unsafe {
+                                        let first_vals = &mut *(first_buf_ptr as *mut Vec<IdxSize>);
+                                        let all_vals =
+                                            &mut *(all_buf_ptr as *mut Vec<Vec<IdxSize>>);
+                                        let offset_idx = first_vals.len() as IdxSize;
+
+                                        let tuples = vec![row_idx];
+                                        all_vals.push(tuples);
+                                        first_vals.push(row_idx);
+                                        offset_idx
+                                    },
+                                    |v| unsafe {
+                                        let all_vals =
+                                            &mut *(all_buf_ptr as *mut Vec<Vec<IdxSize>>);
+                                        let offset_idx = *v;
+                                        let buf = all_vals.get_unchecked_mut(offset_idx as usize);
+                                        buf.push(row_idx)
+                                    },
                                 );
                             }
                             idx += 1;
                         }
                     }
 
                     offset += len;
                 }
-                hash_tbl.into_iter().map(|(_k, v)| v).collect::<Vec<_>>()
+                (first_vals, all_vals)
             })
             .collect::<Vec<_>>()
     });
-    Ok(finish_group_order(groups, sorted))
+    Ok(finish_group_order_vecs(v, sorted))
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/into_groups.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/into_groups.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -757,15 +757,15 @@
     /// | 2020-08-21 | "[Some(20), Some(10)]" |
     /// +------------+------------------------+
     /// ```
     #[deprecated(since = "0.24.1", note = "use polars.lazy aggregations")]
     pub fn agg_list(&self) -> PolarsResult<DataFrame> {
         let (mut cols, agg_cols) = self.prepare_agg()?;
         for agg_col in agg_cols {
-            let new_name = fmt_groupby_column(agg_col.name(), GroupByMethod::List);
+            let new_name = fmt_groupby_column(agg_col.name(), GroupByMethod::Implode);
             let mut agg = unsafe { agg_col.agg_list(&self.groups) };
             agg.rename(&new_name);
             cols.push(agg);
         }
         DataFrame::new(cols)
     }
 
@@ -849,15 +849,15 @@
     First,
     Last,
     Sum,
     Groups,
     NUnique,
     Quantile(f64, QuantileInterpolOptions),
     Count,
-    List,
+    Implode,
     Std(u8),
     Var(u8),
 }
 
 impl Display for GroupByMethod {
     fn fmt(&self, f: &mut Formatter<'_>) -> std::fmt::Result {
         use GroupByMethod::*;
@@ -871,15 +871,15 @@
             First => "first",
             Last => "last",
             Sum => "sum",
             Groups => "groups",
             NUnique => "n_unique",
             Quantile(_, _) => "quantile",
             Count => "count",
-            List => "list",
+            Implode => "list",
             Std(_) => "std",
             Var(_) => "var",
         };
         write!(f, "{s}")
     }
 }
 
@@ -895,28 +895,26 @@
         Mean => format!("{name}_mean"),
         First => format!("{name}_first"),
         Last => format!("{name}_last"),
         Sum => format!("{name}_sum"),
         Groups => "groups".to_string(),
         NUnique => format!("{name}_n_unique"),
         Count => format!("{name}_count"),
-        List => format!("{name}_agg_list"),
+        Implode => format!("{name}_agg_list"),
         Quantile(quantile, _interpol) => format!("{name}_quantile_{quantile:.2}"),
         Std(_) => format!("{name}_agg_std"),
         Var(_) => format!("{name}_agg_var"),
     }
 }
 
 #[cfg(test)]
 mod test {
     use num_traits::FloatConst;
 
-    use crate::frame::groupby::groupby;
     use crate::prelude::*;
-    use crate::utils::split_ca;
 
     #[test]
     #[cfg(feature = "dtype-date")]
     #[cfg_attr(miri, ignore)]
     fn test_group_by() -> PolarsResult<()> {
         let s0 = Series::new(
             "date",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/perfect.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/perfect.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/groupby/proxy.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/groupby/proxy.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use std::mem::ManuallyDrop;
 use std::ops::Deref;
 
 use polars_arrow::utils::CustomIterTools;
+use polars_utils::sync::SyncPtr;
 use rayon::iter::plumbing::UnindexedConsumer;
 use rayon::prelude::*;
 
 use crate::prelude::*;
 use crate::utils::{slice_slice, NoNull};
 use crate::POOL;
 
@@ -40,60 +41,62 @@
 
 impl From<Vec<IdxItem>> for GroupsIdx {
     fn from(v: Vec<IdxItem>) -> Self {
         v.into_iter().collect()
     }
 }
 
-impl From<Vec<Vec<IdxItem>>> for GroupsIdx {
-    fn from(v: Vec<Vec<IdxItem>>) -> Self {
-        // single threaded flatten: 10% faster than `iter().flatten().collect()
-        // this is the multi-threaded impl of that
-        let cap = v.iter().map(|v| v.len()).sum::<usize>();
+impl From<Vec<(Vec<IdxSize>, Vec<Vec<IdxSize>>)>> for GroupsIdx {
+    fn from(v: Vec<(Vec<IdxSize>, Vec<Vec<IdxSize>>)>) -> Self {
+        // we have got the hash tables so we can determine the final
+        let cap = v.iter().map(|v| v.0.len()).sum::<usize>();
         let offsets = v
             .iter()
             .scan(0_usize, |acc, v| {
                 let out = *acc;
-                *acc += v.len();
+                *acc += v.0.len();
                 Some(out)
             })
             .collect::<Vec<_>>();
-        let mut first = Vec::with_capacity(cap);
-        let first_ptr = first.as_ptr() as usize;
-        let mut all = Vec::with_capacity(cap);
-        let all_ptr = all.as_ptr() as usize;
+        let mut global_first = Vec::with_capacity(cap);
+        let global_first_ptr = unsafe { SyncPtr::new(global_first.as_mut_ptr()) };
+        let mut global_all = Vec::with_capacity(cap);
+        let global_all_ptr = unsafe { SyncPtr::new(global_all.as_mut_ptr()) };
 
         POOL.install(|| {
-            v.into_par_iter()
-                .zip(offsets)
-                .for_each(|(mut inner, offset)| {
-                    unsafe {
-                        let first = (first_ptr as *const IdxSize as *mut IdxSize).add(offset);
-                        let all = (all_ptr as *const Vec<IdxSize> as *mut Vec<IdxSize>).add(offset);
-
-                        let inner_ptr = inner.as_mut_ptr();
-                        for i in 0..inner.len() {
-                            let (first_val, vals) = std::ptr::read(inner_ptr.add(i));
-                            std::ptr::write(first.add(i), first_val);
-                            std::ptr::write(all.add(i), vals);
-                        }
-                        // set len to 0 so that the contents will not get dropped
-                        // they are moved to `first` and `all`
-                        inner.set_len(0);
-                    }
-                });
+            v.into_par_iter().zip(offsets).for_each(
+                |((local_first_vals, local_all_vals), offset)| unsafe {
+                    let global_first: *mut IdxSize = global_first_ptr.get();
+                    let global_all: *mut Vec<IdxSize> = global_all_ptr.get();
+                    let global_first = global_first.add(offset);
+                    let global_all = global_all.add(offset);
+
+                    std::ptr::copy_nonoverlapping(
+                        local_first_vals.as_ptr(),
+                        global_first,
+                        local_first_vals.len(),
+                    );
+                    std::ptr::copy_nonoverlapping(
+                        local_all_vals.as_ptr(),
+                        global_all,
+                        local_all_vals.len(),
+                    );
+                    // ensure the vecs don't get dropped
+                    std::mem::forget(local_all_vals);
+                },
+            );
         });
         unsafe {
-            all.set_len(cap);
-            first.set_len(cap);
+            global_all.set_len(cap);
+            global_first.set_len(cap);
         }
         GroupsIdx {
             sorted: false,
-            first,
-            all,
+            first: global_first,
+            all: global_all,
         }
     }
 }
 
 impl GroupsIdx {
     pub fn new(first: Vec<IdxSize>, all: Vec<Vec<IdxSize>>, sorted: bool) -> Self {
         Self { sorted, first, all }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/multiple_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_outer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/single_keys_semi_anti.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/hash_join/sort_merge.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -492,21 +492,21 @@
     /// ```rust
     /// # use polars_core::prelude::*;
     /// let df: DataFrame = df!("Thing" => &["Observable universe", "Human stupidity"],
     ///                         "Diameter (m)" => &[8.8e26, f64::INFINITY])?;
     ///
     /// let f1: Field = Field::new("Thing", DataType::Utf8);
     /// let f2: Field = Field::new("Diameter (m)", DataType::Float64);
-    /// let sc: Schema = Schema::from(vec![f1, f2].into_iter());
+    /// let sc: Schema = Schema::from_iter(vec![f1, f2]);
     ///
     /// assert_eq!(df.schema(), sc);
     /// # Ok::<(), PolarsError>(())
     /// ```
     pub fn schema(&self) -> Schema {
-        Schema::from(self.iter().map(|s| s.field().into_owned()))
+        self.iter().map(|s| s.field().into_owned()).collect()
     }
 
     /// Get a reference to the `DataFrame` columns.
     ///
     /// # Example
     ///
     /// ```rust
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/av_buffer.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/av_buffer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,14 @@
                 match self {
                     Utf8(builder) => {
                         let AnyValue::Utf8(v) = val else { unreachable_unchecked_release!() };
                         builder.append_value(v)
                     }
                     #[cfg(feature = "dtype-struct")]
                     Struct(builders) => {
-                        dbg!(&val);
                         let AnyValue::Struct(idx, arr, fields) = val else { unreachable_unchecked_release!() };
                         let arrays = arr.values();
                         // amortize loop counter
                         for i in 0..fields.len() {
                             unsafe {
                                 let array = arrays.get_unchecked_release(i);
                                 let field = fields.get_unchecked_release(i);
@@ -566,15 +565,19 @@
                         let mut s = b.reset(capacity);
                         s.rename(name.as_str());
                         s
                     })
                     .collect::<Vec<_>>();
                 StructChunked::new("", &v).unwrap().into_series()
             }
-            All(dtype, vals) => Series::from_any_values_and_dtype("", vals, dtype, false).unwrap(),
+            All(dtype, vals) => {
+                let mut swap_vals = Vec::with_capacity(capacity);
+                std::mem::swap(vals, &mut swap_vals);
+                Series::from_any_values_and_dtype("", &swap_vals, dtype, false).unwrap()
+            }
         }
     }
 
     pub fn into_series(mut self) -> Series {
         self.reset(0)
     }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/dataframe.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/dataframe.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
     let max_infer = std::cmp::min(len, infer_schema_length);
     for inner in iter.take(max_infer) {
         for (key, value) in inner {
             add_or_insert(&mut values, &key, value.into());
         }
     }
-    Schema::from(resolve_fields(values).into_iter())
+    Schema::from_iter(resolve_fields(values))
 }
 
 fn add_or_insert(values: &mut Tracker, key: &str, data_type: DataType) {
     if data_type == DataType::Null {
         return;
     }
 
@@ -170,15 +170,15 @@
             break;
         } else {
             for i in nulls {
                 let val = &row.0[i];
 
                 if !is_nested_null(val) {
                     let dtype = val.into();
-                    schema.coerce_by_index(i, dtype).unwrap();
+                    schema.set_dtype_at_index(i, dtype).unwrap();
                 }
             }
         }
     }
     schema
 }
 
@@ -186,15 +186,17 @@
     fn from(val: &AnyValue<'a>) -> Self {
         Field::new("", val.into())
     }
 }
 
 impl From<&Row<'_>> for Schema {
     fn from(row: &Row) -> Self {
-        let fields = row.0.iter().enumerate().map(|(i, av)| {
-            let dtype = av.into();
-            Field::new(format!("column_{i}").as_ref(), dtype)
-        });
-
-        Schema::from(fields)
+        row.0
+            .iter()
+            .enumerate()
+            .map(|(i, av)| {
+                let dtype = av.into();
+                Field::new(format!("column_{i}").as_ref(), dtype)
+            })
+            .collect()
     }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/row/transpose.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/row/transpose.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/top_k.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/top_k.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/frame/upstream_traits.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/frame/upstream_traits.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/fx.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/fx.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/identity.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/identity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/partition.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/hashing/vector_hasher.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/hashing/vector_hasher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/named_from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/named_from.rs`

 * *Files 2% similar despite different names*

```diff
@@ -146,21 +146,18 @@
 
 impl<T: AsRef<[Option<Series>]>> NamedFrom<T, [Option<Series>]> for Series {
     fn new(name: &str, s: T) -> Self {
         let series_slice = s.as_ref();
         let values_cap = series_slice.iter().fold(0, |acc, opt_s| {
             acc + opt_s.as_ref().map(|s| s.len()).unwrap_or(0)
         });
-
-        let dt = series_slice
-            .iter()
-            .filter_map(|opt| opt.as_ref())
-            .next()
-            .expect("cannot create List Series from a slice of nulls")
-            .dtype();
+        let dt = match series_slice.iter().filter_map(|opt| opt.as_ref()).next() {
+            Some(series) => series.dtype(),
+            None => &DataType::Null,
+        };
 
         let mut builder = get_list_builder(dt, values_cap, series_slice.len(), name).unwrap();
         for series in series_slice {
             builder.append_opt_series(series.as_ref())
         }
         builder.finish().into_series()
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/prelude.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/serde/chunked_array.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/serde/chunked_array.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/serde/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/serde/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/serde/series.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/serde/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/any_value.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/any_value.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/arithmetic/borrowed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/arithmetic/owned.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/arithmetic/owned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/comparison.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/comparison.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/from.rs`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 use polars_arrow::kernels::concatenate::concatenate_owned_unchecked;
 
 use crate::chunked_array::cast::cast_chunks;
 #[cfg(feature = "object")]
 use crate::chunked_array::object::extension::polars_extension::PolarsExtension;
 #[cfg(feature = "object")]
 use crate::chunked_array::object::extension::EXTENSION_NAME;
-#[cfg(feature = "dtype-decimal")]
+#[cfg(all(feature = "dtype-decimal", feature = "python"))]
 use crate::config::decimal_is_active;
 use crate::config::verbose;
 use crate::prelude::*;
 
 impl Series {
     /// Takes chunks and a polars datatype and constructs the Series
     /// This is faster than creating from chunks and an arrow datatype because there is no
@@ -83,15 +83,31 @@
             }
             Boolean => BooleanChunked::from_chunks(name, chunks).into_series(),
             Float32 => Float32Chunked::from_chunks(name, chunks).into_series(),
             Float64 => Float64Chunked::from_chunks(name, chunks).into_series(),
             #[cfg(feature = "dtype-struct")]
             Struct(_) => Series::try_from_arrow_unchecked(name, chunks, &dtype.to_arrow()).unwrap(),
             #[cfg(feature = "object")]
-            Object(_) => todo!(),
+            Object(_) => {
+                assert_eq!(chunks.len(), 1);
+                let arr = chunks[0]
+                    .as_any()
+                    .downcast_ref::<FixedSizeBinaryArray>()
+                    .unwrap();
+                // Safety:
+                // this is highly unsafe. it will dereference a raw ptr on the heap
+                // make sure the ptr is allocated and from this pid
+                // (the pid is checked before dereference)
+                {
+                    let pe = PolarsExtension::new(arr.clone());
+                    let s = pe.get_series(name);
+                    pe.take_and_forget();
+                    s
+                }
+            }
             Null => new_null(name, &chunks),
             Unknown => panic!("uh oh, somehow we don't know the dtype?"),
             #[allow(unreachable_patterns)]
             _ => unreachable!(),
         }
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/binary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/categorical.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/categorical.rs`

 * *Files 0% similar despite different names*

```diff
@@ -103,19 +103,18 @@
     fn vec_hash_combine(&self, build_hasher: RandomState, hashes: &mut [u64]) -> PolarsResult<()> {
         self.0.logical().vec_hash_combine(build_hasher, hashes);
         Ok(())
     }
 
     unsafe fn agg_list(&self, groups: &GroupsProxy) -> Series {
         // we cannot cast and dispatch as the inner type of the list would be incorrect
-        self.0
-            .logical()
-            .agg_list(groups)
-            .cast(&DataType::List(Box::new(self.dtype().clone())))
-            .unwrap()
+        let list = self.0.logical().agg_list(groups);
+        let mut list = list.list().unwrap().clone();
+        list.to_logical(self.dtype().clone());
+        list.into_series()
     }
 
     fn zip_outer_join_column(
         &self,
         right_column: &Series,
         opt_join_tuples: &[(Option<IdxSize>, Option<IdxSize>)],
     ) -> Series {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/dates_time.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/dates_time.rs`

 * *Files 2% similar despite different names*

```diff
@@ -305,14 +305,22 @@
                         .0
                         .clone()
                         .into_series()
                         .date()
                         .unwrap()
                         .strftime("%Y-%m-%d")
                         .into_series()),
+                    (DataType::Time, DataType::Utf8) => Ok(self
+                        .0
+                        .clone()
+                        .into_series()
+                        .time()
+                        .unwrap()
+                        .strftime("%T")
+                        .into_series()),
                     #[cfg(feature = "dtype-datetime")]
                     (DataType::Time, DataType::Datetime(_, _)) => {
                         polars_bail!(
                             ComputeError:
                             "cannot cast `Time` to `Datetime`; consider using 'dt.combine'"
                         );
                     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/datetime.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/decimal.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/decimal.rs`

 * *Files 2% similar despite different names*

```diff
@@ -189,8 +189,12 @@
     fn reverse(&self) -> Series {
         self.apply_logical(|ca| ca.reverse())
     }
 
     fn shift(&self, periods: i64) -> Series {
         self.apply_logical(|ca| ca.shift(periods))
     }
+
+    fn clone_inner(&self) -> Arc<dyn SeriesTrait> {
+        Arc::new(SeriesWrap(Clone::clone(&self.0)))
+    }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/duration.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/duration.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/floats.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/floats.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/null.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/null.rs`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,18 @@
         *self = NullChunked::new(self.name.clone(), self.len() + other.len());
         Ok(())
     }
 
     fn extend(&mut self, other: &Series) -> PolarsResult<()> {
         self.append(other)
     }
+
+    fn clone_inner(&self) -> Arc<dyn SeriesTrait> {
+        Arc::new(self.clone())
+    }
 }
 
 unsafe impl IntoSeries for NullChunked {
     fn into_series(self) -> Series
     where
         Self: Sized,
     {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/object.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/object.rs`

 * *Files 2% similar despite different names*

```diff
@@ -163,16 +163,22 @@
         self.0.take_every(n).into_series()
     }
 
     fn new_from_index(&self, index: usize, length: usize) -> Series {
         ChunkExpandAtIndex::new_from_index(&self.0, index, length).into_series()
     }
 
-    fn cast(&self, _data_type: &DataType) -> PolarsResult<Series> {
-        polars_bail!(opq = cast, self.dtype());
+    fn cast(&self, data_type: &DataType) -> PolarsResult<Series> {
+        if matches!(data_type, DataType::Object(_)) {
+            Ok(self.0.clone().into_series())
+        } else {
+            Err(PolarsError::ComputeError(
+                "cannot cast 'Object' type".into(),
+            ))
+        }
     }
 
     fn get(&self, index: usize) -> PolarsResult<AnyValue> {
         ObjectChunked::get_any_value(&self.0, index)
     }
     fn null_count(&self) -> usize {
         ObjectChunked::null_count(&self.0)
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/struct_.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/implementations/utf8.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/implementations/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/into.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/into.rs`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,26 @@
                 let ca = self.list().unwrap();
                 let arr = ca.chunks[chunk_idx].clone();
                 let arr = arr.as_any().downcast_ref::<ListArray<i64>>().unwrap();
 
                 let new_values = if let DataType::Null = &**inner {
                     arr.values().clone()
                 } else {
+                    // we pass physical arrays
+                    // and cast to logical before we convert to arrow
                     let s = unsafe {
                         Series::from_chunks_and_dtype_unchecked(
                             "",
                             vec![arr.values().clone()],
-                            inner,
+                            &inner.to_physical(),
                         )
+                        .cast_unchecked(inner)
+                        .unwrap()
                     };
+
                     s.to_arrow(0)
                 };
 
                 let data_type = ListArray::<i64>::default_datatype(inner.to_arrow());
                 let arr = ListArray::<i64>::new(
                     data_type,
                     arr.offsets().clone(),
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/iterator.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -263,14 +263,23 @@
 
     /// Cast from physical to logical types without any checks on the validity of the cast.
     ///
     /// # Safety
     /// This can lead to invalid memory access in downstream code.
     pub unsafe fn cast_unchecked(&self, dtype: &DataType) -> PolarsResult<Self> {
         match self.dtype() {
+            #[cfg(feature = "dtype-struct")]
+            DataType::Struct(_) => {
+                let ca = self.struct_().unwrap();
+                ca.cast_unchecked(dtype)
+            }
+            DataType::List(_) => {
+                let ca = self.list().unwrap();
+                ca.cast_unchecked(dtype)
+            }
             dt if dt.is_numeric() => {
                 with_match_physical_numeric_polars_type!(dt, |$T| {
                     let ca: &ChunkedArray<$T> = self.as_ref().as_ref().as_ref();
                         ca.cast_unchecked(dtype)
                 })
             }
             _ => self.cast(dtype),
@@ -717,16 +726,23 @@
         rank(self, options.method, options.descending, seed)
     }
 
     /// Cast throws an error if conversion had overflows
     pub fn strict_cast(&self, dtype: &DataType) -> PolarsResult<Series> {
         let null_count = self.null_count();
         let len = self.len();
-        if null_count == len {
-            return Ok(Series::full_null(self.name(), len, dtype));
+
+        match self.dtype() {
+            #[cfg(feature = "dtype-struct")]
+            DataType::Struct(_) => {}
+            _ => {
+                if null_count == len {
+                    return Ok(Series::full_null(self.name(), len, dtype));
+                }
+            }
         }
         let s = self.0.cast(dtype)?;
         if null_count != s.null_count() {
             let failure_mask = !self.is_null() & s.is_null();
             let failures = self.filter_threaded(&failure_mask, false)?.unique()?;
             polars_bail!(
                 ComputeError:
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/diff.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/diff.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/downcast.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/downcast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/ewm.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/ewm.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/moment.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/moment.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/null.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/pct_change.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/pct_change.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/round.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/round.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/to_list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/to_list.rs`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     ca.into_series()
 }
 
 impl Series {
     /// Convert the values of this Series to a ListChunked with a length of 1,
     /// So a Series of:
     /// `[1, 2, 3]` becomes `[[1, 2, 3]]`
-    pub fn to_list(&self) -> PolarsResult<ListChunked> {
+    pub fn implode(&self) -> PolarsResult<ListChunked> {
         let s = self.rechunk();
         let values = s.array_ref(0);
 
         let offsets = vec![0i64, values.len() as i64];
         let inner_type = self.dtype();
 
         let data_type = ListArray::<i64>::default_datatype(values.data_type().clone());
@@ -140,15 +140,15 @@
     fn test_to_list() -> PolarsResult<()> {
         let s = Series::new("a", &[1, 2, 3]);
 
         let mut builder = get_list_builder(s.dtype(), s.len(), 1, s.name())?;
         builder.append_series(&s);
         let expected = builder.finish();
 
-        let out = s.to_list()?;
+        let out = s.implode()?;
         assert!(expected.into_series().series_equal(&out.into_series()));
 
         Ok(())
     }
 
     #[test]
     fn test_reshape() -> PolarsResult<()> {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/ops/unique.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/ops/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/series_trait.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/series_trait.rs`

 * *Files 1% similar despite different names*

```diff
@@ -461,17 +461,15 @@
         _quantile: f64,
         _interpol: QuantileInterpolOptions,
     ) -> PolarsResult<Series> {
         Ok(Series::full_null(self.name(), 1, self.dtype()))
     }
 
     /// Clone inner ChunkedArray and wrap in a new Arc
-    fn clone_inner(&self) -> Arc<dyn SeriesTrait> {
-        invalid_operation_panic!(clone_inner, self)
-    }
+    fn clone_inner(&self) -> Arc<dyn SeriesTrait>;
 
     #[cfg(feature = "object")]
     /// Get the value at this index as a downcastable Any trait ref.
     fn get_object(&self, _index: usize) -> Option<&dyn PolarsObjectSafe> {
         invalid_operation_panic!(get_object, self)
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/series/unstable.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/series/unstable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/testing.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/testing.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/utils/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+pub mod flatten;
 pub(crate) mod series;
 mod supertype;
-
 use std::borrow::Cow;
 use std::ops::{Deref, DerefMut};
 
 use arrow::bitmap::Bitmap;
+use flatten::*;
 use num_traits::{One, Zero};
 pub use polars_arrow::utils::{TrustMyLength, *};
 use rayon::prelude::*;
 pub use series::*;
 use smartstring::alias::String as SmartString;
 pub use supertype::*;
 pub use {arrow, rayon};
@@ -138,49 +139,14 @@
 
 #[cfg(feature = "private")]
 #[doc(hidden)]
 pub fn split_series(s: &Series, n: usize) -> PolarsResult<Vec<Series>> {
     split_array!(s, n, i64)
 }
 
-fn flatten_df(df: &DataFrame) -> impl Iterator<Item = DataFrame> + '_ {
-    df.iter_chunks_physical().flat_map(|chunk| {
-        let df = DataFrame::new_no_checks(
-            df.iter()
-                .zip(chunk.into_arrays())
-                .map(|(s, arr)| {
-                    // Safety:
-                    // datatypes are correct
-                    let mut out = unsafe {
-                        Series::from_chunks_and_dtype_unchecked(s.name(), vec![arr], s.dtype())
-                    };
-                    out.set_sorted_flag(s.is_sorted_flag());
-                    out
-                })
-                .collect(),
-        );
-        if df.height() == 0 {
-            None
-        } else {
-            Some(df)
-        }
-    })
-}
-
-pub fn flatten_series(s: &Series) -> Vec<Series> {
-    let name = s.name();
-    let dtype = s.dtype();
-    unsafe {
-        s.chunks()
-            .iter()
-            .map(|arr| Series::from_chunks_and_dtype_unchecked(name, vec![arr.clone()], dtype))
-            .collect()
-    }
-}
-
 pub fn split_df_as_ref(df: &DataFrame, n: usize) -> PolarsResult<Vec<DataFrame>> {
     let total_len = df.height();
     let chunk_size = std::cmp::max(total_len / n, 3);
 
     if df.n_chunks() == n
         && df.get_columns()[0]
             .chunk_lengths()
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/utils/series.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/series.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use crate::prelude::*;
 use crate::series::unstable::UnstableSeries;
+use crate::series::IsSorted;
 
 /// Transform to physical type and coerce floating point and similar sized integer to a bit representation
 /// to reduce compiler bloat
 pub fn _to_physical_and_bit_repr(s: &[Series]) -> Vec<Series> {
     s.iter()
         .map(|s| {
             let physical = s.to_physical_repr();
@@ -25,7 +26,21 @@
     F: Fn(&mut UnstableSeries) -> T,
 {
     let mut container = Series::full_null("", 0, dtype);
     let mut us = UnstableSeries::new(&mut container);
 
     f(&mut us)
 }
+
+pub fn ensure_sorted_arg(s: &Series) {
+    if !matches!(s.is_sorted_flag(), IsSorted::Ascending) {
+        eprintln!(
+            r#"argument is not explicitly sorted
+
+- If your data is ALREADY sorted, set the sorted flag with: '.set_sorted()'.
+- If your data is NOT sorted, sort the 'expr/series/column' first.
+
+This might become an error in a future version.
+    "#
+        );
+    }
+}
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-core/src/utils/supertype.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/src/utils/supertype.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars/Cargo.toml`

 * *Files 10% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 nightly = ["polars-core/nightly", "polars-ops/nightly", "simd"]
 docs = ["polars-core/docs"]
 temporal = ["polars-core/temporal", "polars-lazy/temporal", "polars-io/temporal", "polars-time"]
 random = ["polars-core/random", "polars-lazy/random"]
 default = [
   "docs",
   "zip_with",
-  "csv-file",
+  "csv",
   "temporal",
   "fmt",
   "dtype-slim",
 ]
 ndarray = ["polars-core/ndarray"]
 # serde support for dataframes and series
 serde = ["polars-core/serde"]
 serde-lazy = ["polars-core/serde-lazy", "polars-lazy/serde", "polars-time/serde", "polars-io/serde", "polars-ops/serde"]
-parquet = ["polars-io", "polars-core/parquet", "polars-lazy/parquet", "polars-io/parquet"]
+parquet = ["polars-io", "polars-core/parquet", "polars-lazy/parquet", "polars-io/parquet", "polars-sql/parquet"]
 async = ["polars-lazy/async"]
 aws = ["async", "polars-io/aws"]
 azure = ["async", "polars-io/azure"]
 gcp = ["async", "polars-io/gcp"]
 lazy = ["polars-core/lazy", "polars-lazy", "polars-lazy/compile"]
 # commented out until UB is fixed
 # parallel = ["polars-core/parallel"]
@@ -42,27 +42,27 @@
 # extra utilities for Utf8Chunked
 strings = ["polars-core/strings", "polars-lazy/strings", "polars-ops/strings"]
 
 # support for ObjectChunked<T> (downcastable Series of any type)
 object = ["polars-core/object", "polars-lazy/object"]
 
 # support for arrows json parsing
-json = ["polars-io", "polars-io/json", "polars-lazy/json"]
+json = ["polars-io", "polars-io/json", "polars-lazy/json", "polars-sql/json"]
 
 # support for arrows ipc file parsing
-ipc = ["polars-io", "polars-io/ipc", "polars-lazy/ipc"]
+ipc = ["polars-io", "polars-io/ipc", "polars-lazy/ipc", "polars-sql/ipc"]
 
 # support for arrows streaming ipc file parsing
 ipc_streaming = ["polars-io", "polars-io/ipc_streaming", "polars-lazy/ipc"]
 
 # support for apache avro file parsing
 avro = ["polars-io", "polars-io/avro"]
 
 # support for arrows csv file parsing
-csv-file = ["polars-io", "polars-io/csv-file", "polars-lazy/csv-file"]
+csv = ["polars-io", "polars-io/csv", "polars-lazy/csv", "polars-sql/csv"]
 
 # slower builds
 performant = [
   "polars-core/performant",
   "chunked_ids",
   "dtype-u8",
   "dtype-u16",
@@ -154,28 +154,28 @@
 
 test = [
   "lazy",
   "private",
   "rolling_window",
   "rank",
   "round_series",
-  "csv-file",
+  "csv",
   "dtype-categorical",
   "cum_agg",
   "fmt",
   "diff",
   "abs",
   "parquet",
   "ipc",
   "ipc_streaming",
   "json",
 ]
 
 # don't use this
-private = ["polars-lazy/private", "polars-core/private", "polars-time/private"]
+private = ["polars-lazy/private", "polars-core/private", "polars-time/private", "polars-sql/private"]
 
 # all opt-in datatypes
 dtype-full = [
   "dtype-date",
   "dtype-datetime",
   "dtype-duration",
   "dtype-time",
@@ -234,15 +234,15 @@
   "polars-core/dtype-struct",
   "polars-lazy/dtype-struct",
   "polars-ops/dtype-struct",
   "polars-io/dtype-struct",
 ]
 
 docs-selection = [
-  "csv-file",
+  "csv",
   "json",
   "parquet",
   "ipc",
   "ipc_streaming",
   "dtype-full",
   "is_in",
   "rows",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-time/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/Makefile` & `polars_lts_cpu-0.17.6/local_dependencies/polars/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 		-p polars-time \
 		-p polars-error \
 		-p polars-ops \
 		-p polars-sql
 
 clippy:
 	cargo clippy --all-features \
-	    -p polars-core \
-	    -p polars-io \
-	    -p polars-lazy \
-	    -p polars-arrow \
-	    -p polars-utils \
-	    -p polars-ops \
-	    -p polars-error \
-	    -p polars-row \
-	    -p polars-time \
+		-p polars-core \
+		-p polars-io \
+		-p polars-lazy \
+		-p polars-arrow \
+		-p polars-utils \
+		-p polars-ops \
+		-p polars-error \
+		-p polars-row \
+		-p polars-time \
 		-p polars-sql
 
 clippy-default:
 	cargo clippy
 
 test:  ## Run tests
 	POLARS_NO_STREAMING_GROUPBY=1 POLARS_MAX_THREADS=4 cargo t -p polars-core test_4_threads
@@ -72,15 +72,15 @@
 	    -p polars-core \
 	    -p polars-arrow
 
 pre-commit: fmt clippy clippy-default  ## Run autoformatting and linting
 
 
 check-features:
-	cargo hack check --each-feature --no-dev-deps --features private
+	cargo hack check --each-feature --no-dev-deps --features private 
 
 bench-save:
 	cargo bench --features=random --bench $(BENCH) -- --save-baseline $(SAVE)
 
 bench-cmp:
 	cargo bench --features=random --bench $(BENCH) -- --load-baseline $(FEAT) --baseline $(BASE)
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/eager.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/eager.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/lazy.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/lazy.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/src/docs/performance.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/src/docs/performance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 //!     - `serde` - Support for [serde](https://crates.io/crates/serde) serialization and deserialization.
 //!                 Can be used for JSON and more serde supported serialization formats.
 //!     - `serde-lazy` - Support for [serde](https://crates.io/crates/serde) serialization and deserialization.
 //!                 Can be used for JSON and more serde supported serialization formats.
 //!     - `parquet` - Read Apache Parquet format
 //!     - `json` - JSON serialization
 //!     - `ipc` - Arrow's IPC format serialization
-//!     - `decompress` - Automatically infer compression of csv-files and decompress them.
+//!     - `decompress` - Automatically infer compression of csvs and decompress them.
 //!                      Supported compressions:
 //!                         * zip
 //!                         * gzip
 //!
 //! * `DataFrame` operations:
 //!     - `dynamic_groupby` - Groupby based on a time window instead of predefined keys.
 //!                           Also activates rolling window group by operations.
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/date_like.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/date_like.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/groupby.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/joins.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/list.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use polars::prelude::*;
 
 #[test]
 fn test_to_list_logical() -> PolarsResult<()> {
     let ca = Utf8Chunked::new("a", &["2021-01-01", "2021-01-02", "2021-01-03"]);
     let out = ca.as_date(None, false)?.into_series();
-    let out = out.to_list().unwrap();
+    let out = out.implode().unwrap();
     assert_eq!(out.len(), 1);
     let s = format!("{:?}", out);
     // check if dtype is maintained all the way to formatting
     assert!(s.contains("[2021-01-01, 2021-01-02, 2021-01-03]"));
 
     let expl = out.explode().unwrap();
     assert_eq!(expl.dtype(), &DataType::Date);
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/pivot.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/random.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/random.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/rolling_window.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/rolling_window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/core/series.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/core/series.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/csv.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/csv.rs`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,15 @@
     assert_eq!(df.column("bar").unwrap().dtype(), &DataType::Int64);
     assert_eq!(df.column("foo").unwrap().dtype(), &DataType::Float64);
 }
 
 #[test]
 fn test_empty_bytes_to_dataframe() {
     let fields = vec![Field::new("test_field", DataType::Utf8)];
-    let schema = Schema::from(fields.into_iter());
+    let schema = Schema::from_iter(fields);
     let file = Cursor::new(vec![]);
 
     let result = CsvReader::new(file)
         .has_header(false)
         .with_columns(Some(schema.iter_names().map(|s| s.to_string()).collect()))
         .with_schema(Arc::new(schema))
         .finish();
@@ -388,22 +388,19 @@
 1,2,3
 1,2
 "#;
 
     let file = Cursor::new(csv);
     let df = CsvReader::new(file)
         .has_header(true)
-        .with_schema(Arc::new(Schema::from(
-            vec![
-                Field::new("foo", DataType::UInt32),
-                Field::new("bar", DataType::UInt32),
-                Field::new("ham", DataType::UInt32),
-            ]
-            .into_iter(),
-        )))
+        .with_schema(Arc::new(Schema::from_iter([
+            Field::new("foo", DataType::UInt32),
+            Field::new("bar", DataType::UInt32),
+            Field::new("ham", DataType::UInt32),
+        ])))
         .finish()
         .unwrap();
     assert_eq!(df.column("ham").unwrap().len(), 3)
 }
 
 #[test]
 #[cfg(feature = "temporal")]
@@ -413,21 +410,18 @@
 AUDCAD,1616455919,0.91212,0.95556,1
 AUDCAD,1616455920,0.92212,0.95556,1
 AUDCAD,1616455921,0.96212,0.95666,1
 "#;
     let file = Cursor::new(csv);
     let df = CsvReader::new(file)
         .has_header(true)
-        .with_dtypes(Some(Arc::new(Schema::from(
-            vec![Field::new(
-                "b",
-                DataType::Datetime(TimeUnit::Nanoseconds, None),
-            )]
-            .into_iter(),
-        ))))
+        .with_dtypes(Some(Arc::new(Schema::from_iter([Field::new(
+            "b",
+            DataType::Datetime(TimeUnit::Nanoseconds, None),
+        )]))))
         .finish()?;
 
     assert_eq!(
         df.dtypes(),
         &[
             DataType::Utf8,
             DataType::Datetime(TimeUnit::Nanoseconds, None),
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/ipc_stream.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/ipc_stream.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/json.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/json.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/io/parquet.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/io/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/joins.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/aggregation.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/aggregation.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/cse.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/apply.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/arity.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/arity.rs`

 * *Files 2% similar despite different names*

```diff
@@ -380,32 +380,7 @@
             .into_no_null_iter()
             .collect::<Vec<_>>(),
         &["a", "b", "c", "d"]
     );
 
     Ok(())
 }
-
-#[test]
-fn test_binary_null_prop() -> PolarsResult<()> {
-    let df = df![
-        "a" => [0, 0],
-        "b" => [1, 2]
-    ]?
-    .lazy();
-
-    let expr = col("a").filter(col("a").gt(lit(0)));
-
-    let out = df
-        .groupby([col("b")])
-        .agg([(expr.clone() - expr.mean()).alias("a_mean")])
-        .sort("b", Default::default())
-        .collect()?;
-
-    let a_mean: [Option<f64>; 2] = [None, None];
-    assert!(out.frame_equal_missing(&df![
-        "b" => [1, 2],
-        "a_mean" => a_mean,
-    ]?));
-
-    Ok(())
-}
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/expand.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/expand.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/filter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/expressions/window.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/folds.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/folds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/groupby.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/predicate_queries.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/projection_queries.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars/tests/it/lazy/queries.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars/tests/it/lazy/queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 [dependencies]
 ahash= "0.8"
 bitflags= "1.3"
 glob = "0.3"
 once_cell = "1"
 polars-arrow = { version = "0.28.0", path = "../polars-arrow" }
 polars-core = { version = "0.28.0", path = "../polars-core", features = ["lazy", "private", "zip_with", "random"], default-features = false }
-polars-io = { version = "0.28.0", path = "../polars-io", features = ["lazy", "csv-file", "private"], default-features = false }
+polars-io = { version = "0.28.0", path = "../polars-io", features = ["lazy", "csv", "private"], default-features = false }
 polars-ops = { version = "0.28.0", path = "../polars-ops", default-features = false }
 polars-pipe = { version = "0.28.0", path = "../polars-pipe", optional = true }
 polars-plan = { version = "0.28.0", path = "../polars-plan" }
 polars-time = { version = "0.28.0", path = "../polars-time", optional = true }
 polars-utils = { version = "0.28.0", path = "../polars-utils" }
 pyo3 = { version = "0.18", optional = true }
 rayon= "1.6"
@@ -39,15 +39,15 @@
   "polars-plan/async",
   "polars-io/cloud",
   "polars-pipe/async",
   "streaming",
 ]
 ipc = ["polars-io/ipc", "polars-plan/ipc", "polars-pipe/ipc"]
 json = ["polars-io/json", "polars-plan/json"]
-csv-file = ["polars-io/csv-file", "polars-plan/csv-file", "polars-pipe/csv-file"]
+csv = ["polars-io/csv", "polars-plan/csv", "polars-pipe/csv"]
 temporal = ["dtype-datetime", "dtype-date", "dtype-time", "dtype-duration", "polars-plan/temporal"]
 # debugging purposes
 fmt = ["polars-core/fmt", "polars-plan/fmt"]
 strings = ["polars-plan/strings"]
 future = []
 dtype-u8 = ["polars-plan/dtype-u8", "polars-pipe/dtype-u8"]
 dtype-u16 = ["polars-plan/dtype-u16", "polars-pipe/dtype-u16"]
@@ -141,15 +141,15 @@
 test = [
   "polars-plan/debugging",
   "panic_on_schema",
   "private",
   "rolling_window",
   "rank",
   "round_series",
-  "csv-file",
+  "csv",
   "dtype-categorical",
   "cum_agg",
   "regex",
   "polars-core/fmt",
   "diff",
   "abs",
   "parquet",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dot.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/eval.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/functions.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/list.rs`

 * *Files 2% similar despite different names*

```diff
@@ -93,24 +93,24 @@
                             None
                         }
                     }
                 })
             })
             .collect_trusted()
     };
+    if let Some(err) = err {
+        return Err(err);
+    }
 
     ca.rename(s.name());
 
     if ca.dtype() != output_field.data_type() {
         ca.cast(output_field.data_type()).map(Some)
     } else {
-        match err {
-            None => Ok(Some(ca.into_series())),
-            Some(e) => Err(e),
-        }
+        Ok(Some(ca.into_series()))
     }
 }
 
 fn run_on_groupby_engine(
     name: &str,
     lst: &ListChunked,
     expr: &Expr,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/dsl/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/csv.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/csv.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 use polars_io::csv::{CsvEncoding, NullValues};
 use polars_io::RowCount;
 
 use crate::frame::LazyFileListReader;
 use crate::prelude::*;
 
 #[derive(Clone)]
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 pub struct LazyCsvReader<'a> {
     path: PathBuf,
     delimiter: u8,
     has_header: bool,
     ignore_errors: bool,
     skip_rows: usize,
     n_rows: Option<usize>,
@@ -30,15 +30,15 @@
     rechunk: bool,
     skip_rows_after_header: usize,
     encoding: CsvEncoding,
     row_count: Option<RowCount>,
     try_parse_dates: bool,
 }
 
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 impl<'a> LazyCsvReader<'a> {
     pub fn new(path: impl AsRef<Path>) -> Self {
         LazyCsvReader {
             path: path.as_ref().to_owned(),
             delimiter: b',',
             has_header: true,
             ignore_errors: false,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/file_list_reader.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/file_list_reader.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/ipc.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 //! Lazy variant of a [DataFrame](polars_core::frame::DataFrame).
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 mod csv;
 #[cfg(feature = "ipc")]
 mod ipc;
 #[cfg(feature = "json")]
 mod ndjson;
 #[cfg(feature = "parquet")]
 mod parquet;
@@ -17,15 +17,15 @@
 
 use std::borrow::Cow;
 #[cfg(any(feature = "parquet", feature = "ipc"))]
 use std::path::PathBuf;
 use std::sync::Arc;
 
 pub use anonymous_scan::*;
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 pub use csv::*;
 pub use file_list_reader::*;
 #[cfg(feature = "ipc")]
 pub use ipc::*;
 #[cfg(feature = "json")]
 pub use ndjson::*;
 #[cfg(feature = "parquet")]
@@ -33,15 +33,15 @@
 use polars_arrow::prelude::QuantileInterpolOptions;
 use polars_core::frame::explode::MeltArgs;
 use polars_core::frame::hash_join::JoinType;
 use polars_core::prelude::*;
 use polars_io::RowCount;
 pub use polars_plan::frame::{AllowedOptimizations, OptState};
 use polars_plan::global::FETCH_ROWS;
-#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
 use polars_plan::logical_plan::collect_fingerprints;
 use polars_plan::logical_plan::optimize;
 use polars_plan::utils::expr_to_leaf_column_names;
 use smartstring::alias::String as SmartString;
 
 use crate::physical_plan::executors::Executor;
 use crate::physical_plan::planner::create_physical_plan;
@@ -489,21 +489,21 @@
         let mut expr_arena = Arena::with_capacity(256);
         let mut lp_arena = Arena::with_capacity(128);
         let mut scratch = vec![];
         let lp_top =
             self.optimize_with_scratch(&mut lp_arena, &mut expr_arena, &mut scratch, false)?;
 
         let finger_prints = if file_caching {
-            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
             {
                 let mut fps = Vec::with_capacity(8);
                 collect_fingerprints(lp_top, &mut fps, &lp_arena, &expr_arena);
                 Some(fps)
             }
-            #[cfg(not(any(feature = "ipc", feature = "parquet", feature = "csv-file")))]
+            #[cfg(not(any(feature = "ipc", feature = "parquet", feature = "csv")))]
             {
                 None
             }
         } else {
             None
         };
 
@@ -536,15 +536,15 @@
     /// }
     /// ```
     pub fn collect(self) -> PolarsResult<DataFrame> {
         let (mut state, mut physical_plan, _) = self.prepare_collect(false)?;
         let out = physical_plan.execute(&mut state);
         #[cfg(debug_assertions)]
         {
-            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
             state.file_cache.assert_empty();
         }
         out
     }
 
     /// Profile a LazyFrame.
     ///
@@ -1134,15 +1134,15 @@
     ///
     /// # Warning
     /// This can have a negative effect on query performance.
     /// This may for instance block predicate pushdown optimization.
     pub fn with_row_count(mut self, name: &str, offset: Option<IdxSize>) -> LazyFrame {
         let add_row_count_in_map = match &mut self.logical_plan {
             // Do the row count at scan
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             LogicalPlan::CsvScan { options, .. } => {
                 options.row_count = Some(RowCount {
                     name: name.to_string(),
                     offset: offset.unwrap_or(0),
                 });
                 false
             }
@@ -1163,15 +1163,18 @@
                 false
             }
             _ => true,
         };
 
         let name2: SmartString = name.into();
         let udf_schema = move |s: &Schema| {
-            let new = s.insert_index(0, name2.clone(), IDX_DTYPE).unwrap();
+            // Can't error, index 0 is always in bounds
+            let new = s
+                .new_inserting_at_index(0, name2.clone(), IDX_DTYPE)
+                .unwrap();
             Ok(Arc::new(new))
         };
 
         let name = name.to_owned();
 
         // if we do the row count at scan we add a dummy map, to update the schema
         let opt = if add_row_count_in_map {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/ndjson.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/ndjson.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/parquet.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/frame/pivot.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/frame/pivot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/cache.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/executor.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/ext_context.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_dynamic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_partitioned.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/groupby_rolling.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/python_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ipc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/mod.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,29 @@
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 mod csv;
 #[cfg(feature = "ipc")]
 mod ipc;
 #[cfg(feature = "json")]
 mod ndjson;
 #[cfg(feature = "parquet")]
 mod parquet;
 
 use std::mem;
 
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 pub(crate) use csv::CsvExec;
 #[cfg(feature = "ipc")]
 pub(crate) use ipc::IpcExec;
 #[cfg(feature = "parquet")]
 pub(crate) use parquet::ParquetExec;
 #[cfg(any(feature = "ipc", feature = "parquet"))]
 use polars_io::predicates::PhysicalIoExpr;
 use polars_io::prelude::*;
 use polars_plan::global::_set_n_rows_for_scan;
-#[cfg(any(
-    feature = "parquet",
-    feature = "csv-file",
-    feature = "ipc",
-    feature = "cse"
-))]
+#[cfg(any(feature = "parquet", feature = "csv", feature = "ipc", feature = "cse"))]
 use polars_plan::logical_plan::FileFingerPrint;
 
 use super::*;
 use crate::prelude::*;
 
 #[cfg(any(feature = "ipc", feature = "parquet"))]
 type Projection = Option<Vec<usize>>;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/ndjson.rs`

 * *Files 11% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
     fn schema(&self, infer_schema_length: Option<usize>) -> PolarsResult<Schema> {
         let f = std::fs::File::open(&self.path)?;
         let mut reader = std::io::BufReader::new(f);
 
         let data_type =
             arrow_ndjson::read::infer(&mut reader, infer_schema_length).map_err(to_compute_err)?;
-        let schema: Schema = StructArray::get_fields(&data_type).iter().into();
+        let schema = Schema::from_iter(StructArray::get_fields(&data_type));
 
         Ok(schema)
     }
     fn allows_projection_pushdown(&self) -> bool {
         true
     }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/scan/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/stack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/udf.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/executors/unique.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/exotic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/exotic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/aggregation.rs`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
                     agg_s
                 }
                 GroupByMethod::NUnique => {
                     check_null_prop!();
                     let agg_s = ac.flat_naive().into_owned().agg_n_unique(ac.groups());
                     rename_series(agg_s, &keep_name)
                 }
-                GroupByMethod::List => {
+                GroupByMethod::Implode => {
                     if state.unset_finalize_window_as_list() {
                         let agg = ac.aggregated();
                         rename_series(agg, &keep_name)
                     } else {
                         // if the aggregation is already
                         // in an aggregate flat state for instance by
                         // a mean aggregation, we simply convert to list
@@ -311,15 +311,15 @@
                         let mut count_s = series.agg_valid_count(groups);
                         count_s.rename("__POLARS_COUNT");
                         Ok(StructChunked::new(&new_name, &[agg_s, count_s])
                             .unwrap()
                             .into_series())
                     }
                 }
-                GroupByMethod::List => {
+                GroupByMethod::Implode => {
                     let new_name = series.name();
                     let mut agg = series.agg_list(groups);
                     agg.rename(new_name);
                     Ok(agg)
                 }
                 GroupByMethod::First => {
                     let mut agg = series.agg_first(groups);
@@ -386,15 +386,15 @@
                     _ => Ok(Series::full_null(
                         new_name,
                         groups.len(),
                         partitioned.dtype(),
                     )),
                 }
             }
-            GroupByMethod::List => {
+            GroupByMethod::Implode => {
                 // the groups are scattered over multiple groups/sub dataframes.
                 // we now must collect them into a single group
                 let ca = partitioned.list().unwrap();
                 let new_name = partitioned.name().to_string();
 
                 let mut values = Vec::with_capacity(groups.len());
                 let mut can_fast_explode = true;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/alias.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/binary.rs`

 * *Files 6% similar despite different names*

```diff
@@ -87,57 +87,20 @@
         Operator::Or => left.bitor(right),
         Operator::Xor => left.bitxor(right),
         Operator::Modulus => Ok(left % right),
     }
 }
 
 impl BinaryExpr {
-    fn null_propagate(&self, ac_l: &mut AggregationContext, ac_r: &AggregationContext) -> bool {
-        // this null prop can exist due to:
-        // assuming 2 rows
-        //
-        // expr = col().filter(false)
-        //
-        // this would null propagate
-        // (expr - expr.mean()) -> [None, None]
-        //
-        // but adding another aggregation is valid:
-        // (expr - expr.mean()).mean()
-        match ac_l.agg_state() {
-            AggState::AggregatedFlat(s) if s.null_count() == s.len() => {
-                let s = s.clone();
-                ac_l.with_update_groups(UpdateGroups::No);
-                ac_l.with_series(s, true, Some(&self.expr)).unwrap();
-                ac_l.null_propagated = true;
-                return true;
-            }
-            _ => {}
-        }
-        match ac_r.agg_state() {
-            AggState::AggregatedFlat(s) if s.null_count() == s.len() => {
-                ac_l.with_update_groups(UpdateGroups::No);
-                ac_l.with_series(s.clone(), true, Some(&self.expr)).unwrap();
-                ac_l.null_propagated = true;
-                return true;
-            }
-            _ => {}
-        }
-        false
-    }
-
     fn apply_elementwise<'a>(
         &self,
         mut ac_l: AggregationContext<'a>,
         ac_r: AggregationContext,
         aggregated: bool,
     ) -> PolarsResult<AggregationContext<'a>> {
-        if self.null_propagate(&mut ac_l, &ac_r) {
-            return Ok(ac_l);
-        }
-
         // we want to be able to mutate in place
         // so we take the lhs to make sure that we drop
         let lhs = ac_l.series().clone();
         let rhs = ac_r.series().clone();
 
         // drop lhs so that we might operate in place
         {
@@ -151,18 +114,14 @@
     }
 
     fn apply_group_aware<'a>(
         &self,
         mut ac_l: AggregationContext<'a>,
         mut ac_r: AggregationContext<'a>,
     ) -> PolarsResult<AggregationContext<'a>> {
-        if self.null_propagate(&mut ac_l, &ac_r) {
-            return Ok(ac_l);
-        }
-
         let name = ac_l.series().name().to_string();
         let mut ca: ListChunked = ac_l
             .iter_groups(false)
             .zip(ac_r.iter_groups(false))
             .map(|(l, r)| {
                 match (l, r) {
                     (Some(l), Some(r)) => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/cast.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/column.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/group_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/literal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sort.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/sortby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/take.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/ternary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/expressions/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/file_cache.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::sync::Mutex;
 
 use polars_core::prelude::*;
-#[cfg(any(feature = "parquet", feature = "csv-file", feature = "ipc"))]
+#[cfg(any(feature = "parquet", feature = "csv", feature = "ipc"))]
 use polars_plan::logical_plan::FileFingerPrint;
 
 use crate::prelude::*;
 
 #[derive(Clone)]
 pub(crate) struct FileCache {
     // (path, predicate) -> (read_count, df)
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/node_timer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/expr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -399,21 +399,22 @@
                             )))
                         }
                     }
                 }
                 AAggExpr::Implode(expr) => {
                     let input = create_physical_expr(expr, ctxt, expr_arena, schema)?;
                     match ctxt {
-                        Context::Aggregation => {
-                            Ok(Arc::new(AggregationExpr::new(input, GroupByMethod::List)))
-                        }
+                        Context::Aggregation => Ok(Arc::new(AggregationExpr::new(
+                            input,
+                            GroupByMethod::Implode,
+                        ))),
                         Context::Default => {
                             let function = SpecialEq::new(Arc::new(move |s: &mut [Series]| {
                                 let s = &s[0];
-                                s.to_list().map(|ca| Some(ca.into_series()))
+                                s.implode().map(|ca| Some(ca.into_series()))
                             })
                                 as Arc<dyn SeriesUdf>);
                             Ok(Arc::new(ApplyExpr::new_minimal(
                                 vec![input],
                                 function,
                                 node_to_expr(expression, expr_arena),
                                 ApplyOptions::ApplyFlat,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/planner/lp.rs`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
             Ok(Box::new(executors::SliceExec { input, offset, len }))
         }
         Selection { input, predicate } => {
             let input = create_physical_plan(input, lp_arena, expr_arena)?;
             let predicate = create_physical_expr(predicate, Context::Default, expr_arena, None)?;
             Ok(Box::new(executors::FilterExec::new(predicate, input)))
         }
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         CsvScan {
             path,
             file_info,
             output_schema,
             options,
             predicate,
         } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/state.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/state.rs`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 
 use bitflags::bitflags;
 use once_cell::sync::OnceCell;
 use polars_core::config::verbose;
 use polars_core::frame::groupby::GroupsProxy;
 use polars_core::frame::hash_join::JoinOptIds;
 use polars_core::prelude::*;
-#[cfg(any(feature = "parquet", feature = "csv-file", feature = "ipc"))]
+#[cfg(any(feature = "parquet", feature = "csv", feature = "ipc"))]
 use polars_plan::logical_plan::FileFingerPrint;
 
-#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
 use super::file_cache::FileCache;
 use crate::physical_plan::node_timer::NodeTimer;
 
 pub type JoinTuplesCache = Arc<Mutex<PlHashMap<String, JoinOptIds>>>;
 pub type GroupsProxyCache = Arc<Mutex<PlHashMap<String, GroupsProxy>>>;
 
 bitflags! {
@@ -62,15 +62,15 @@
 }
 
 /// State/ cache that is maintained during the Execution of the physical plan.
 pub struct ExecutionState {
     // cached by a `.cache` call and kept in memory for the duration of the plan.
     df_cache: Arc<Mutex<PlHashMap<usize, Arc<OnceCell<DataFrame>>>>>,
     // cache file reads until all branches got there file, then we delete it
-    #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+    #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
     pub(crate) file_cache: FileCache,
     pub(super) schema_cache: RwLock<Option<SchemaRef>>,
     /// Used by Window Expression to prevent redundant grouping
     pub(super) group_tuples: GroupsProxyCache,
     /// Used by Window Expression to prevent redundant joins
     pub(super) join_tuples: JoinTuplesCache,
     // every join/union split gets an increment to distinguish between schema state
@@ -107,15 +107,15 @@
         }
     }
 
     /// Partially clones and partially clears state
     pub(super) fn split(&self) -> Self {
         Self {
             df_cache: self.df_cache.clone(),
-            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
             file_cache: self.file_cache.clone(),
             schema_cache: Default::default(),
             group_tuples: Default::default(),
             join_tuples: Default::default(),
             branch_idx: self.branch_idx,
             flags: AtomicU8::new(self.flags.load(Ordering::Relaxed)),
             ext_contexts: self.ext_contexts.clone(),
@@ -123,36 +123,36 @@
         }
     }
 
     /// clones and partially clears state
     pub(super) fn clone(&self) -> Self {
         Self {
             df_cache: self.df_cache.clone(),
-            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
             file_cache: self.file_cache.clone(),
             schema_cache: self.schema_cache.read().unwrap().clone().into(),
             group_tuples: self.group_tuples.clone(),
             join_tuples: self.join_tuples.clone(),
             branch_idx: self.branch_idx,
             flags: AtomicU8::new(self.flags.load(Ordering::Relaxed)),
             ext_contexts: self.ext_contexts.clone(),
             node_timer: self.node_timer.clone(),
         }
     }
 
-    #[cfg(not(any(feature = "parquet", feature = "csv-file", feature = "ipc")))]
+    #[cfg(not(any(feature = "parquet", feature = "csv", feature = "ipc")))]
     pub(crate) fn with_finger_prints(_finger_prints: Option<usize>) -> Self {
         Self::new()
     }
-    #[cfg(any(feature = "parquet", feature = "csv-file", feature = "ipc"))]
+    #[cfg(any(feature = "parquet", feature = "csv", feature = "ipc"))]
     pub(crate) fn with_finger_prints(finger_prints: Option<Vec<FileFingerPrint>>) -> Self {
         Self {
             df_cache: Arc::new(Mutex::new(PlHashMap::default())),
             schema_cache: Default::default(),
-            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
             file_cache: FileCache::new(finger_prints),
             group_tuples: Arc::new(Mutex::new(PlHashMap::default())),
             join_tuples: Arc::new(Mutex::new(PlHashMap::default())),
             branch_idx: 0,
             flags: AtomicU8::new(StateFlags::init().as_u8()),
             ext_contexts: Default::default(),
             node_timer: None,
@@ -163,15 +163,15 @@
         let mut flags: StateFlags = Default::default();
         if verbose() {
             flags |= StateFlags::VERBOSE;
         }
         Self {
             df_cache: Default::default(),
             schema_cache: Default::default(),
-            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+            #[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
             file_cache: FileCache::new(None),
             group_tuples: Default::default(),
             join_tuples: Default::default(),
             branch_idx: 0,
             flags: AtomicU8::new(StateFlags::init().as_u8()),
             ext_contexts: Default::default(),
             node_timer: None,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/convert.rs`

 * *Files 1% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                         &mut stack,
                         scratch,
                         &mut pipeline_trees,
                         lp,
                     )
                 }
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { .. } => {
                 if state.streamable {
                     state.sources.push(root);
                     pipeline_trees[current_idx].push(state)
                 }
             }
             #[cfg(feature = "parquet")]
@@ -300,15 +300,15 @@
                 };
                 state_left
                     .operators_sinks
                     .push((IS_SINK, !IS_RHS_JOIN, root));
                 stack.push((input_left, state_left, current_idx));
             }
             // add globbing patterns
-            #[cfg(all(feature = "csv-file", feature = "parquet"))]
+            #[cfg(all(feature = "csv", feature = "parquet"))]
             Union { inputs, .. } => {
                 if state.streamable
                     && inputs.iter().all(|node| match lp_arena.get(*node) {
                         ParquetScan { .. } => true,
                         CsvScan { .. } => true,
                         MapFunction {
                             input,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/physical_plan/streaming/tree.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/prelude.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/aggregations.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/aggregations.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/arity.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/arity.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/cse.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/cse.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/io.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/io.rs`

 * *Files 2% similar despite different names*

```diff
@@ -282,15 +282,15 @@
         assert_eq!(out.shape(), (1, 3));
     }
 
     Ok(())
 }
 
 #[test]
-#[cfg(all(feature = "ipc", feature = "csv-file"))]
+#[cfg(all(feature = "ipc", feature = "csv"))]
 fn test_slice_filter() -> PolarsResult<()> {
     init_files();
     let _guard = SINGLE_LOCK.lock().unwrap();
 
     // make sure that the slices are not applied before the predicates.
     let len = 5;
     let offset = 3;
@@ -434,17 +434,18 @@
         DataType::UInt8,
         DataType::Int16,
         DataType::UInt16,
     ];
     for dt in small_dt {
         let df = LazyCsvReader::new(FOODS_CSV)
             .has_header(true)
-            .with_dtype_overwrite(Some(&Schema::from(
-                vec![Field::new("sugars_g", dt.clone())].into_iter(),
-            )))
+            .with_dtype_overwrite(Some(&Schema::from_iter([Field::new(
+                "sugars_g",
+                dt.clone(),
+            )])))
             .finish()?
             .select(&[col("sugars_g")])
             .collect()?;
 
         assert_eq!(df.dtypes(), &[dt]);
     }
     Ok(())
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/logical.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/logical.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/mod.rs`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 static GLOB_PARQUET: &str = "../../examples/datasets/*.parquet";
 static GLOB_CSV: &str = "../../examples/datasets/*.csv";
 static GLOB_IPC: &str = "../../examples/datasets/*.ipc";
 static FOODS_CSV: &str = "../../examples/datasets/foods1.csv";
 static FOODS_IPC: &str = "../../examples/datasets/foods1.ipc";
 static FOODS_PARQUET: &str = "../../examples/datasets/foods1.parquet";
 
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 fn scan_foods_csv() -> LazyFrame {
     LazyCsvReader::new(FOODS_CSV).finish().unwrap()
 }
 
 #[cfg(feature = "ipc")]
 fn scan_foods_ipc() -> LazyFrame {
     init_files();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/optimization_checks.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/optimization_checks.rs`

 * *Files 1% similar despite different names*

```diff
@@ -502,15 +502,15 @@
             }
             | DataFrameScan { .. } => true,
             _ => false,
         }
     }));
     assert_eq!(
         q.schema().unwrap().as_ref(),
-        &Schema::from([Field::new("c1", DataType::Int32)].into_iter())
+        &Schema::from_iter([Field::new("c1", DataType::Int32)])
     );
     Ok(())
 }
 
 #[test]
 fn test_slice_at_scan_groupby() -> PolarsResult<()> {
     let ldf = scan_foods_csv();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/predicate_queries.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/predicate_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/projection_queries.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/projection_queries.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/queries.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/queries.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1411,15 +1411,15 @@
 
     let schema = df
         .lazy()
         .select([when(col("A").gt(lit(1)))
             .then(Null {}.lit())
             .otherwise(col("A"))])
         .schema();
-    assert_ne!(schema?.get_index(0).unwrap().1, &DataType::Null);
+    assert_ne!(schema?.get_at_index(0).unwrap().1, &DataType::Null);
 
     Ok(())
 }
 
 #[test]
 fn test_singleton_broadcast() -> PolarsResult<()> {
     let df = fruits_cars();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/streaming.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/streaming.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/tests/tpch.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/tests/tpch.rs`

 * *Files 2% similar despite different names*

```diff
@@ -81,24 +81,21 @@
             [true, false, false, false],
             false,
         )
         .limit(100)
         .with_common_subplan_elimination(true);
 
     let out = q.collect()?;
-    let schema = Schema::from(
-        [
-            Field::new("s_acctbal", DataType::Float64),
-            Field::new("s_name", DataType::Utf8),
-            Field::new("n_name", DataType::Utf8),
-            Field::new("p_partkey", DataType::Int64),
-            Field::new("p_mfgr", DataType::Utf8),
-            Field::new("s_address", DataType::Utf8),
-            Field::new("s_phone", DataType::Utf8),
-            Field::new("s_comment", DataType::Utf8),
-        ]
-        .into_iter(),
-    );
+    let schema = Schema::from_iter([
+        Field::new("s_acctbal", DataType::Float64),
+        Field::new("s_name", DataType::Utf8),
+        Field::new("n_name", DataType::Utf8),
+        Field::new("p_partkey", DataType::Int64),
+        Field::new("p_mfgr", DataType::Utf8),
+        Field::new("s_address", DataType::Utf8),
+        Field::new("s_phone", DataType::Utf8),
+        Field::new("s_comment", DataType::Utf8),
+    ]);
     assert_eq!(&out.schema(), &schema);
 
     Ok(())
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-lazy/src/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     root_lp: Node,
     paths: &mut PlHashSet<PathBuf>,
     lp_arena: &Arena<ALogicalPlan>,
 ) {
     lp_arena.iter(root_lp).for_each(|(_, lp)| {
         use ALogicalPlan::*;
         match lp {
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { path, .. } => {
                 paths.insert(path.clone());
             }
             #[cfg(feature = "parquet")]
             ParquetScan { path, .. } => {
                 paths.insert(path.clone());
             }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # support for arrows ipc file parsing
 ipc = ["arrow/io_ipc", "arrow/io_ipc_compression", "memmap"]
 # support for arrows streaming ipc file parsing
 ipc_streaming = ["arrow/io_ipc", "arrow/io_ipc_compression"]
 # support for arrow avro parsing
 avro = ["arrow/io_avro", "arrow/io_avro_compression"]
 # ipc = []
-csv-file = ["memmap", "lexical", "polars-core/rows", "lexical-core", "fast-float", "simdutf8"]
+csv = ["memmap", "lexical", "polars-core/rows", "lexical-core", "fast-float", "simdutf8"]
 decompress = ["flate2/miniz_oxide"]
 decompress-fast = ["flate2/zlib-ng"]
 dtype-categorical = ["polars-core/dtype-categorical"]
 dtype-date = ["polars-core/dtype-date", "polars-time/dtype-date"]
 dtype-datetime = [
   "polars-core/dtype-datetime",
   "polars-core/temporal",
@@ -79,19 +79,19 @@
 simd-json = { version = "0.7.0", optional = true, features = ["allow-non-simd", "known-key"] }
 simdutf8 = { version = "0.1", optional = true }
 tokio = { version = "1.26.0", features = ["net"], optional = true }
 url = { version = "2.3.1", optional = true }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/avro/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/avro/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/avro/read.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/avro/read.rs`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     projection: Option<Vec<usize>>,
 }
 
 impl<R: Read + Seek> AvroReader<R> {
     /// Get schema of the Avro File
     pub fn schema(&mut self) -> PolarsResult<Schema> {
         let schema = self.arrow_schema()?;
-        Ok((schema.fields.iter()).into())
+        Ok(Schema::from_iter(&schema.fields))
     }
 
     /// Get arrow schema of the avro File, this is faster than a polars schema.
     pub fn arrow_schema(&mut self) -> PolarsResult<ArrowSchema> {
         let metadata =
             avro::avro_schema::read::read_metadata(&mut self.reader).map_err(to_compute_err)?;
         let schema = read::infer_schema(&metadata.record)?;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/avro/write.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/avro/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/cloud/adaptors.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/cloud/adaptors.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/cloud/glob.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/cloud/glob.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/cloud/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/cloud/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/buffer.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/buffer.rs`

 * *Files 0% similar despite different names*

```diff
@@ -509,15 +509,15 @@
 ) -> PolarsResult<Vec<Buffer<'a>>> {
     // we keep track of the string columns we have seen so that we can increment the index
     let mut str_index = 0;
 
     projection
         .iter()
         .map(|&i| {
-            let (name, dtype) = schema.get_index(i).unwrap();
+            let (name, dtype) = schema.get_at_index(i).unwrap();
             let mut str_capacity = 0;
             // determine the needed capacity for this column
             if dtype == &DataType::Utf8 {
                 str_capacity = str_capacities[str_index].size_hint();
                 str_index += 1;
             }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/parser.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/parser.rs`

 * *Files 0% similar despite different names*

```diff
@@ -463,15 +463,15 @@
                         if add_null {
                             buf.add_null(!missing_is_null && field.is_empty())
                         } else {
                             buf.add(field, ignore_errors, needs_escaping, missing_is_null)
                                 .map_err(|_| {
                                     let bytes_offset = offset + field.as_ptr() as usize - start;
                                     let unparsable = String::from_utf8_lossy(field);
-                                    let column_name = schema.get_index(idx as usize).unwrap().0;
+                                    let column_name = schema.get_at_index(idx as usize).unwrap().0;
                                     polars_err!(
                                         ComputeError:
                                         "Could not parse `{}` as dtype `{}` at column '{}' (column number {}).\n\
                                         The current offset in the file is {} bytes.\n\
                                         \n\
                                         You might want to try:\n\
                                         - increasing `infer_schema_length` (e.g. `infer_schema_length=10000`),\n\
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read.rs`

 * *Files 2% similar despite different names*

```diff
@@ -373,38 +373,40 @@
     fn prepare_schema_overwrite(&self, overwriting_schema: &Schema) -> (Schema, Vec<Field>, bool) {
         // This branch we check if there are dtypes we cannot parse.
         // We only support a few dtypes in the parser and later cast to the required dtype
         let mut to_cast = Vec::with_capacity(overwriting_schema.len());
 
         let mut _has_categorical = false;
 
-        #[allow(clippy::unnecessary_filter_map)]
-        let fields = overwriting_schema.iter_fields().filter_map(|mut fld| {
-            use DataType::*;
-            match fld.data_type() {
-                Time => {
-                    to_cast.push(fld);
-                    // let inference decide the column type
-                    None
+        let schema = overwriting_schema
+            .iter_fields()
+            .filter_map(|mut fld| {
+                use DataType::*;
+                match fld.data_type() {
+                    Time => {
+                        to_cast.push(fld);
+                        // let inference decide the column type
+                        None
+                    }
+                    Int8 | Int16 | UInt8 | UInt16 => {
+                        // We have not compiled these buffers, so we cast them later.
+                        to_cast.push(fld.clone());
+                        fld.coerce(DataType::Int32);
+                        Some(fld)
+                    }
+                    #[cfg(feature = "dtype-categorical")]
+                    Categorical(_) => {
+                        _has_categorical = true;
+                        Some(fld)
+                    }
+                    _ => Some(fld),
                 }
-                Int8 | Int16 | UInt8 | UInt16 => {
-                    // We have not compiled these buffers, so we cast them later.
-                    to_cast.push(fld.clone());
-                    fld.coerce(DataType::Int32);
-                    Some(fld)
-                }
-                #[cfg(feature = "dtype-categorical")]
-                Categorical(_) => {
-                    _has_categorical = true;
-                    Some(fld)
-                }
-                _ => Some(fld),
-            }
-        });
-        let schema = Schema::from(fields);
+            })
+            .collect::<Schema>();
+
         (schema, to_cast, _has_categorical)
     }
 
     pub fn batched_borrowed_mmap(&'a mut self) -> PolarsResult<BatchedCsvReaderMmap<'a>> {
         if let Some(schema) = self.schema_overwrite.as_deref() {
             let (schema, to_cast, has_cat) = self.prepare_schema_overwrite(schema);
             let schema = Arc::new(schema);
@@ -579,20 +581,21 @@
         #[cfg(feature = "temporal")]
         // only needed until we also can parse time columns in place
         if self.try_parse_dates {
             // determine the schema that's given by the user. That should not be changed
             let fixed_schema = match (schema_overwrite, self.dtype_overwrite) {
                 (Some(schema), _) => schema,
                 (None, Some(dtypes)) => {
-                    let fields = dtypes
+                    let schema = dtypes
                         .iter()
                         .zip(df.get_column_names())
-                        .map(|(dtype, name)| Field::new(name, dtype.clone()));
+                        .map(|(dtype, name)| Field::new(name, dtype.clone()))
+                        .collect::<Schema>();
 
-                    Arc::new(Schema::from(fields))
+                    Arc::new(schema)
                 }
                 _ => Arc::default(),
             };
             df = parse_dates(df, &fixed_schema)
         }
         Ok(df)
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read_impl/batched_read.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/read_impl/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/read_impl/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
                     Arc::new(inferred_schema)
                 }
             }
         };
         if let Some(dtypes) = dtype_overwrite {
             let s = Arc::make_mut(&mut schema);
             for (index, dt) in dtypes.iter().enumerate() {
-                s.coerce_by_index(index, dt.clone()).unwrap();
+                s.set_dtype_at_index(index, dt.clone()).unwrap();
             }
         }
 
         // create a null value for every column
         let mut null_values = null_values.map(|nv| nv.compile(&schema)).transpose()?;
 
         if let Some(cols) = columns {
@@ -481,15 +481,15 @@
         // Per string column we keep a statistic of the maximum length of string bytes per chunk
         // We must the names, not the indexes, (the indexes are incorrect due to projection
         // pushdown)
 
         let mut new_projection = Vec::with_capacity(projection.len());
 
         for i in projection {
-            let (_, dtype) = self.schema.get_index(*i).ok_or_else(|| {
+            let (_, dtype) = self.schema.get_at_index(*i).ok_or_else(|| {
                 polars_err!(
                     ComputeError:
                     "projection index {} is out of bounds for CSV schema with {} columns",
                     i, self.schema.len(),
                 )
             })?;
 
@@ -875,12 +875,12 @@
     /// of fields in the `schema`.
     fn new(schema: SchemaRef, fields: Vec<usize>) -> Self {
         Self { schema, fields }
     }
 
     fn iter(&self) -> impl Iterator<Item = &str> {
         self.fields.iter().map(|schema_i| {
-            let (name, _) = self.schema.get_index(*schema_i).unwrap();
+            let (name, _) = self.schema.get_at_index(*schema_i).unwrap();
             name.as_str()
         })
     }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/splitfields.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/splitfields.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -435,15 +435,15 @@
                 fields.push(Field::new(name, dtype.clone()));
                 continue;
             }
 
             // column might have been renamed
             // execute only if schema is complete
             if schema_overwrite.len() == header_length {
-                if let Some((name, dtype)) = schema_overwrite.get_index(i) {
+                if let Some((name, dtype)) = schema_overwrite.get_at_index(i) {
                     fields.push(Field::new(name, dtype.clone()));
                     continue;
                 }
             }
         }
 
         // determine data type based on possible types
@@ -502,19 +502,15 @@
             quote_char,
             eol_char,
             null_values,
             try_parse_dates,
         );
     }
 
-    Ok((
-        Schema::from(fields.into_iter()),
-        rows_count,
-        end_ptr - start_ptr,
-    ))
+    Ok((Schema::from_iter(fields), rows_count, end_ptr - start_ptr))
 }
 
 // magic numbers
 const GZIP: [u8; 2] = [31, 139];
 const ZLIB0: [u8; 2] = [0x78, 0x01];
 const ZLIB1: [u8; 2] = [0x78, 0x9C];
 const ZLIB2: [u8; 2] = [0x78, 0xDA];
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/write.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/csv/write_impl.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/csv/write_impl.rs`

 * *Files 2% similar despite different names*

```diff
@@ -325,24 +325,35 @@
             let _ = writer.write(&buf)?;
             buf.clear();
             write_buffer_pool.set(buf);
         }
 
         n_rows_finished += total_rows_per_pool_iter;
     }
-
     Ok(())
 }
+
 /// Writes a CSV header to `writer`
 pub(crate) fn write_header<W: Write>(
     writer: &mut W,
     names: &[&str],
     options: &SerializeOptions,
 ) -> PolarsResult<()> {
+    let mut escaped_names: Vec<String> = Vec::with_capacity(names.len());
+    let mut nm: Vec<u8> = vec![];
+
+    for name in names {
+        fmt_and_escape_str(&mut nm, name, options)?;
+        unsafe {
+            // Safety: we know headers will be valid utf8 at this point
+            escaped_names.push(std::str::from_utf8_unchecked(&nm).to_string());
+        }
+        nm.clear();
+    }
     writer.write_all(
-        names
+        escaped_names
             .join(std::str::from_utf8(&[options.delimiter]).unwrap())
             .as_bytes(),
     )?;
     writer.write_all(&[b'\n'])?;
     Ok(())
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/ipc_file.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/ipc_file.rs`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         }
         Ok(self.metadata.as_ref().unwrap())
     }
 
     /// Get schema of the Ipc File
     pub fn schema(&mut self) -> PolarsResult<Schema> {
         let metadata = self.get_metadata()?;
-        Ok(metadata.schema.fields.iter().into())
+        Ok(Schema::from_iter(&metadata.schema.fields))
     }
 
     /// Get arrow schema of the Ipc File, this is faster than creating a polars schema.
     pub fn arrow_schema(&mut self) -> PolarsResult<ArrowSchema> {
         let metadata = read::read_file_metadata(&mut self.reader)?;
         Ok(metadata.schema)
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/ipc_stream.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/ipc_stream.rs`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     row_count: Option<RowCount>,
     metadata: Option<StreamMetadata>,
 }
 
 impl<R: Read> IpcStreamReader<R> {
     /// Get schema of the Ipc Stream File
     pub fn schema(&mut self) -> PolarsResult<Schema> {
-        Ok((self.metadata()?.schema.fields.iter()).into())
+        Ok(Schema::from_iter(&self.metadata()?.schema.fields))
     }
 
     /// Get arrow schema of the Ipc Stream File, this is faster than creating a polars schema.
     pub fn arrow_schema(&mut self) -> PolarsResult<ArrowSchema> {
         Ok(self.metadata()?.schema)
     }
     /// Stop reading when `n` rows are read.
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/mmap.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/write.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ipc/write_async.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ipc/write_async.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/json.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/json.rs`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,18 @@
 use std::io::Write;
 use std::ops::Deref;
 
 use arrow::array::StructArray;
 pub use arrow::error::Result as ArrowResult;
 pub use arrow::io::json;
 use polars_arrow::conversion::chunk_to_struct;
+use polars_arrow::utils::CustomIterTools;
 use polars_core::error::to_compute_err;
 use polars_core::prelude::*;
+use polars_core::utils::try_get_supertype;
 
 use crate::mmap::{MmapBytesReader, ReaderBytes};
 use crate::prelude::*;
 
 /// The format to use to write the DataFrame to JSON: `Json` (a JSON array) or `JsonLines` (each row output on a
 /// separate line). In either case, each row is serialized as a JSON object whose keys are the column names and whose
 /// values are the row's corresponding values.
@@ -193,19 +195,40 @@
     /// incompatible types in the input. In the event that a column contains mixed dtypes, is it unspecified whether an
     /// error is returned or whether elements of incompatible dtypes are replaced with `null`.
     fn finish(self) -> PolarsResult<DataFrame> {
         let rb: ReaderBytes = (&self.reader).into();
 
         let out = match self.json_format {
             JsonFormat::Json => {
+                use arrow::io::json::read::json_deserializer::Value;
                 let bytes = rb.deref();
                 let json_value =
                     json::read::json_deserializer::parse(bytes).map_err(to_compute_err)?;
                 // likely struct type
-                let dtype = json::read::infer(&json_value)?;
+                let dtype = if let Value::Array(values) = &json_value {
+                    // struct types may have missing fields so find supertype
+                    let dtype = values
+                        .iter()
+                        .take(self.infer_schema_len.unwrap_or(usize::MAX))
+                        .map(|value| {
+                            json::read::infer(value)
+                                .map_err(PolarsError::from)
+                                .map(|dt| DataType::from(&dt))
+                        })
+                        .fold_first_(|l, r| {
+                            let l = l?;
+                            let r = r?;
+                            try_get_supertype(&l, &r)
+                        })
+                        .unwrap()?;
+                    let dtype = DataType::List(Box::new(dtype));
+                    dtype.to_arrow()
+                } else {
+                    json::read::infer(&json_value)?
+                };
                 let arr = json::read::deserialize(&json_value, dtype)?;
                 let arr = arr.as_any().downcast_ref::<StructArray>().ok_or_else(
                     || polars_err!(ComputeError: "can only deserialize json objects"),
                 )?;
                 DataFrame::try_from(arr.clone())
             }
             JsonFormat::JsonLines => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -2,43 +2,43 @@
 #![cfg_attr(feature = "simd", feature(portable_simd))]
 #![allow(ambiguous_glob_reexports)]
 
 #[cfg(feature = "avro")]
 pub mod avro;
 #[cfg(feature = "cloud")]
 mod cloud;
-#[cfg(any(feature = "csv-file", feature = "json"))]
+#[cfg(any(feature = "csv", feature = "json"))]
 pub mod csv;
 #[cfg(feature = "parquet")]
 pub mod export;
 #[cfg(any(feature = "ipc", feature = "ipc_streaming"))]
 pub mod ipc;
 #[cfg(feature = "json")]
 pub mod json;
 #[cfg(feature = "json")]
 pub mod ndjson_core;
 #[cfg(feature = "cloud")]
 pub use crate::cloud::glob as async_glob;
 
 #[cfg(any(
-    feature = "csv-file",
+    feature = "csv",
     feature = "parquet",
     feature = "ipc",
     feature = "json"
 ))]
 pub mod mmap;
 mod options;
 #[cfg(feature = "parquet")]
 pub mod parquet;
 #[cfg(feature = "private")]
 pub mod predicates;
 #[cfg(not(feature = "private"))]
 pub(crate) mod predicates;
 pub mod prelude;
-#[cfg(all(test, feature = "csv-file"))]
+#[cfg(all(test, feature = "csv"))]
 mod tests;
 pub(crate) mod utils;
 
 #[cfg(feature = "partition")]
 pub mod partition;
 
 use std::io::{Read, Write};
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/mmap.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ndjson_core/buffer.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ndjson_core/buffer.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/ndjson_core/ndjson.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/ndjson_core/ndjson.rs`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         let schema = match schema {
             Some(schema) => Cow::Borrowed(schema),
             None => {
                 let bytes: &[u8] = &reader_bytes;
                 let mut cursor = Cursor::new(bytes);
 
                 let data_type = arrow_ndjson::read::infer(&mut cursor, infer_schema_len)?;
-                let schema: Schema = StructArray::get_fields(&data_type).iter().into();
+                let schema = StructArray::get_fields(&data_type).iter().collect();
 
                 Cow::Owned(schema)
             }
         };
         Ok(CoreJsonReader {
             reader_bytes: Some(reader_bytes),
             schema,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/async_impl.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/async_impl.rs`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     }
 
     pub async fn schema(&mut self) -> PolarsResult<Schema> {
         let metadata = self.get_metadata().await?;
 
         let arrow_schema = parquet2_read::infer_schema(metadata)?;
 
-        Ok(arrow_schema.fields.iter().into())
+        Ok(Schema::from_iter(&arrow_schema.fields))
     }
 
     /// Number of rows in the parquet file.
     pub async fn num_rows(&mut self) -> PolarsResult<usize> {
         let metadata = self.get_metadata().await?;
         Ok(metadata.num_rows)
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/mmap.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/mmap.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/predicates.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/predicates.rs`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         // note that we only select a single row group.
         let st = match rg {
             None => deserialize(fld, md)?,
             // we select a single row group and collect only those stats
             Some(rg) => deserialize(fld, &md[rg..rg + 1])?,
         };
         schema.with_column((&fld.name).into(), (&fld.data_type).into());
-        stats.push(ColumnStats(st, Field::from(fld)));
+        stats.push(ColumnStats(st, fld.into()));
     }
 
     Ok(if stats.is_empty() {
         None
     } else {
         Some(BatchStats { schema, stats })
     })
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/read.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/read.rs`

 * *Files 0% similar despite different names*

```diff
@@ -121,16 +121,15 @@
         self.row_count = row_count;
         self
     }
 
     /// [`Schema`] of the file.
     pub fn schema(&mut self) -> PolarsResult<Schema> {
         let metadata = self.get_metadata()?;
-        let schema = read::infer_schema(metadata)?;
-        Ok(schema.fields.iter().into())
+        Ok(Schema::from_iter(&read::infer_schema(metadata)?.fields))
     }
 
     /// Use statistics in the parquet to determine if pages
     /// can be skipped from reading.
     pub fn use_statistics(mut self, toggle: bool) -> Self {
         self.use_statistics = toggle;
         self
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/read_impl.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/read_impl.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/parquet/write.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/parquet/write.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/partition.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/predicates.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/predicates.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/prelude.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/prelude.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #[cfg(test)]
 use polars_core::prelude::*;
 
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 pub use crate::csv::*;
 #[cfg(any(feature = "ipc", feature = "ipc_streaming"))]
 pub use crate::ipc::*;
 #[cfg(feature = "json")]
 pub use crate::json::*;
 #[cfg(feature = "json")]
 pub use crate::ndjson_core::ndjson::*;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-io/src/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-io/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-error/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-error/Cargo.toml`

 * *Files 11% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 [dependencies]
 regex = { version = "1.6", optional = true }
 thiserror= "^1"
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-error/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-core/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-error/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-error/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 
 [dependencies]
 polars-error = { version = "0.28.0", path = "../polars-error" }
 polars-utils = { version = "0.28.0", path = "../polars-utils" }
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-ops/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encode.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encode.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encodings/fixed.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encodings/fixed.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/encodings/variable.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/encodings/variable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/lib.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/row.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/row.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-row/src/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-row/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-sql/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-sql/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/context.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/context.rs`

 * *Files 9% similar despite different names*

```diff
@@ -18,28 +18,32 @@
 
 thread_local! {pub(crate) static TABLES: RefCell<Vec<String>> = RefCell::new(vec![])}
 
 /// The SQLContext is the main entry point for executing SQL queries.
 #[derive(Default, Clone)]
 pub struct SQLContext {
     pub(crate) table_map: PlHashMap<String, LazyFrame>,
+    pub(crate) tables: Vec<String>,
     cte_map: RefCell<PlHashMap<String, LazyFrame>>,
 }
 
 impl SQLContext {
     /// Create a new SQLContext
     pub fn new() -> Self {
         Self {
             table_map: PlHashMap::new(),
+            tables: vec![],
             cte_map: RefCell::new(PlHashMap::new()),
         }
     }
+
     /// Register a DataFrame as a table in the SQLContext.
     pub fn register(&mut self, name: &str, lf: LazyFrame) {
         self.table_map.insert(name.to_owned(), lf);
+        self.tables.push(name.to_owned());
     }
 
     fn register_cte(&mut self, name: &str, lf: LazyFrame) {
         self.cte_map.borrow_mut().insert(name.to_owned(), lf);
     }
 
     fn get_table_from_current_scope(&mut self, name: &str) -> Option<LazyFrame> {
@@ -62,27 +66,27 @@
         res
     }
 
     pub(crate) fn execute_statement(&mut self, stmt: &Statement) -> PolarsResult<LazyFrame> {
         let ast = stmt;
         Ok(match ast {
             Statement::Query(query) => self.execute_query(query)?,
-
             stmt @ Statement::ShowTables { .. } => self.execute_show_tables(stmt)?,
             stmt @ Statement::CreateTable { .. } => self.execute_create_table(stmt)?,
             _ => polars_bail!(
                 ComputeError: "SQL statement type {:?} is not supported", ast,
             ),
         })
     }
 
     pub(crate) fn execute_query(&mut self, query: &Query) -> PolarsResult<LazyFrame> {
         self.register_ctes(query)?;
         let mut lf = match &query.body.as_ref() {
             SetExpr::Select(select_stmt) => self.execute_select(select_stmt)?,
+            SetExpr::Query(query) => self.execute_query(query)?,
             _ => polars_bail!(ComputeError: "INSERT, UPDATE is not supported"),
         };
 
         if !query.order_by.is_empty() {
             lf = self.process_order_by(lf, &query.order_by)?;
         }
         match &query.limit {
@@ -96,18 +100,15 @@
             _ => polars_bail!(
                 ComputeError: "non-number arguments to LIMIT clause are not supported",
             ),
         }
     }
 
     fn execute_show_tables(&mut self, _: &Statement) -> PolarsResult<LazyFrame> {
-        let tables = Series::new(
-            "name",
-            self.table_map.clone().into_keys().collect::<Vec<_>>(),
-        );
+        let tables = Series::new("name", self.tables.clone());
         let df = DataFrame::new(vec![tables])?;
         Ok(df.lazy())
     }
 
     fn register_ctes(&mut self, query: &Query) -> PolarsResult<()> {
         if let Some(with) = &query.with {
             if with.recursive {
@@ -381,7 +382,32 @@
     fn drop(&mut self) {
         // drop old tables
         TABLES.with(|cell| {
             cell.borrow_mut().clear();
         });
     }
 }
+
+#[cfg(feature = "private")]
+impl SQLContext {
+    /// get all registered tables. For internal use only.
+    pub fn get_tables(&self) -> Vec<String> {
+        self.tables.clone()
+    }
+    /// get internal table map. For internal use only.
+    #[cfg(feature = "private")]
+    pub fn get_table_map(&self) -> PlHashMap<String, LazyFrame> {
+        self.table_map.clone()
+    }
+    /// Create a new SQLContext from a table map and a list of tables. For internal use only
+    #[cfg(feature = "private")]
+    pub fn new_from_tables_and_map(
+        tables: Vec<String>,
+        table_map: PlHashMap<String, LazyFrame>,
+    ) -> Self {
+        Self {
+            table_map,
+            tables,
+            cte_map: RefCell::new(PlHashMap::new()),
+        }
+    }
+}
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/functions.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use polars_core::prelude::{polars_bail, polars_err, PolarsError, PolarsResult};
-use polars_lazy::dsl::{lit, Expr};
+use polars_lazy::dsl::Expr;
+use polars_plan::dsl::count;
 use sqlparser::ast::{
     Expr as SqlExpr, Function as SQLFunction, FunctionArg, FunctionArgExpr, Value as SqlValue,
     WindowSpec,
 };
 
 use crate::sql_expr::parse_sql_expr;
 use crate::SQLContext;
@@ -228,14 +229,59 @@
     /// SQL 'array_contains' function
     /// Returns true if the array contains the value
     /// ```sql
     /// SELECT ARRAY_CONTAINS(column_1, 'foo') from df;
     /// ```
     ArrayContains,
 }
+impl PolarsSqlFunctions {
+    pub(crate) fn keywords() -> &'static [&'static str] {
+        &[
+            "abs",
+            "acos",
+            "asin",
+            "atan",
+            "ceil",
+            "ceiling",
+            "exp",
+            "floor",
+            "ln",
+            "log2",
+            "log10",
+            "log",
+            "log1p",
+            "pow",
+            "lower",
+            "upper",
+            "ltrim",
+            "rtrim",
+            "starts_with",
+            "ends_with",
+            "count",
+            "sum",
+            "min",
+            "max",
+            "avg",
+            "stddev",
+            "variance",
+            "first",
+            "last",
+            "array_length",
+            "array_lower",
+            "array_upper",
+            "array_sum",
+            "array_mean",
+            "array_reverse",
+            "array_unique",
+            "unnest",
+            "array_get",
+            "array_contains",
+        ]
+    }
+}
 
 impl TryFrom<&'_ SQLFunction> for PolarsSqlFunctions {
     type Error = PolarsError;
     fn try_from(function: &'_ SQLFunction) -> Result<Self, Self::Error> {
         let function_name = function.name.0[0].value.to_lowercase();
         Ok(match function_name.as_str() {
             // ----
@@ -399,26 +445,26 @@
         }
     }
 
     fn visit_count(&self) -> PolarsResult<Expr> {
         let args = extract_args(self.func);
         Ok(match (args.len(), self.func.distinct) {
             // count()
-            (0, false) => lit(1i32).count(),
+            (0, false) => count(),
             // count(distinct)
             (0, true) => return not_supported_error("count", &args),
             (1, false) => match args[0] {
                 // count(col)
                 FunctionArgExpr::Expr(sql_expr) => {
                     let expr = self
                         .apply_window_spec(parse_sql_expr(sql_expr, self.ctx)?, &self.func.over)?;
                     expr.count()
                 }
                 // count(*)
-                FunctionArgExpr::Wildcard => lit(1i32).count(),
+                FunctionArgExpr::Wildcard => count(),
                 // count(tbl.*) is not supported
                 _ => return not_supported_error("count", &args),
             },
             (1, true) => {
                 // count(distinct col)
                 if let FunctionArgExpr::Expr(sql_expr) = args[0] {
                     let expr = self
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/lib.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-//! # Polars SQL
+//! Polars SQL
+//! This crate provides a SQL interface for Polars DataFrames
 #![deny(missing_docs)]
 mod context;
 mod functions;
+pub mod keywords;
 mod sql_expr;
 mod table_functions;
+
 pub use context::SQLContext;
 
 #[cfg(test)]
 mod test {
     use polars_core::prelude::*;
     use polars_lazy::dsl::lit;
     use polars_lazy::prelude::*;
@@ -756,22 +759,22 @@
                 r#"
                 SELECT "category" as category
                 FROM foods
                 GROUP BY "category"
         "#,
             )?
             .collect()?
-            .sort(&["category"], vec![false])?;
+            .sort(["category"], vec![false])?;
 
         let expected = LazyCsvReader::new("../../examples/datasets/foods1.csv")
             .finish()?
             .groupby(vec![col("category").alias("category")])
             .agg(vec![])
             .collect()?
-            .sort(&["category"], vec![false])?;
+            .sort(["category"], vec![false])?;
 
         assert!(df_sql.frame_equal(&expected));
         Ok(())
     }
     #[test]
     #[cfg(feature = "ipc")]
     fn test_groupby_2() -> PolarsResult<()> {
@@ -806,15 +809,14 @@
                 ])
                 .sort_by_exprs(
                     vec![col("count"), col("category")],
                     vec![false, true],
                     false,
                 )
                 .limit(2);
-        let lp = expected.clone().describe_optimized_plan()?;
         let expected = expected.collect()?;
         assert!(df_sql.frame_equal(&expected));
         Ok(())
     }
 
     #[test]
     #[cfg(feature = "csv")]
@@ -829,8 +831,28 @@
         assert!(context.execute(sql).is_ok());
 
         let sql = r#"select * from foods"#;
         assert!(context.execute(sql).is_err());
 
         Ok(())
     }
+
+    #[test]
+    #[cfg(feature = "csv")]
+    fn iss_8395() -> PolarsResult<()> {
+        let mut context = SQLContext::new();
+        let sql = r#"
+        with foods as (
+            SELECT *
+            FROM read_csv('../../examples/datasets/foods1.csv')
+        )
+        select * from foods where category IN ('vegetables', 'seafood')"#;
+        let res = context.execute(sql)?;
+        let df = res.collect()?;
+
+        // assert that the df only contains [vegetables, seafood]
+        let s = df.column("category")?.unique()?.sort(false);
+        let expected = Series::new("category", &["seafood", "vegetables"]);
+        assert!(s.series_equal(&expected));
+        Ok(())
+    }
 }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/sql_expr.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/sql_expr.rs`

 * *Files 7% similar despite different names*

```diff
@@ -75,14 +75,19 @@
             SqlExpr::IsNotFalse(expr) => Ok(self.visit_expr(expr)?.eq(lit(false)).not()),
             SqlExpr::IsTrue(expr) => Ok(self.visit_expr(expr)?.eq(lit(true))),
             SqlExpr::IsNotTrue(expr) => Ok(self.visit_expr(expr)?.eq(lit(true)).not()),
             SqlExpr::AnyOp(expr) => Ok(self.visit_expr(expr)?.any()),
             SqlExpr::AllOp(_) => Ok(self.visit_expr(expr)?.all()),
             SqlExpr::Nested(expr) => self.visit_expr(expr),
             SqlExpr::UnaryOp { op, expr } => self.visit_unary_op(op, expr),
+            SqlExpr::InList {
+                expr,
+                list,
+                negated,
+            } => self.visit_is_in(expr, list, *negated),
             other => polars_bail!(ComputeError: "SQL expression {:?} is not yet supported", other),
         }
     }
 
     /// Visit a compound identifier
     ///
     /// e.g. df.column or "df"."column"
@@ -195,14 +200,36 @@
             SqlValue::HexStringLiteral(s) => lit(s.clone()),
             SqlValue::DoubleQuotedString(s) => lit(s.clone()),
             SqlValue::Boolean(b) => lit(*b),
             SqlValue::Null => Expr::Literal(LiteralValue::Null),
             other => polars_bail!(ComputeError: "SQL value {:?} is not yet supported", other),
         })
     }
+
+    // similar to visit_literal, but returns an AnyValue instead of Expr
+    fn visit_anyvalue(&self, value: &SqlValue) -> PolarsResult<AnyValue> {
+        Ok(match value {
+            SqlValue::Number(s, _) => {
+                // Check for existence of decimal separator dot
+                if s.contains('.') {
+                    s.parse::<f64>().map(AnyValue::Float64).map_err(|_| ())
+                } else {
+                    s.parse::<i64>().map(AnyValue::Int64).map_err(|_| ())
+                }
+                .map_err(|_| polars_err!(ComputeError: "cannot parse literal: {:?}"))?
+            }
+            SqlValue::SingleQuotedString(s)
+            | SqlValue::NationalStringLiteral(s)
+            | SqlValue::HexStringLiteral(s)
+            | SqlValue::DoubleQuotedString(s) => AnyValue::Utf8Owned(s.into()),
+            SqlValue::Boolean(b) => AnyValue::Boolean(*b),
+            SqlValue::Null => AnyValue::Null,
+            other => polars_bail!(ComputeError: "SQL value {:?} is not yet supported", other),
+        })
+    }
     /// Visit a SQL `BETWEEN` expression
     /// See [sqlparser::ast::Expr::Between] for more details
     fn visit_between(
         &self,
         expr: &SqlExpr,
         negated: bool,
         low: &SqlExpr,
@@ -271,14 +298,37 @@
         polars_ensure!(
             !expr.within_group,
             ComputeError: "ARRAY_AGG WITHIN GROUP is not yet supported"
         );
         Ok(base.implode())
     }
 
+    /// Visit a SQL `IN` expression
+    fn visit_is_in(&self, expr: &SqlExpr, list: &[SqlExpr], negated: bool) -> PolarsResult<Expr> {
+        let expr = self.visit_expr(expr)?;
+        let list = list
+            .iter()
+            .map(|e| {
+                if let SqlExpr::Value(v) = e {
+                    let av = self.visit_anyvalue(v)?;
+                    Ok(av)
+                } else {
+                    Err(polars_err!(ComputeError: "SQL expression {:?} is not yet supported", e))
+                }
+            })
+            .collect::<PolarsResult<Vec<_>>>()?;
+        let s = Series::from_any_values("", &list, true)?;
+
+        if negated {
+            Ok(expr.is_in(lit(s)).not())
+        } else {
+            Ok(expr.is_in(lit(s)))
+        }
+    }
+
     fn visit_order_by(&self, order_by: &OrderByExpr) -> PolarsResult<(Expr, bool)> {
         let expr = self.visit_expr(&order_by.expr)?;
         let descending = order_by.asc.unwrap_or(false);
         Ok((expr, descending))
     }
 
     fn err(&self, expr: &Expr) -> PolarsResult<Expr> {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-sql/src/table_functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-sql/src/table_functions.rs`

 * *Files 15% similar despite different names*

```diff
@@ -23,28 +23,36 @@
     ReadParquet,
     /// SQL 'read_ipc' function
     /// ```sql
     /// SELECT * FROM read_ipc('path/to/file.ipc')
     /// ```
     #[cfg(feature = "ipc")]
     ReadIpc,
+    /// SQL 'read_json' function. *Only ndjson is currently supported.*
+    /// ```sql
+    /// SELECT * FROM read_json('path/to/file.json')
+    /// ```
+    #[cfg(feature = "json")]
+    ReadJson,
 }
 
 impl FromStr for PolarsTableFunctions {
     type Err = PolarsError;
 
     #[allow(unreachable_code)]
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         Ok(match s {
             #[cfg(feature = "csv")]
             "read_csv" => PolarsTableFunctions::ReadCsv,
             #[cfg(feature = "parquet")]
             "read_parquet" => PolarsTableFunctions::ReadParquet,
             #[cfg(feature = "ipc")]
             "read_ipc" => PolarsTableFunctions::ReadIpc,
+            #[cfg(feature = "json")]
+            "read_json" => PolarsTableFunctions::ReadJson,
             _ => polars_bail!(ComputeError: "'{}' is not a supported table function", s),
         })
     }
 }
 
 impl PolarsTableFunctions {
     #[allow(unused_variables, unreachable_patterns)]
@@ -52,14 +60,16 @@
         match self {
             #[cfg(feature = "csv")]
             PolarsTableFunctions::ReadCsv => self.read_csv(args),
             #[cfg(feature = "parquet")]
             PolarsTableFunctions::ReadParquet => self.read_parquet(args),
             #[cfg(feature = "ipc")]
             PolarsTableFunctions::ReadIpc => self.read_ipc(args),
+            #[cfg(feature = "json")]
+            PolarsTableFunctions::ReadJson => self.read_ndjson(args),
             _ => unreachable!(),
         }
     }
 
     #[cfg(feature = "csv")]
     fn read_csv(&self, args: &[FunctionArg]) -> PolarsResult<(String, LazyFrame)> {
         use polars_lazy::frame::LazyFileListReader;
@@ -77,14 +87,23 @@
 
     #[cfg(feature = "ipc")]
     fn read_ipc(&self, args: &[FunctionArg]) -> PolarsResult<(String, LazyFrame)> {
         let path = self.get_file_path_from_arg(&args[0])?;
         let lf = LazyFrame::scan_ipc(&path, Default::default())?;
         Ok((path, lf))
     }
+    #[cfg(feature = "json")]
+    fn read_ndjson(&self, args: &[FunctionArg]) -> PolarsResult<(String, LazyFrame)> {
+        use polars_lazy::frame::LazyFileListReader;
+        use polars_lazy::prelude::LazyJsonLineReader;
+
+        let path = self.get_file_path_from_arg(&args[0])?;
+        let lf = LazyJsonLineReader::new(path.clone()).finish()?;
+        Ok((path, lf))
+    }
 
     #[allow(dead_code)]
     fn get_file_path_from_arg(&self, arg: &FunctionArg) -> PolarsResult<String> {
         use sqlparser::ast::{Expr as SqlExpr, Value as SqlValue};
         match arg {
             FunctionArg::Unnamed(FunctionArgExpr::Expr(SqlExpr::Value(
                 SqlValue::SingleQuotedString(s),
@@ -92,7 +111,23 @@
             _ => polars_bail!(
                 ComputeError:
                 "only a single quoted string is accepted as the first parameter; received: {}", arg,
             ),
         }
     }
 }
+
+impl PolarsTableFunctions {
+    // list sql names of all table functions
+    pub(crate) fn keywords() -> &'static [&'static str] {
+        &[
+            #[cfg(feature = "csv")]
+            "read_csv",
+            #[cfg(feature = "parquet")]
+            "read_parquet",
+            #[cfg(feature = "ipc")]
+            "read_ipc",
+            #[cfg(feature = "json")]
+            "read_json",
+        ]
+    }
+}
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -27,19 +27,19 @@
 performant = []
 like = ["arrow/compute_like"]
 timezones = ["chrono-tz", "chrono"]
 simd = []
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-lazy/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/default_arrays.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/default_arrays.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/get.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/get.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/null.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/array/utf8.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/array/utf8.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/bit_util.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/bit_util.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/bitmap/mutable.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/bitmap/mutable.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/compute/take/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/compute/take/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/compute/take/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/compute/take/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/conversion.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/conversion.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/data_types.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/data_types.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/floats/ord.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/floats/ord.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/index.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/index.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/is_valid.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/is_valid.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/agg_mean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/agg_mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/concatenate.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/concatenate.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/ewm/average.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/average.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/ewm/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/float.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/float.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/list_bytes_iter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/no_nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/quantile.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/nulls/variance.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/rolling/window.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/rolling/window.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/set.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sort_partition.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sort_partition.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/inner.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/sorted_join/left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/string.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/take_agg/var.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/kernels/time.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/kernels/time.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/time_zone.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/time_zone.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,16 @@
 unsafe impl<A, F: FnMut() -> A> TrustedLen for std::iter::RepeatWith<F> {}
 unsafe impl<A: TrustedLen> TrustedLen for std::iter::Take<A> {}
 
 unsafe impl<I: TrustedLen + DoubleEndedIterator> TrustedLen for std::iter::Rev<I> {}
 
 unsafe impl<I: Iterator<Item = J>, J> TrustedLen for TrustMyLength<I, J> {}
 unsafe impl<T> TrustedLen for std::ops::Range<T> where std::ops::Range<T>: Iterator {}
+unsafe impl<T> TrustedLen for std::ops::RangeInclusive<T> where std::ops::RangeInclusive<T>: Iterator
+{}
 unsafe impl TrustedLen for arrow::array::Utf8ValuesIter<'_, i64> {}
 unsafe impl TrustedLen for arrow::array::BinaryValueIter<'_, i64> {}
 unsafe impl<T, I: TrustedLen + Iterator<Item = T>, V: TrustedLen + Iterator<Item = bool>> TrustedLen
     for ZipValidityIter<T, I, V>
 {
 }
 unsafe impl<T, I: TrustedLen + Iterator<Item = T>, V: TrustedLen + Iterator<Item = bool>> TrustedLen
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/trusted_len/push_unchecked.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-arrow/src/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-arrow/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 polars-row = { version = "0.28.0", path = "../polars-row" }
 polars-utils = { version = "0.28.0", path = "../polars-utils", features = ["sysinfo"] }
 rayon= "1.6"
 smartstring = { version = "1" }
 
 [features]
 compile = []
-csv-file = ["polars-plan/csv-file", "polars-io/csv-file"]
+csv = ["polars-plan/csv", "polars-io/csv"]
 parquet = ["polars-plan/parquet", "polars-io/parquet"]
 ipc = ["polars-plan/ipc", "polars-io/ipc"]
 async = ["polars-plan/async", "polars-io/async"]
 nightly = ["polars-core/nightly", "polars-utils/nightly", "hashbrown/nightly"]
 cross_join = ["polars-core/cross_join"]
 dtype-u8 = ["polars-core/dtype-u8"]
 dtype-u16 = ["polars-core/dtype-u16"]
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/filter.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/filter.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/function.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/function.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/placeholder.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/projection.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/operators/reproject.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/operators/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/file_sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/convert.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/count.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/first.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/interface.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/last.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/mean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/min_max.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/null.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/aggregates/sum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/eval.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/global.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/hash_table.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/generic/thread_local.rs`

 * *Files 2% similar despite different names*

```diff
@@ -41,19 +41,19 @@
     fn split(&self) -> Self {
         let n_columns = self.keys_dtypes.as_ref().len() + self.agg_dtypes.as_ref().len();
 
         let keys_aggs_partitioned = (0..PARTITION_SIZE)
             .map(|_| {
                 let mut buf = Vec::with_capacity(n_columns);
                 for dtype in self.keys_dtypes.as_ref() {
-                    let builder = AnyValueBufferTrusted::new(dtype, OB_SIZE);
+                    let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
                     buf.push(builder);
                 }
                 for dtype in self.agg_dtypes.as_ref() {
-                    let builder = AnyValueBufferTrusted::new(dtype, OB_SIZE);
+                    let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
                     buf.push(builder);
                 }
                 buf
             })
             .collect();
 
         let hash_partitioned = vec![Vec::with_capacity(OB_SIZE); PARTITION_SIZE];
@@ -77,19 +77,19 @@
         if !self.spilled {
             let n_columns = self.keys_dtypes.as_ref().len() + self.agg_dtypes.as_ref().len();
 
             self.keys_aggs_partitioned = (0..PARTITION_SIZE)
                 .map(|_| {
                     let mut buf = Vec::with_capacity(n_columns);
                     for dtype in self.keys_dtypes.as_ref() {
-                        let builder = AnyValueBufferTrusted::new(dtype, OB_SIZE);
+                        let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
                         buf.push(builder);
                     }
                     for dtype in self.agg_dtypes.as_ref() {
-                        let builder = AnyValueBufferTrusted::new(dtype, OB_SIZE);
+                        let builder = AnyValueBufferTrusted::new(&dtype.to_physical(), OB_SIZE);
                         buf.push(builder);
                     }
                     buf
                 })
                 .collect();
 
             self.hash_partitioned = vec![Vec::with_capacity(OB_SIZE); PARTITION_SIZE];
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/ooc_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/primitive/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
                         }
                         // safety:
                         // we will not alias.
                         let ptr = aggregators as *mut AggregateFunction;
                         let agg_fns =
                             unsafe { std::slice::from_raw_parts_mut(ptr, aggregators_len) };
                         let mut key_builder = PrimitiveChunkedBuilder::<K>::new(
-                            self.output_schema.get_index(0).unwrap().0,
+                            self.output_schema.get_at_index(0).unwrap().0,
                             agg_map.len(),
                         );
                         let dtypes = agg_fns
                             .iter()
                             .take(self.number_of_aggs())
                             .map(|func| func.dtype())
                             .collect::<Vec<_>>();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/groupby/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/io.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/io.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/cross.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/generic_build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/joins/inner_left.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/memory.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/memory.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/ordered.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/slice.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/slice.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/ooc.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/sink_multiple.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/sort/source.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sinks/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sinks/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/csv.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/csv.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/frame.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/frame.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/ipc_one_shot.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/parquet.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/parquet.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/reproject.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/reproject.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/executors/sources/union.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/executors/sources/union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/chunks.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/chunks.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/operators/sink.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/operators/sink.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/convert.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/convert.rs`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 // projection is free
                 if let Some(projection) = projection {
                     df = df.select(projection.as_slice())?;
                 }
             }
             Ok(Box::new(sources::DataFrameSource::from_df(df)) as Box<dyn Source>)
         }
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         CsvScan {
             path,
             file_info,
             options,
             predicate,
             output_schema,
             ..
@@ -335,15 +335,15 @@
                     aggregation_columns,
                     Arc::from(agg_fns),
                     output_schema.clone(),
                     options.slice,
                 ))
             } else {
                 match (
-                    output_schema.get_index(0).unwrap().1.to_physical(),
+                    output_schema.get_at_index(0).unwrap().1.to_physical(),
                     keys.len(),
                 ) {
                     (dt, 1) if dt.is_integer() => {
                         with_match_physical_integer_polars_type!(dt, |$T| {
                             Box::new(groupby::PrimitiveGroupbySink::<$T>::new(
                                 key_columns[0].clone(),
                                 aggregation_columns,
@@ -463,15 +463,15 @@
                 lp.clone(),
                 &mut operator_objects,
                 expr_arena,
                 &to_physical,
                 true,
                 verbose,
             )?,
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             lp @ CsvScan { .. } => get_source(
                 lp.clone(),
                 &mut operator_objects,
                 expr_arena,
                 &to_physical,
                 true,
                 verbose,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/dispatcher.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-pipe/src/pipeline/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/src/pipeline/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/Cargo.toml` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ahash= "0.8"
 chrono = { version = "0.4", optional = true }
 chrono-tz = { version = "0.8", optional = true }
 futures = { version = "0.3.25", optional = true }
 once_cell= "1"
 polars-arrow = { version = "0.28.0", path = "../polars-arrow" }
 polars-core = { version = "0.28.0", path = "../polars-core", features = ["lazy", "private", "zip_with", "random"], default-features = false }
-polars-io = { version = "0.28.0", path = "../polars-io", features = ["lazy", "csv-file", "private"], default-features = false }
+polars-io = { version = "0.28.0", path = "../polars-io", features = ["lazy", "csv", "private"], default-features = false }
 polars-ops = { version = "0.28.0", path = "../polars-ops", default-features = false }
 polars-time = { version = "0.28.0", path = "../polars-time", optional = true }
 polars-utils = { version = "0.28.0", path = "../polars-utils" }
 pyo3 = { version = "0.18", optional = true }
 rayon= "1.6"
 regex = { version = "1.6", optional = true }
 serde = { version = "1", features = ["derive", "rc"], optional = true }
@@ -35,15 +35,15 @@
 compile = []
 default = ["compile", "private"]
 streaming = []
 parquet = ["polars-core/parquet", "polars-io/parquet"]
 async = []
 ipc = ["polars-io/ipc"]
 json = ["polars-io/json"]
-csv-file = ["polars-io/csv-file"]
+csv = ["polars-io/csv"]
 temporal = ["polars-core/temporal", "dtype-date", "dtype-datetime", "dtype-time"]
 # debugging purposes
 fmt = ["polars-core/fmt"]
 strings = ["polars-core/strings", "polars-ops/strings"]
 future = []
 dtype-u8 = ["polars-core/dtype-u8"]
 dtype-u16 = ["polars-core/dtype-u16"]
@@ -125,19 +125,19 @@
 [package.metadata.docs.rs]
 all-features = true
 # defines the configuration attribute `docsrs`
 rustdoc-args = ["--cfg", "docsrs"]
 
 [dependencies.arrow]
 package = "arrow2"
-git = "https://github.com/jorgecarleitao/arrow2"
-# git = "https://github.com/ritchie46/arrow2"
-rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+# git = "https://github.com/jorgecarleitao/arrow2"
+git = "https://github.com/ritchie46/arrow2"
+# rev = "1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
 # path = "../arrow2"
-# branch = "polars_2023-04-05"
+branch = "polars_2023-04-20"
 version = "0.17"
 default-features = false
 features = [
   "compute_aggregate",
   "compute_arithmetics",
   "compute_boolean",
   "compute_boolean_kleene",
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/LICENSE` & `polars_lts_cpu-0.17.6/local_dependencies/polars-pipe/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dot.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dot.rs`

 * *Files 1% similar despite different names*

```diff
@@ -336,15 +336,15 @@
                 };
                 if self.is_single(branch, id) {
                     self.write_single_node(acc_str, current_node)
                 } else {
                     self.write_dot(acc_str, prev_node, current_node, id_map)
                 }
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan {
                 path,
                 options,
                 file_info,
                 predicate,
                 ..
             } => self.write_scan(
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/arithmetic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/arithmetic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/binary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/cat.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/dt.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/dt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/expr.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/from.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/from.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/arg_where.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/boolean.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/bounds.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cat.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/cum.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/datetime.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/dispatch.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/log.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/log.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/pow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/schema.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
         let mapper = FieldsMapper { fields };
         match self {
             #[cfg(feature = "abs")]
             Abs => mapper.with_same_dtype(),
             NullCount => mapper.with_dtype(IDX_DTYPE),
             Pow => mapper.map_to_float_dtype(),
-            Coalesce => mapper.map_to_list_supertype(),
+            Coalesce => mapper.map_to_supertype(),
             #[cfg(feature = "row_hash")]
             Hash(..) => mapper.with_dtype(DataType::UInt64),
             #[cfg(feature = "arg_where")]
             ArgWhere => mapper.with_dtype(IDX_DTYPE),
             #[cfg(feature = "search_sorted")]
             SearchSorted(_) => mapper.with_dtype(IDX_DTYPE),
             #[cfg(feature = "strings")]
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shift_and_fill.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/shrink_type.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/sign.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/strings.rs`

 * *Files 1% similar despite different names*

```diff
@@ -339,33 +339,34 @@
 
     let ca = s.utf8()?;
     ca.count_match(&pat).map(|ca| ca.into_series())
 }
 
 #[cfg(feature = "temporal")]
 pub(super) fn strptime(s: &Series, options: &StrpTimeOptions) -> PolarsResult<Series> {
-    let tz_aware = match (options.tz_aware, &options.fmt) {
+    let tz_aware = match (options.tz_aware, &options.format) {
         (true, Some(_)) => true,
         (true, None) => polars_bail!(
             ComputeError:
-            "passing 'tz_aware=True' without 'fmt' is not yet supported, please specify 'fmt'"
+            "passing 'tz_aware=True' without 'format' is not yet supported, please specify 'format'"
         ),
         #[cfg(feature = "timezones")]
-        (false, Some(fmt)) => TZ_AWARE_RE.is_match(fmt),
+        (false, Some(format)) => TZ_AWARE_RE.is_match(format),
         (false, _) => false,
     };
     let ca = s.utf8()?;
 
     let out = match &options.date_dtype {
         DataType::Date => {
             if options.exact {
-                ca.as_date(options.fmt.as_deref(), options.cache)?
+                ca.as_date(options.format.as_deref(), options.cache)?
                     .into_series()
             } else {
-                ca.as_date_not_exact(options.fmt.as_deref())?.into_series()
+                ca.as_date_not_exact(options.format.as_deref())?
+                    .into_series()
             }
         }
         DataType::Datetime(tu, tz) => {
             match (tz, tz_aware, options.utc) {
                 (Some(_), true, _) => polars_bail!(
                     ComputeError:
                     "cannot use strptime with both a tz-aware format and a tz-aware dtype, \
@@ -376,32 +377,32 @@
                     "cannot use strptime with both 'utc=True' and tz-aware dtype, \
                     please drop time zone from the dtype"
                 ),
                 _ => (),
             };
             if options.exact {
                 ca.as_datetime(
-                    options.fmt.as_deref(),
+                    options.format.as_deref(),
                     *tu,
                     options.cache,
                     tz_aware,
                     options.utc,
                     tz.as_ref(),
                 )?
                 .into_series()
             } else {
-                ca.as_datetime_not_exact(options.fmt.as_deref(), *tu, tz.as_ref())?
+                ca.as_datetime_not_exact(options.format.as_deref(), *tu, tz.as_ref())?
                     .into_series()
             }
         }
         dt @ DataType::Time => {
             polars_ensure!(
                 options.exact, ComputeError: "non-exact not implemented for datatype {}", dt,
             );
-            ca.as_time(options.fmt.as_deref(), options.cache)?
+            ca.as_time(options.format.as_deref(), options.cache)?
                 .into_series()
         }
         dt => polars_bail!(ComputeError: "not implemented for dtype {}", dt),
     };
     if options.strict {
         polars_ensure!(
             out.null_count() == ca.null_count(),
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/temporal.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/function_expr/trigonometry.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/functions.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/functions.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 use polars_core::utils::arrow::temporal_conversions::SECONDS_IN_DAY;
 #[cfg(feature = "dtype-struct")]
 use polars_core::utils::get_supertype;
 
 #[cfg(feature = "arg_where")]
 use crate::dsl::function_expr::FunctionExpr;
 use crate::dsl::function_expr::ListFunction;
-#[cfg(feature = "strings")]
+#[cfg(all(feature = "concat_str", feature = "strings"))]
 use crate::dsl::function_expr::StringFunction;
 use crate::dsl::*;
 use crate::prelude::*;
 
 /// Compute the covariance between two columns.
 pub fn cov(a: Expr, b: Expr) -> Expr {
     let name = "cov";
@@ -322,18 +322,18 @@
             fmt_str: "concat_list",
             ..Default::default()
         },
     })
 }
 
 /// Create list entries that are range arrays
-/// - if `low` and `high` are a column, every element will expand into an array in a list column.
-/// - if `low` and `high` are literals the output will be of `Int64`.
+/// - if `start` and `end` are a column, every element will expand into an array in a list column.
+/// - if `start` and `end` are literals the output will be of `Int64`.
 #[cfg(feature = "arange")]
-pub fn arange(low: Expr, high: Expr, step: usize) -> Expr {
+pub fn arange(start: Expr, end: Expr, step: i64) -> Expr {
     let has_col_without_agg = |e: &Expr| {
         has_expr(e, |ae| matches!(ae, Expr::Column(_)))
             &&
             // check if there is no aggregation
             !has_expr(e, |ae| {
                 matches!(
                     ae,
@@ -356,97 +356,116 @@
                 )
             })
     };
     let has_lit = |e: &Expr| {
         (matches!(e, Expr::Literal(_)) && !matches!(e, Expr::Literal(LiteralValue::Series(_))))
     };
 
-    let any_column_no_agg = has_col_without_agg(&low) || has_col_without_agg(&high);
-    let literal_low = has_lit(&low);
-    let literal_high = has_lit(&high);
+    let any_column_no_agg = has_col_without_agg(&start) || has_col_without_agg(&end);
+    let literal_start = has_lit(&start);
+    let literal_end = has_lit(&end);
 
-    if (literal_low || literal_high) && !any_column_no_agg {
+    if (literal_start || literal_end) && !any_column_no_agg {
         let f = move |sa: Series, sb: Series| {
+            polars_ensure!(step != 0, InvalidOperation: "step must not be zero");
             let sa = sa.cast(&DataType::Int64)?;
             let sb = sb.cast(&DataType::Int64)?;
-            let low = sa
+            let start = sa
                 .i64()?
                 .get(0)
-                .ok_or_else(|| polars_err!(NoData: "no data in `low` evaluation"))?;
-            let high = sb
+                .ok_or_else(|| polars_err!(NoData: "no data in `start` evaluation"))?;
+            let end = sb
                 .i64()?
                 .get(0)
-                .ok_or_else(|| polars_err!(NoData: "no data in `high` evaluation"))?;
+                .ok_or_else(|| polars_err!(NoData: "no data in `end` evaluation"))?;
 
-            let mut ca = if step > 1 {
-                Int64Chunked::from_iter_values("arange", (low..high).step_by(step))
-            } else {
-                Int64Chunked::from_iter_values("arange", low..high)
+            let mut ca = match step {
+                1 => Int64Chunked::from_iter_values("arange", start..end),
+                2.. => {
+                    Int64Chunked::from_iter_values("arange", (start..end).step_by(step as usize))
+                }
+                _ => {
+                    polars_ensure!(start > end, InvalidOperation: "range must be decreasing if 'step' is negative");
+                    Int64Chunked::from_iter_values(
+                        "arange",
+                        (end..=start).rev().step_by(step.unsigned_abs() as usize),
+                    )
+                }
             };
-            let is_sorted = if high < low {
+            let is_sorted = if end < start {
                 IsSorted::Descending
             } else {
                 IsSorted::Ascending
             };
             ca.set_sorted_flag(is_sorted);
             Ok(Some(ca.into_series()))
         };
         apply_binary(
-            low,
-            high,
+            start,
+            end,
             f,
             GetOutput::map_field(|_| Field::new("arange", DataType::Int64)),
         )
     } else {
         let f = move |sa: Series, sb: Series| {
+            polars_ensure!(step != 0, InvalidOperation: "step must not be zero");
             let mut sa = sa.cast(&DataType::Int64)?;
             let mut sb = sb.cast(&DataType::Int64)?;
 
             if sa.len() != sb.len() {
                 if sa.len() == 1 {
                     sa = sa.new_from_index(0, sb.len())
                 } else if sb.len() == 1 {
                     sb = sb.new_from_index(0, sa.len())
                 } else {
                     polars_bail!(
                         ComputeError:
-                        "lengths of `low`: {} and `high`: {} arguments `\
+                        "lengths of `start`: {} and `end`: {} arguments `\
                         cannot be matched in the `arange` expression",
                         sa.len(), sb.len()
                     );
                 }
             }
 
-            let low = sa.i64()?;
-            let high = sb.i64()?;
+            let start = sa.i64()?;
+            let end = sb.i64()?;
             let mut builder = ListPrimitiveChunkedBuilder::<Int64Type>::new(
                 "arange",
-                low.len(),
-                low.len() * 3,
+                start.len(),
+                start.len() * 3,
                 DataType::Int64,
             );
 
-            low.into_iter()
-                .zip(high.into_iter())
-                .for_each(|(opt_l, opt_h)| match (opt_l, opt_h) {
-                    (Some(l), Some(r)) => {
-                        if step > 1 {
-                            builder.append_iter_values((l..r).step_by(step));
-                        } else {
-                            builder.append_iter_values(l..r);
+            for (opt_start, opt_end) in start.into_iter().zip(end.into_iter()) {
+                match (opt_start, opt_end) {
+                    (Some(start_v), Some(end_v)) => match step {
+                        1 => {
+                            builder.append_iter_values(start_v..end_v);
+                        }
+                        2.. => {
+                            builder.append_iter_values((start_v..end_v).step_by(step as usize));
                         }
-                    }
+                        _ => {
+                            polars_ensure!(start_v > end_v, InvalidOperation: "range must be decreasing if 'step' is negative");
+                            builder.append_iter_values(
+                                (end_v..=start_v)
+                                    .rev()
+                                    .step_by(step.unsigned_abs() as usize),
+                            )
+                        }
+                    },
                     _ => builder.append_null(),
-                });
+                }
+            }
 
             Ok(Some(builder.finish().into_series()))
         };
         apply_binary(
-            low,
-            high,
+            start,
+            end,
             f,
             GetOutput::map_field(|_| Field::new("arange", DataType::List(DataType::Int64.into()))),
         )
     }
 }
 
 macro_rules! impl_unit_setter {
@@ -724,14 +743,21 @@
 }
 
 /// Construct a column of `Duration` from the provided [`DurationArgs`]
 #[cfg(feature = "temporal")]
 pub fn duration(args: DurationArgs) -> Expr {
     let function = SpecialEq::new(Arc::new(move |s: &mut [Series]| {
         assert_eq!(s.len(), 8);
+        if s.iter().any(|s| s.is_empty()) {
+            return Ok(Some(Series::new_empty(
+                s[0].name(),
+                &DataType::Duration(TimeUnit::Nanoseconds),
+            )));
+        }
+
         let days = s[0].cast(&DataType::Int64).unwrap();
         let seconds = s[1].cast(&DataType::Int64).unwrap();
         let mut nanoseconds = s[2].cast(&DataType::Int64).unwrap();
         let microseconds = s[3].cast(&DataType::Int64).unwrap();
         let milliseconds = s[4].cast(&DataType::Int64).unwrap();
         let minutes = s[5].cast(&DataType::Int64).unwrap();
         let hours = s[6].cast(&DataType::Int64).unwrap();
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/list.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/list.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/meta.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/options.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/options.rs`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 #[derive(Clone, PartialEq, Debug, Eq, Hash)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub struct StrpTimeOptions {
     /// DataType to parse in. One of {Date, Datetime}
     pub date_dtype: DataType,
     /// Formatting string
-    pub fmt: Option<String>,
+    pub format: Option<String>,
     /// If set then polars will return an error if any date parsing fails
     pub strict: bool,
     /// If polars may parse matches that not contain the whole string
     /// e.g. "foo-2021-01-01-bar" could match "2021-01-01"
     pub exact: bool,
     /// use a cache of unique, converted dates to apply the datetime conversion.
     pub cache: bool,
@@ -25,15 +25,15 @@
     pub utc: bool,
 }
 
 impl Default for StrpTimeOptions {
     fn default() -> Self {
         StrpTimeOptions {
             date_dtype: DataType::Datetime(TimeUnit::Microseconds, None),
-            fmt: None,
+            format: None,
             strict: false,
             exact: false,
             cache: true,
             tz_aware: false,
             utc: false,
         }
     }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/string.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/string.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/dsl/struct_.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/dsl/struct_.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/frame/opt_state.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/frame/opt_state.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/aexpr/schema.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/alp.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/alp.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use std::borrow::Cow;
-#[cfg(any(feature = "ipc", feature = "csv-file", feature = "parquet"))]
+#[cfg(any(feature = "ipc", feature = "csv", feature = "parquet"))]
 use std::path::PathBuf;
 use std::sync::Arc;
 
 #[cfg(feature = "parquet")]
 use polars_core::cloud::CloudOptions;
 use polars_core::prelude::*;
 use polars_utils::arena::{Arena, Node};
 
 use crate::logical_plan::functions::FunctionNode;
 use crate::logical_plan::schema::{det_join_schema, FileInfo};
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 use crate::logical_plan::CsvParserOptions;
 #[cfg(feature = "ipc")]
 use crate::logical_plan::IpcScanOptionsInner;
 #[cfg(feature = "parquet")]
 use crate::logical_plan::ParquetOptions;
 use crate::prelude::*;
 use crate::utils::{aexprs_to_schema, PushNode};
@@ -39,15 +39,15 @@
         offset: i64,
         len: IdxSize,
     },
     Selection {
         input: Node,
         predicate: Node,
     },
-    #[cfg(feature = "csv-file")]
+    #[cfg(feature = "csv")]
     CsvScan {
         path: PathBuf,
         file_info: FileInfo,
         // schema of the projected file
         output_schema: Option<SchemaRef>,
         options: CsvParserOptions,
         predicate: Option<Node>,
@@ -159,15 +159,15 @@
     /// Get the schema of the logical plan node but don't take projections into account at the scan
     /// level. This ensures we can apply the predicate
     pub(crate) fn scan_schema(&self) -> &SchemaRef {
         use ALogicalPlan::*;
         match self {
             #[cfg(feature = "python")]
             PythonScan { options, .. } => &options.schema,
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { file_info, .. } => &file_info.schema,
             #[cfg(feature = "parquet")]
             ParquetScan { file_info, .. } => &file_info.schema,
             #[cfg(feature = "ipc")]
             IpcScan { file_info, .. } => &file_info.schema,
             AnonymousScan { file_info, .. } => &file_info.schema,
             _ => unreachable!(),
@@ -178,15 +178,15 @@
         use ALogicalPlan::*;
         match self {
             AnonymousScan { .. } => "anonymous_scan",
             #[cfg(feature = "python")]
             PythonScan { .. } => "python_scan",
             Slice { .. } => "slice",
             Selection { .. } => "selection",
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { .. } => "csv_scan",
             #[cfg(feature = "ipc")]
             IpcScan { .. } => "ipc_scan",
             #[cfg(feature = "parquet")]
             ParquetScan { .. } => "parquet_scan",
             DataFrameScan { .. } => "df",
             Projection { .. } => "projection",
@@ -232,15 +232,15 @@
             } => output_schema.as_ref().unwrap_or(schema),
             AnonymousScan {
                 file_info,
                 output_schema,
                 ..
             } => output_schema.as_ref().unwrap_or(&file_info.schema),
             Selection { input, .. } => return arena.get(*input).schema(arena),
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan {
                 file_info,
                 output_schema,
                 ..
             } => output_schema.as_ref().unwrap_or(&file_info.schema),
             Projection { schema, .. } => schema,
             LocalProjection { schema, .. } => schema,
@@ -398,15 +398,15 @@
                     file_info: file_info.clone(),
                     output_schema: output_schema.clone(),
                     predicate: new_predicate,
                     options: options.clone(),
                     cloud_options: cloud_options.clone(),
                 }
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan {
                 path,
                 file_info,
                 output_schema,
                 predicate,
                 options,
                 ..
@@ -507,15 +507,15 @@
             }
             #[cfg(feature = "ipc")]
             IpcScan { predicate, .. } => {
                 if let Some(node) = predicate {
                     container.push(*node)
                 }
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { predicate, .. } => {
                 if let Some(node) = predicate {
                     container.push(*node)
                 }
             }
             DataFrameScan { selection, .. } => {
                 if let Some(expr) = selection {
@@ -583,15 +583,15 @@
                 }
                 *input
             }
             #[cfg(feature = "parquet")]
             ParquetScan { .. } => return,
             #[cfg(feature = "ipc")]
             IpcScan { .. } => return,
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { .. } => return,
             DataFrameScan { .. } => return,
             AnonymousScan { .. } => return,
             #[cfg(feature = "python")]
             PythonScan { .. } => return,
         };
         container.push_node(input)
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/anonymous_scan.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/apply.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/builder.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/builder.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 use std::io::{Read, Seek};
 
 #[cfg(feature = "parquet")]
 use polars_core::cloud::CloudOptions;
 use polars_core::frame::explode::MeltArgs;
 use polars_core::prelude::*;
 use polars_core::utils::try_get_supertype;
 #[cfg(feature = "ipc")]
 use polars_io::ipc::IpcReader;
 #[cfg(all(feature = "parquet", feature = "async"))]
 use polars_io::parquet::ParquetAsyncReader;
 #[cfg(feature = "parquet")]
 use polars_io::parquet::ParquetReader;
-#[cfg(any(feature = "parquet", feature = "parquet_async", feature = "csv-file"))]
+#[cfg(any(feature = "parquet", feature = "parquet_async", feature = "csv"))]
 use polars_io::RowCount;
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 use polars_io::{
     csv::utils::{get_reader_bytes, infer_file_schema, is_compressed},
     csv::CsvEncoding,
     csv::NullValues,
 };
 
 use crate::logical_plan::functions::FunctionNode;
@@ -196,15 +196,15 @@
             predicate: None,
             options: options.into(),
         }
         .into())
     }
 
     #[allow(clippy::too_many_arguments)]
-    #[cfg(feature = "csv-file")]
+    #[cfg(feature = "csv")]
     pub fn scan_csv<P: Into<std::path::PathBuf>>(
         path: P,
         delimiter: u8,
         has_header: bool,
         ignore_errors: bool,
         mut skip_rows: usize,
         n_rows: Option<usize>,
@@ -331,20 +331,15 @@
         .into()
     }
 
     pub fn fill_null(self, fill_value: Expr) -> Self {
         let schema = try_delayed!(self.0.schema(), &self.0, into);
         let exprs = schema
             .iter_names()
-            .map(|name| {
-                when(col(name).is_null())
-                    .then(fill_value.clone())
-                    .otherwise(col(name))
-                    .alias(name)
-            })
+            .map(|name| col(name).fill_null(fill_value.clone()))
             .collect();
         self.project_local(exprs)
     }
 
     pub fn fill_nan(self, fill_value: Expr) -> Self {
         let schema = try_delayed!(self.0.schema(), &self.0, into);
 
@@ -734,19 +729,19 @@
             },
         }
         .into()
     }
 }
 
 pub(crate) fn det_melt_schema(args: &MeltArgs, input_schema: &Schema) -> SchemaRef {
-    let mut new_schema = Schema::from(
-        args.id_vars
-            .iter()
-            .map(|id| Field::new(id, input_schema.get(id).unwrap().clone())),
-    );
+    let mut new_schema = args
+        .id_vars
+        .iter()
+        .map(|id| Field::new(id, input_schema.get(id).unwrap().clone()))
+        .collect::<Schema>();
     let variable_name = args
         .variable_name
         .as_ref()
         .cloned()
         .unwrap_or_else(|| "variable".into());
     let value_name = args
         .value_name
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/conversion.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/conversion.rs`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,15 @@
                 predicate: p,
             }
         }
         LogicalPlan::Slice { input, offset, len } => {
             let input = to_alp(*input, expr_arena, lp_arena)?;
             ALogicalPlan::Slice { input, offset, len }
         }
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         LogicalPlan::CsvScan {
             path,
             file_info,
             options,
             predicate,
         } => ALogicalPlan::CsvScan {
             path,
@@ -680,15 +680,15 @@
                 let lp = convert_to_lp(input, lp_arena);
                 let p = node_to_expr(predicate, expr_arena);
                 LogicalPlan::Selection {
                     input: Box::new(lp),
                     predicate: p,
                 }
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             ALogicalPlan::CsvScan {
                 path,
                 file_info,
                 output_schema: _,
                 options,
                 predicate,
             } => LogicalPlan::CsvScan {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/format.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/format.rs`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
                     predicate,
                 )
             }
             Selection { predicate, input } => {
                 write!(f, "{:indent$}FILTER {predicate:?} FROM", "")?;
                 input._format(f, indent)
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan {
                 path,
                 options,
                 file_info,
                 predicate,
                 ..
             } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/drop.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/merge_sorted.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -150,17 +150,15 @@
             },
             Pipeline { schema, .. } => Ok(Cow::Owned(schema.clone())),
             FastProjection { columns } => {
                 let schema = columns
                     .iter()
                     .map(|name| {
                         let name = name.as_ref();
-                        input_schema
-                            .get_field(name)
-                            .ok_or_else(|| polars_err!(SchemaFieldNotFound: "{}", name))
+                        input_schema.try_get_field(name)
                     })
                     .collect::<PolarsResult<Schema>>()?;
                 Ok(Cow::Owned(Arc::new(schema)))
             }
             DropNulls { .. } => Ok(Cow::Borrowed(input_schema)),
             Rechunk => Ok(Cow::Borrowed(input_schema)),
             Unnest { columns: _columns } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/functions/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/iterator.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/iterator.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/lit.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/lit.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use std::fmt::Debug;
-#[cfg(any(feature = "ipc", feature = "csv-file", feature = "parquet"))]
+#[cfg(any(feature = "ipc", feature = "csv", feature = "parquet"))]
 use std::path::PathBuf;
 use std::sync::{Arc, Mutex};
 
 #[cfg(feature = "parquet")]
 use polars_core::cloud::CloudOptions;
 use polars_core::prelude::*;
 
@@ -41,20 +41,15 @@
 pub use iterator::*;
 pub use lit::*;
 pub use optimizer::*;
 pub use schema::*;
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 
-#[cfg(any(
-    feature = "ipc",
-    feature = "parquet",
-    feature = "csv-file",
-    feature = "cse"
-))]
+#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv", feature = "cse"))]
 pub use crate::logical_plan::optimizer::file_caching::{
     collect_fingerprints, find_column_union_and_fingerprints, FileCacher, FileFingerPrint,
 };
 use crate::logical_plan::schema::FileInfo;
 
 #[derive(Clone, Copy, Debug)]
 pub enum Context {
@@ -155,15 +150,15 @@
     /// Cache the input at this point in the LP
     Cache {
         input: Box<LogicalPlan>,
         id: usize,
         count: usize,
     },
     /// Scan a CSV file
-    #[cfg(feature = "csv-file")]
+    #[cfg(feature = "csv")]
     CsvScan {
         path: PathBuf,
         file_info: FileInfo,
         options: CsvParserOptions,
         /// Filters at the scan level
         predicate: Option<Expr>,
     },
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cache_states.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/cse.rs`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 ..
             },
         ) => {
             path_left == path_right
                 && options_l == options_r
                 && predicate_equal(*predicate_l, *predicate_r, expr_arena)
         }
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         (
             CsvScan {
                 path: path_left,
                 predicate: predicate_l,
                 options: options_l,
                 ..
             },
@@ -435,15 +435,15 @@
         IpcScan { options, .. } => {
             if acc_count >= options.file_counter {
                 options.file_counter = 1;
             } else {
                 options.file_counter -= acc_count as FileCount
             }
         }
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         CsvScan { options, .. } => {
             if acc_count >= options.file_counter {
                 options.file_counter = 1;
             } else {
                 options.file_counter -= acc_count as FileCount
             }
         }
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/delay_rechunk.rs`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                     match lp {
                         // we get the input node
                         #[cfg(feature = "parquet")]
                         ParquetScan { .. } => {
                             input_node = Some(node);
                             break;
                         }
-                        #[cfg(feature = "csv-file")]
+                        #[cfg(feature = "csv")]
                         CsvScan { .. } => {
                             input_node = Some(node);
                             break;
                         }
                         #[cfg(feature = "ipc")]
                         IpcScan { .. } => {
                             input_node = Some(node);
@@ -58,15 +58,15 @@
                         _ => {}
                     }
                     previous_node = node;
                 }
 
                 if let Some(node) = input_node {
                     match lp_arena.get_mut(node) {
-                        #[cfg(feature = "csv-file")]
+                        #[cfg(feature = "csv")]
                         CsvScan { options, .. } => {
                             options.rechunk = false;
                         }
                         #[cfg(feature = "parquet")]
                         ParquetScan { options, .. } => options.rechunk = false,
                         #[cfg(feature = "ipc")]
                         IpcScan { options, .. } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/drop_nulls.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/fast_projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/file_caching.rs`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     root: Node,
     fps: &mut Vec<FileFingerPrint>,
     lp_arena: &Arena<ALogicalPlan>,
     expr_arena: &Arena<AExpr>,
 ) {
     use ALogicalPlan::*;
     match lp_arena.get(root) {
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         CsvScan {
             path,
             options,
             predicate,
             ..
         } => {
             let slice = (options.skip_rows, options.n_rows);
@@ -123,15 +123,15 @@
     // we also keep track of how often a needs file needs to be read so we can cache until last read
     columns: &mut PlHashMap<FileFingerPrint, (FileCount, PlIndexSet<String>)>,
     lp_arena: &Arena<ALogicalPlan>,
     expr_arena: &Arena<AExpr>,
 ) {
     use ALogicalPlan::*;
     match lp_arena.get(root) {
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         CsvScan {
             path,
             options,
             predicate,
             file_info,
             ..
         } => {
@@ -314,15 +314,15 @@
                         lp_arena,
                         &finger_print,
                         options.with_columns,
                         behind_cache,
                     );
                     lp_arena.replace(root, lp);
                 }
-                #[cfg(feature = "csv-file")]
+                #[cfg(feature = "csv")]
                 ALogicalPlan::CsvScan {
                     path,
                     file_info,
                     output_schema,
                     predicate,
                     mut options,
                 } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/flatten_union.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,34 +5,29 @@
 
 mod cache_states;
 #[cfg(feature = "cse")]
 mod cse;
 mod delay_rechunk;
 mod drop_nulls;
 mod fast_projection;
-#[cfg(any(
-    feature = "ipc",
-    feature = "parquet",
-    feature = "csv-file",
-    feature = "cse"
-))]
+#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv", feature = "cse"))]
 pub(crate) mod file_caching;
 mod flatten_union;
 mod predicate_pushdown;
 mod projection_pushdown;
 mod simplify_expr;
 mod slice_pushdown_expr;
 mod slice_pushdown_lp;
 mod stack_opt;
 mod type_coercion;
 
 use delay_rechunk::DelayRechunk;
 use drop_nulls::ReplaceDropNulls;
 use fast_projection::FastProjectionAndCollapse;
-#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv-file"))]
+#[cfg(any(feature = "ipc", feature = "parquet", feature = "csv"))]
 use file_caching::{find_column_union_and_fingerprints, FileCacher};
 pub use predicate_pushdown::PredicatePushDown;
 pub use projection_pushdown::ProjectionPushDown;
 pub use simplify_expr::{SimplifyBooleanRule, SimplifyExprRule};
 use slice_pushdown_lp::SlicePushDown;
 pub use stack_opt::{OptimizationRule, StackOptimizer};
 pub use type_coercion::TypeCoercionRule;
@@ -139,20 +134,15 @@
     if simplify_expr {
         rules.push(Box::new(SimplifyBooleanRule {}));
     }
 
     // make sure that we do that once slice pushdown
     // and predicate pushdown are done. At that moment
     // the file fingerprints are finished.
-    #[cfg(any(
-        feature = "cse",
-        feature = "parquet",
-        feature = "ipc",
-        feature = "csv-file"
-    ))]
+    #[cfg(any(feature = "cse", feature = "parquet", feature = "ipc", feature = "csv"))]
     if agg_scan_projection || cse_changed {
         // we do this so that expressions are simplified created by the pushdown optimizations
         // we must clean up the predicates, because the agg_scan_projection
         // uses them in the hashtable to determine duplicates.
         let simplify_bools = &mut [Box::new(SimplifyBooleanRule {}) as Box<dyn OptimizationRule>];
         lp_top = opt.optimize_loop(simplify_bools, expr_arena, lp_arena, lp_top)?;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/keys.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,15 @@
                     output_schema,
                     predicate,
                     options,
                     cloud_options,
                 };
                 Ok(self.optional_apply_predicate(lp, local_predicates, lp_arena, expr_arena))
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan {
                 path,
                 file_info,
                 output_schema,
                 options,
                 predicate,
             } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/predicate_pushdown/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/melt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/functions/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/generic.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/groupby.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/hstack.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/joins.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -490,15 +490,15 @@
                         expr_arena,
                         &options.schema,
                         true,
                     )?))
                 };
                 Ok(PythonScan { options, predicate })
             }
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan {
                 path,
                 file_info,
                 mut options,
                 predicate,
                 ..
             } => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/projection.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/rename.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/projection_pushdown/semi_anti_join.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/simplify_expr.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 use polars_utils::arena::Arena;
 
-#[cfg(feature = "strings")]
+#[cfg(all(feature = "strings", feature = "concat_str"))]
 use crate::dsl::function_expr::StringFunction;
 use crate::logical_plan::optimizer::stack_opt::OptimizationRule;
 use crate::logical_plan::*;
 use crate::prelude::function_expr::FunctionExpr;
 
 macro_rules! eval_binary_same_type {
     ($lhs:expr, $operand: tt, $rhs:expr) => {{
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_expr.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/slice_pushdown_lp.rs`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
                     options
                 };
 
                 Ok(lp)
 
             }
 
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             (CsvScan {
                 path,
                 file_info,
                 output_schema,
                 mut options,
                 predicate,
             }, Some(state)) if state.offset >= 0 && predicate.is_none() => {
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/stack_opt.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/binary.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/optimizer/type_coercion/mod.rs`

 * *Files 0% similar despite different names*

```diff
@@ -514,15 +514,15 @@
 
     use super::*;
     use crate::prelude::*;
 
     #[test]
     fn test_categorical_utf8() {
         let mut rules: Vec<Box<dyn OptimizationRule>> = vec![Box::new(TypeCoercionRule {})];
-        let schema = Schema::from(vec![Field::new("fruits", DataType::Categorical(None))]);
+        let schema = Schema::from_iter([Field::new("fruits", DataType::Categorical(None))]);
 
         let expr = col("fruits").eq(lit("somestr"));
         let out = optimize_expr(expr.clone(), schema.clone(), &mut rules);
         // we test that the fruits column is not casted to utf8 for the comparison
         assert_eq!(out, expr);
 
         let expr = col("fruits") + (lit("somestr"));
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/options.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/options.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use std::path::PathBuf;
 
 use polars_core::prelude::*;
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 use polars_io::csv::{CsvEncoding, NullValues};
 #[cfg(feature = "ipc")]
 use polars_io::ipc::IpcCompression;
 #[cfg(feature = "parquet")]
 use polars_io::parquet::ParquetCompression;
 use polars_io::RowCount;
 #[cfg(feature = "dynamic_groupby")]
@@ -13,15 +13,15 @@
 #[cfg(feature = "serde")]
 use serde::{Deserialize, Serialize};
 
 use crate::prelude::Expr;
 
 pub type FileCount = u32;
 
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 #[derive(Clone, Debug, PartialEq, Eq)]
 #[cfg_attr(feature = "serde", derive(Serialize, Deserialize))]
 pub struct CsvParserOptions {
     pub delimiter: u8,
     pub comment_char: Option<u8>,
     pub quote_char: Option<u8>,
     pub eol_char: u8,
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/projection.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/projection.rs`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         Expr::Nth(i) => {
             match i.negative_to_usize(schema.len()) {
                 None => {
                     let name = if *i == 0 { "first" } else { "last" };
                     *e = Expr::Column(Arc::from(name));
                 }
                 Some(idx) => {
-                    let (name, _dtype) = schema.get_index(idx).unwrap();
+                    let (name, _dtype) = schema.get_at_index(idx).unwrap();
                     *e = Expr::Column(Arc::from(&**name))
                 }
             }
             true
         }
         _ => true,
     })
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/pyarrow.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/logical_plan/schema.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/logical_plan/schema.rs`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             #[cfg(feature = "parquet")]
             ParquetScan { file_info, .. } => Ok(Cow::Borrowed(&file_info.schema)),
             #[cfg(feature = "ipc")]
             IpcScan { file_info, .. } => Ok(Cow::Borrowed(&file_info.schema)),
             DataFrameScan { schema, .. } => Ok(Cow::Borrowed(schema)),
             AnonymousScan { file_info, .. } => Ok(Cow::Borrowed(&file_info.schema)),
             Selection { input, .. } => input.schema(),
-            #[cfg(feature = "csv-file")]
+            #[cfg(feature = "csv")]
             CsvScan { file_info, .. } => Ok(Cow::Borrowed(&file_info.schema)),
             Projection { schema, .. } => Ok(Cow::Borrowed(schema)),
             LocalProjection { schema, .. } => Ok(Cow::Borrowed(schema)),
             Aggregate { schema, .. } => Ok(Cow::Borrowed(schema)),
             Join { schema, .. } => Ok(Cow::Borrowed(schema)),
             HStack { schema, .. } => Ok(Cow::Borrowed(schema)),
             Distinct { input, .. } | FileSink { input, .. } => input.schema(),
@@ -185,15 +185,15 @@
                 unreachable!()
             }
         }
         DataFrameScan { df, .. } => {
             let len = df.height();
             (Some(len), len, _filter_count)
         }
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         CsvScan { file_info, .. } => {
             let (known_size, estimated_size) = file_info.row_estimation;
             (known_size, estimated_size, _filter_count)
         }
         #[cfg(feature = "ipc")]
         IpcScan { file_info, .. } => {
             let (known_size, estimated_size) = file_info.row_estimation;
```

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/prelude.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/prelude.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/local_dependencies/polars-plan/src/utils.rs` & `polars_lts_cpu-0.17.6/local_dependencies/polars-plan/src/utils.rs`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             _ => panic!("cannot push more than 1 node"),
         }
     }
 }
 
 pub(crate) fn is_scan(plan: &ALogicalPlan) -> bool {
     match plan {
-        #[cfg(feature = "csv-file")]
+        #[cfg(feature = "csv")]
         ALogicalPlan::CsvScan { .. } => true,
         ALogicalPlan::DataFrameScan { .. } => true,
         #[cfg(feature = "parquet")]
         ALogicalPlan::ParquetScan { .. } => true,
         _ => false,
     }
 }
@@ -310,18 +310,17 @@
 /// Take a list of expressions and a schema and determine the output schema.
 pub fn expressions_to_schema(
     expr: &[Expr],
     schema: &Schema,
     ctxt: Context,
 ) -> PolarsResult<Schema> {
     let mut expr_arena = Arena::with_capacity(4 * expr.len());
-    let fields = expr
-        .iter()
-        .map(|expr| expr.to_field_amortized(schema, ctxt, &mut expr_arena));
-    Schema::try_from_fallible(fields)
+    expr.iter()
+        .map(|expr| expr.to_field_amortized(schema, ctxt, &mut expr_arena))
+        .collect()
 }
 
 pub fn aexpr_to_leaf_names_iter(
     node: Node,
     arena: &Arena<AExpr>,
 ) -> impl Iterator<Item = Arc<str>> + '_ {
     aexpr_to_leaf_nodes_iter(node, arena).map(|node| match arena.get(node) {
@@ -353,18 +352,17 @@
 
 pub(crate) fn aexprs_to_schema(
     expr: &[Node],
     schema: &Schema,
     ctxt: Context,
     arena: &Arena<AExpr>,
 ) -> Schema {
-    let fields = expr
-        .iter()
-        .map(|expr| arena.get(*expr).to_field(schema, ctxt, arena).unwrap());
-    Schema::from(fields)
+    expr.iter()
+        .map(|expr| arena.get(*expr).to_field(schema, ctxt, arena).unwrap())
+        .collect()
 }
 
 pub fn combine_predicates_expr<I>(iter: I) -> Expr
 where
     I: Iterator<Item = Expr>,
 {
     let mut single_pred = None;
```

### Comparing `polars_lts_cpu-0.17.5/Cargo.toml` & `polars_lts_cpu-0.17.6/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "py-polars"
-version = "0.17.5"
+version = "0.17.6"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [workspace]
 # prevents package from thinking it's in the workspace
 [target.'cfg(any(not(target_os = "linux"), use_mimalloc))'.dependencies]
@@ -47,15 +47,15 @@
 # also includes simd
 nightly = ["polars/nightly"]
 streaming = ["polars/streaming"]
 meta = ["polars/meta"]
 search_sorted = ["polars/search_sorted"]
 decompress = ["polars/decompress"]
 lazy_regex = ["polars/lazy_regex"]
-csv-file = ["polars/csv-file"]
+csv = ["polars/csv"]
 object = ["polars/object"]
 extract_jsonpath = ["polars/extract_jsonpath"]
 pivot = ["polars/pivot"]
 top_k = ["polars/top_k"]
 propagate_nans = ["polars/propagate_nans"]
 sql = ["polars/sql"]
 build_info = ["dep:pyo3-built", "dep:built"]
@@ -80,15 +80,15 @@
   "cross_join",
   "pct_change",
   "search_sorted",
   "merge_sorted",
   "meta",
   "decompress",
   "lazy_regex",
-  "csv-file",
+  "csv",
   "extract_jsonpath",
   "timezones",
   "object",
   "pivot",
   "top_k",
   "build_info",
   "cse",
```

### Comparing `polars_lts_cpu-0.17.5/LICENSE` & `polars_lts_cpu-0.17.6/LICENSE`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/Makefile` & `polars_lts_cpu-0.17.6/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/README.md` & `polars_lts_cpu-0.17.6/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,33 +15,40 @@
   </a>
   <a href="https://pypi.org/project/polars/">
     <img src="https://img.shields.io/pypi/v/polars.svg" alt="PyPi Latest Release"/>
   </a>
   <a href="https://www.npmjs.com/package/nodejs-polars">
     <img src="https://img.shields.io/npm/v/nodejs-polars.svg" alt="NPM Latest Release"/>
   </a>
+  <a href="https://rpolars.r-universe.dev">
+    <img src="https://rpolars.r-universe.dev/badges/polars" alt="R-universe Latest Release"/>
+  </a>
   <a href="https://doi.org/10.5281/zenodo.7697217">
     <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7697217.svg" alt="DOI Latest Release"/>
   </a>
 </div>
 
 <p align="center">
   <b>Documentation</b>:
   <a href="https://pola-rs.github.io/polars/py-polars/html/reference/index.html">Python</a>
   -
   <a href="https://pola-rs.github.io/polars/polars/index.html">Rust</a>
   -
   <a href="https://pola-rs.github.io/nodejs-polars/index.html">Node.js</a>
+  -
+  <a href="https://rpolars.github.io/index.html">R</a>
   |
   <b>StackOverflow</b>:
   <a href="https://stackoverflow.com/questions/tagged/python-polars">Python</a>
   -
   <a href="https://stackoverflow.com/questions/tagged/rust-polars">Rust</a>
   -
   <a href="https://stackoverflow.com/questions/tagged/nodejs-polars">Node.js</a>
+  -
+  <a href="https://stackoverflow.com/questions/tagged/r-polars">R</a>
   |
   <a href="https://pola-rs.github.io/polars-book/">User Guide</a>
   |
   <a href="https://discord.gg/4UfP5cfBE7">Discord</a>
 </p>
 
 ## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL
@@ -51,15 +58,15 @@
 
 - Lazy | eager execution
 - Multi-threaded
 - SIMD
 - Query optimization
 - Powerful expression API
 - Hybrid Streaming (larger than RAM datasets)
-- Rust | Python | NodeJS | ...
+- Rust | Python | NodeJS | R | ...
 
 To learn more, read the [User Guide](https://pola-rs.github.io/polars-book/).
 
 ## Python
 
 ```python
 >>> import polars as pl
@@ -130,20 +137,37 @@
 >>> (lf.join(other_table)
 ...      .groupby("foo")
 ...      .agg(
 ...     pl.col("sum_v1").count()
 ... ).collect())
 ```
 
+SQL commands can also be ran directly from your terminal.
+
+```bash
+> cargo install polars-cli --locked
+# run an inline sql query
+> polars -c "SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE id1 = 'id016' LIMIT 10"
+
+# run interactively
+> polars
+Polars CLI v0.1.0
+Type .help for help.
+
+> SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE id1 = 'id016' LIMIT 10;
+```
+
+Refer to [polars-cli](./polars-cli/README.md) for more information.
+
 ## Performance 🚀🚀
 
 ### Blazingly fast
 
 Polars is very fast. In fact, it is one of the best performing solutions available.
-See the results in [h2oai's db-benchmark](https://h2oai.github.io/db-benchmark/).
+See the results in [DuckDB's db-benchmark](https://duckdblabs.github.io/db-benchmark/).
 
 In the [TPCH benchmarks](https://www.pola.rs/benchmarks.html) polars is orders of magnitudes faster than pandas, dask, modin and vaex
 on full queries (including IO).
 
 ### Lightweight
 
 Polars is also very lightweight. It comes with zero required dependencies, and this shows in the import times:
```

#### html2text {}

```diff
@@ -1,22 +1,23 @@
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
-           Latest_Release] [NPM_Latest_Release] [DOI_Latest_Release]
-Documentation: Python - Rust - Node.js | StackOverflow: Python - Rust - Node.js
-                            | User_Guide | Discord
+ Latest_Release] [NPM_Latest_Release] [R-universe_Latest_Release] [DOI_Latest
+                                   Release]
+  Documentation: Python - Rust - Node.js - R | StackOverflow: Python - Rust -
+                      Node.js - R | User_Guide | Discord
 ## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL Polars
 is a DataFrame interface on top of an OLAP Query Engine implemented in Rust
 using [Apache Arrow Columnar Format](https://arrow.apache.org/docs/format/
 Columnar.html) as the memory model. - Lazy | eager execution - Multi-threaded -
 SIMD - Query optimization - Powerful expression API - Hybrid Streaming (larger
-than RAM datasets) - Rust | Python | NodeJS | ... To learn more, read the [User
-Guide](https://pola-rs.github.io/polars-book/). ## Python ```python >>> import
-polars as pl >>> df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ...
+than RAM datasets) - Rust | Python | NodeJS | R | ... To learn more, read the
+[User Guide](https://pola-rs.github.io/polars-book/). ## Python ```python >>>
+import polars as pl >>> df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ...
 "fruits": ["banana", "banana", "apple", "apple", "banana"], ... "B": [5, 4, 3,
 2, 1], ... "cars": ["beetle", "audi", "beetle", "beetle", "beetle"], ... } ...
 ) # embarrassingly parallel execution & very expressive query language >>>
 df.sort("fruits").select( ... "fruits", ... "cars", ... pl.lit("fruits").alias
 ("literal_string_fruits"), ... pl.col("B").filter(pl.col("cars") ==
 "beetle").sum(), ... pl.col("A").filter(pl.col("B") > 2).sum().over
 ("cars").alias("sum_A_by_cars"), ... pl.col("A").sum().over("fruits").alias
@@ -44,48 +45,55 @@
 materialization >>> context.query(query) shape: (1, 2)
 ââââââââââ¬âââââââââ â sum_v1 â min_v2
 â â --- â --- â â i64 â i64 â
 ââââââââââªâââââââââ¡ â 298268 â 1 â
 ââââââââââ´âââââââââ >>> ## OPTION 2 >>> #
 Don't materialize the query, but return as LazyFrame >>> # and continue in
 python >>> lf = context.execute(query) >>> (lf.join(other_table) ... .groupby
-("foo") ... .agg( ... pl.col("sum_v1").count() ... ).collect()) ``` ##
-Performance ðð ### Blazingly fast Polars is very fast. In fact, it is one
-of the best performing solutions available. See the results in [h2oai's db-
-benchmark](https://h2oai.github.io/db-benchmark/). In the [TPCH benchmarks]
-(https://www.pola.rs/benchmarks.html) polars is orders of magnitudes faster
-than pandas, dask, modin and vaex on full queries (including IO). ###
-Lightweight Polars is also very lightweight. It comes with zero required
-dependencies, and this shows in the import times: - polars: 70ms - numpy: 104ms
-- pandas: 520ms ### Handles larger than RAM data If you have data that does not
-fit into memory, polars lazy is able to process your query (or parts of your
-query) in a streaming fashion, this drastically reduces memory requirements so
-you might be able to process your 250GB dataset on your laptop. Collect with
-`collect(streaming=True)` to run the query streaming. (This might be a little
-slower, but it is still very fast!) ## Setup ### Python Install the latest
-polars version with: ```sh pip install polars ``` We also have a conda package
-(`conda install -c conda-forge polars`), however pip is the preferred way to
-install Polars. Install Polars with all optional dependencies. ```sh pip
-install 'polars[all]' pip install 'polars[numpy,pandas,pyarrow]' # install a
-subset of all optional dependencies ``` You can also install the dependencies
-directly. | Tag | Description | | ---------- | --------------------------------
--------------------------------------------------------------------------------
----------------------- | | all | Install all optional dependencies (all of the
-following) | | pandas | Install with Pandas for converting data to and from
-Pandas Dataframes/Series | | numpy | Install with numpy for converting data to
-and from numpy arrays | | pyarrow | Reading data formats using PyArrow | |
-fsspec | Support for reading from remote file systems | | connectorx | Support
-for reading from SQL databases | | xlsx2csv | Support for reading from Excel
-files | | deltalake | Support for reading from Delta Lake Tables | | timezone |
-Timezone support, only needed if 1. you are on Python < 3.9 and/or 2. you are
-on Windows, otherwise no dependencies will be installed | Releases happen quite
-often (weekly / every few days) at the moment, so updating polars regularly to
-get the latest bugfixes / features might not be a bad idea. ### Rust You can
-take latest release from `crates.io`, or if you want to use the latest features
-/ performance improvements point to the `main` branch of this repo. ```toml
+("foo") ... .agg( ... pl.col("sum_v1").count() ... ).collect()) ``` SQL
+commands can also be ran directly from your terminal. ```bash > cargo install
+polars-cli --locked # run an inline sql query > polars -c "SELECT sum(v1) as
+sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE id1 = 'id016' LIMIT
+10" # run interactively > polars Polars CLI v0.1.0 Type .help for help. >
+SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE
+id1 = 'id016' LIMIT 10; ``` Refer to [polars-cli](./polars-cli/README.md) for
+more information. ## Performance ðð ### Blazingly fast Polars is very
+fast. In fact, it is one of the best performing solutions available. See the
+results in [DuckDB's db-benchmark](https://duckdblabs.github.io/db-benchmark/).
+In the [TPCH benchmarks](https://www.pola.rs/benchmarks.html) polars is orders
+of magnitudes faster than pandas, dask, modin and vaex on full queries
+(including IO). ### Lightweight Polars is also very lightweight. It comes with
+zero required dependencies, and this shows in the import times: - polars: 70ms
+- numpy: 104ms - pandas: 520ms ### Handles larger than RAM data If you have
+data that does not fit into memory, polars lazy is able to process your query
+(or parts of your query) in a streaming fashion, this drastically reduces
+memory requirements so you might be able to process your 250GB dataset on your
+laptop. Collect with `collect(streaming=True)` to run the query streaming.
+(This might be a little slower, but it is still very fast!) ## Setup ### Python
+Install the latest polars version with: ```sh pip install polars ``` We also
+have a conda package (`conda install -c conda-forge polars`), however pip is
+the preferred way to install Polars. Install Polars with all optional
+dependencies. ```sh pip install 'polars[all]' pip install 'polars
+[numpy,pandas,pyarrow]' # install a subset of all optional dependencies ``` You
+can also install the dependencies directly. | Tag | Description | | ---------
+- | ---------------------------------------------------------------------------
+---------------------------------------------------------- | | all | Install
+all optional dependencies (all of the following) | | pandas | Install with
+Pandas for converting data to and from Pandas Dataframes/Series | | numpy |
+Install with numpy for converting data to and from numpy arrays | | pyarrow |
+Reading data formats using PyArrow | | fsspec | Support for reading from remote
+file systems | | connectorx | Support for reading from SQL databases | |
+xlsx2csv | Support for reading from Excel files | | deltalake | Support for
+reading from Delta Lake Tables | | timezone | Timezone support, only needed if
+1. you are on Python < 3.9 and/or 2. you are on Windows, otherwise no
+dependencies will be installed | Releases happen quite often (weekly / every
+few days) at the moment, so updating polars regularly to get the latest
+bugfixes / features might not be a bad idea. ### Rust You can take latest
+release from `crates.io`, or if you want to use the latest features /
+performance improvements point to the `main` branch of this repo. ```toml
 polars = { git = "https://github.com/pola-rs/polars", rev = "" } ``` Required
 Rust version `>=1.62` ## Contributing Want to contribute? Read our
 [contribution guideline](./CONTRIBUTING.md). ## Python: compile polars from
 source If you want a bleeding edge release or maximal performance you should
 compile **polars** from source. This can be done by going through the following
 steps in sequence: 1. Install the latest [Rust compiler](https://www.rust-
 lang.org/tools/install) 2. Install [maturin](https://maturin.rs/): `pip install
```

### Comparing `polars_lts_cpu-0.17.5/build.rs` & `polars_lts_cpu-0.17.6/build.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/Makefile` & `polars_lts_cpu-0.17.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/_templates/autosummary/class.rst` & `polars_lts_cpu-0.17.6/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/_static/css/custom.css` & `polars_lts_cpu-0.17.6/docs/source/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/conf.py` & `polars_lts_cpu-0.17.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/api.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/api.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/dataframe/modify_select.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/dataframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/datatypes.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/datatypes.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/computation.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/functions.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/list.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/modify_select.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/operators.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/operators.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/string.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/expressions/temporal.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/expressions/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/functions.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/functions.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/io.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/io.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/lazyframe/modify_select.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/lazyframe/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/series/computation.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/series/computation.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/series/descriptive.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/series/descriptive.rst`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     Series.is_duplicated
     Series.is_empty
     Series.is_finite
     Series.is_first
     Series.is_float
     Series.is_in
     Series.is_infinite
+    Series.is_integer
     Series.is_nan
     Series.is_not_nan
     Series.is_not_null
     Series.is_null
     Series.is_numeric
     Series.is_sorted
     Series.is_temporal
```

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/series/list.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/series/list.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/series/modify_select.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/series/modify_select.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/series/string.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/series/string.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/series/temporal.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/series/temporal.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/docs/source/reference/testing.rst` & `polars_lts_cpu-0.17.6/docs/source/reference/testing.rst`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/__init__.py` & `polars_lts_cpu-0.17.6/polars/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/api.py` & `polars_lts_cpu-0.17.6/polars/api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/config.py` & `polars_lts_cpu-0.17.6/polars/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import contextlib
 import os
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from polars.dependencies import json
 
 
 # dummy func required (so docs build)
 def _get_float_fmt() -> str:
     return "n/a"
@@ -68,29 +68,73 @@
 
     >>> with pl.Config() as cfg:
     ...     # set verbose for more detailed output within the scope
     ...     cfg.set_verbose(True)  # doctest: +IGNORE_RESULT
     ...
     >>> # scope exit - no longer in verbose mode
 
+    This can also be written more compactly as:
+
+    >>> with pl.Config(verbose=True):
+    ...     pass
+    ...
+
+    (The compact format is available for all `Config` methods that take a single value).
+
     """
 
+    _original_state: str = ""
+
+    def __init__(self, **options: Any) -> None:
+        """
+        Initialise a Config object instance for context manager usage.
+
+        Any `options` kwargs should correspond to the available named "set_"
+        methods, but can optionally to omit the "set_" prefix for brevity.
+
+        Parameters
+        ----------
+        options
+            keyword args that will set the option; equivalent to calling the
+            named "set_<option>" method with the given value.
+
+        Examples
+        --------
+        >>> with pl.Config(
+        ...     # these options will be set for scope duration
+        ...     tbl_formatting="ASCII_MARKDOWN",
+        ...     tbl_width_chars=180,
+        ... ):
+        ...     pass
+
+        """
+        # save original state _before_ any changes are made
+        self._original_state = self.save()
+
+        for opt, value in options.items():
+            if not hasattr(self, opt) and not opt.startswith("set_"):
+                opt = f"set_{opt}"
+            if not hasattr(self, opt):
+                raise AttributeError(f"Config has no {opt!r} option")
+            getattr(self, opt)(value)
+
     def __enter__(self) -> Config:
         """Support setting temporary Config options that are reset on scope exit."""
-        self._original_state = self.save()
+        self._original_state = self._original_state or self.save()
         return self
 
     def __exit__(
         self,
         exc_type: type[BaseException] | None,
         exc_val: BaseException | None,
         exc_tb: TracebackType | None,
     ) -> None:
         """Reset any Config options that were set within the scope."""
         self.restore_defaults().load(self._original_state)
+        self._original_state = ""
 
     @classmethod
     def load(cls, cfg: str) -> type[Config]:
         """
         Load and set previously saved (or shared) Config options.
 
         Parameters
@@ -340,40 +384,42 @@
         Parameters
         ----------
         n : int
             number of columns to display; if ``n < 0`` (eg: -1), display all columns.
 
         Examples
         --------
+        Set number of displayed columns to a low value:
+
         >>> with pl.Config() as cfg:
-        ...     cfg.set_tbl_cols(5)  # doctest: +IGNORE_RESULT
+        ...     cfg.set_tbl_cols(5)
         ...     df = pl.DataFrame({str(i): [i] for i in range(100)})
-        ...     df
+        ...     print(df)
         ...
+        <class 'polars.config.Config'>
         shape: (1, 100)
-        ┌─────┬─────┬─────┬─────┬─────┬─────┐
-        │ 0   ┆ 1   ┆ 2   ┆ ... ┆ 98  ┆ 99  │
-        │ --- ┆ --- ┆ --- ┆     ┆ --- ┆ --- │
-        │ i64 ┆ i64 ┆ i64 ┆     ┆ i64 ┆ i64 │
-        ╞═════╪═════╪═════╪═════╪═════╪═════╡
-        │ 0   ┆ 1   ┆ 2   ┆ ... ┆ 98  ┆ 99  │
-        └─────┴─────┴─────┴─────┴─────┴─────┘
+        ┌─────┬─────┬─────┬───┬─────┬─────┐
+        │ 0   ┆ 1   ┆ 2   ┆ … ┆ 98  ┆ 99  │
+        │ --- ┆ --- ┆ --- ┆   ┆ --- ┆ --- │
+        │ i64 ┆ i64 ┆ i64 ┆   ┆ i64 ┆ i64 │
+        ╞═════╪═════╪═════╪═══╪═════╪═════╡
+        │ 0   ┆ 1   ┆ 2   ┆ … ┆ 98  ┆ 99  │
+        └─────┴─────┴─────┴───┴─────┴─────┘
 
-        >>> with pl.Config() as cfg:
-        ...     cfg.set_tbl_cols(10)  # doctest: +IGNORE_RESULT
-        ...     df
+        >>> with pl.Config(tbl_cols=10):
+        ...     print(df)
         ...
         shape: (1, 100)
-        ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
-        │ 0   ┆ 1   ┆ 2   ┆ 3   ┆ 4   ┆ ... ┆ 95  ┆ 96  ┆ 97  ┆ 98  ┆ 99  │
-        │ --- ┆ --- ┆ --- ┆ --- ┆ --- ┆     ┆ --- ┆ --- ┆ --- ┆ --- ┆ --- │
-        │ i64 ┆ i64 ┆ i64 ┆ i64 ┆ i64 ┆     ┆ i64 ┆ i64 ┆ i64 ┆ i64 ┆ i64 │
-        ╞═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╡
-        │ 0   ┆ 1   ┆ 2   ┆ 3   ┆ 4   ┆ ... ┆ 95  ┆ 96  ┆ 97  ┆ 98  ┆ 99  │
-        └─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┘
+        ┌─────┬─────┬─────┬─────┬─────┬───┬─────┬─────┬─────┬─────┬─────┐
+        │ 0   ┆ 1   ┆ 2   ┆ 3   ┆ 4   ┆ … ┆ 95  ┆ 96  ┆ 97  ┆ 98  ┆ 99  │
+        │ --- ┆ --- ┆ --- ┆ --- ┆ --- ┆   ┆ --- ┆ --- ┆ --- ┆ --- ┆ --- │
+        │ i64 ┆ i64 ┆ i64 ┆ i64 ┆ i64 ┆   ┆ i64 ┆ i64 ┆ i64 ┆ i64 ┆ i64 │
+        ╞═════╪═════╪═════╪═════╪═════╪═══╪═════╪═════╪═════╪═════╪═════╡
+        │ 0   ┆ 1   ┆ 2   ┆ 3   ┆ 4   ┆ … ┆ 95  ┆ 96  ┆ 97  ┆ 98  ┆ 99  │
+        └─────┴─────┴─────┴─────┴─────┴───┴─────┴─────┴─────┴─────┴─────┘
 
         """
         os.environ["POLARS_FMT_MAX_COLS"] = str(n)
         return cls
 
     @classmethod
     def set_tbl_column_data_type_inline(cls, active: bool = True) -> type[Config]:
@@ -607,26 +653,27 @@
             rows (DataFrame) and all elements (Series).
 
         Examples
         --------
         >>> df = pl.DataFrame(
         ...     {"abc": [1.0, 2.5, 3.5, 5.0], "xyz": [True, False, True, False]}
         ... )
-        >>> pl.Config.set_tbl_rows(2)  # doctest: +SKIP
-        # ...
-        # shape: (4, 2)
-        # ┌─────┬───────┐
-        # │ abc ┆ xyz   │
-        # │ --- ┆ ---   │
-        # │ f64 ┆ bool  │
-        # ╞═════╪═══════╡
-        # │ 1.0 ┆ true  │
-        # │ …   ┆ …     │
-        # │ 5.0 ┆ false │
-        # └─────┴───────┘
+        >>> with pl.Config(tbl_rows=2):
+        ...     print(df)
+        ...
+        shape: (4, 2)
+        ┌─────┬───────┐
+        │ abc ┆ xyz   │
+        │ --- ┆ ---   │
+        │ f64 ┆ bool  │
+        ╞═════╪═══════╡
+        │ 1.0 ┆ true  │
+        │ …   ┆ …     │
+        │ 5.0 ┆ false │
+        └─────┴───────┘
 
         """
         os.environ["POLARS_FMT_MAX_ROWS"] = str(n)
         return cls
 
     @classmethod
     def set_tbl_width_chars(cls, width: int) -> type[Config]:
```

### Comparing `polars_lts_cpu-0.17.5/polars/convert.py` & `polars_lts_cpu-0.17.6/polars/convert.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/dataframe/_html.py` & `polars_lts_cpu-0.17.6/polars/dataframe/_html.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/dataframe/frame.py` & `polars_lts_cpu-0.17.6/polars/dataframe/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from polars import internals as pli
 from polars.dataframe._html import NotebookFormatter
 from polars.dataframe.groupby import DynamicGroupBy, GroupBy, RollingGroupBy
 from polars.datatypes import (
     FLOAT_DTYPES,
     INTEGER_DTYPES,
     N_INFER_DEFAULT,
+    SIGNED_INTEGER_DTYPES,
     Boolean,
     Categorical,
     DataTypeClass,
     Float64,
     Int8,
     Int16,
     Int32,
@@ -43,14 +44,15 @@
     Object,
     UInt8,
     UInt16,
     UInt32,
     UInt64,
     Utf8,
     py_type_to_dtype,
+    unpack_dtypes,
 )
 from polars.dependencies import (
     _PYARROW_AVAILABLE,
     _check_for_numpy,
     _check_for_pandas,
     _check_for_pyarrow,
 )
@@ -1421,15 +1423,15 @@
                                 "Index positions should be smaller than 2^32."
                             )
                     if idxs.dtype == Int64:
                         if idxs.min() < -(2**32):  # type: ignore[operator]
                             raise ValueError(
                                 "Index positions should be bigger than -2^32 + 1."
                             )
-                if idxs.dtype in {Int8, Int16, Int32, Int64}:
+                if idxs.dtype in SIGNED_INTEGER_DTYPES:
                     if idxs.min() < 0:  # type: ignore[operator]
                         if idx_type == UInt32:
                             if idxs.dtype in {Int8, Int16}:
                                 idxs = idxs.cast(Int32)
                         else:
                             if idxs.dtype in {Int8, Int16, Int32}:
                                 idxs = idxs.cast(Int64)
@@ -1484,45 +1486,43 @@
             | tuple[int, MultiColSelector]
             | tuple[MultiRowSelector, MultiColSelector]
         ),
     ) -> Self:
         ...
 
     @overload
-    def __getitem__(self, item: tuple[MultiRowSelector, int]) -> Series:
+    def __getitem__(self, item: tuple[int, int | str]) -> Any:
         ...
 
     @overload
-    def __getitem__(self, item: tuple[MultiRowSelector, str]) -> Series:
-        ...
-
-    @overload
-    def __getitem__(self, item: tuple[int, int]) -> Any:
-        ...
-
-    @overload
-    def __getitem__(self, item: tuple[int, str]) -> Any:
+    def __getitem__(self, item: tuple[MultiRowSelector, int | str]) -> Series:
         ...
 
     def __getitem__(
         self,
         item: (
             str
             | int
             | np.ndarray[Any, Any]
             | MultiColSelector
             | tuple[int, MultiColSelector]
             | tuple[MultiRowSelector, MultiColSelector]
-            | tuple[MultiRowSelector, int]
-            | tuple[MultiRowSelector, str]
-            | tuple[int, int]
-            | tuple[int, str]
+            | tuple[MultiRowSelector, int | str]
+            | tuple[int, int | str]
         ),
     ) -> DataFrame | Series:
         """Get item. Does quite a lot. Read the comments."""
+        # fail on ['col1', 'col2', ..., 'coln']
+        if (
+            isinstance(item, tuple)
+            and len(item) > 1
+            and all(isinstance(x, str) for x in item)
+        ):
+            raise KeyError(item)
+
         # select rows and columns at once
         # every 2d selection, i.e. tuple is row column order, just like numpy
         if isinstance(item, tuple) and len(item) == 2:
             row_selection, col_selection = item
 
             # df[:, unknown]
             if isinstance(row_selection, slice):
@@ -1645,17 +1645,17 @@
         elif is_int_sequence(item):
             item = pli.Series("", item)  # fall through to next if isinstance
 
         if isinstance(item, pli.Series):
             dtype = item.dtype
             if dtype == Utf8:
                 return self._from_pydf(self._df.select(item))
-            if dtype == UInt32:
+            elif dtype == UInt32:
                 return self._from_pydf(self._df.take_with_series(item._s))
-            if dtype in {UInt8, UInt16, UInt64, Int8, Int16, Int32, Int64}:
+            elif dtype in INTEGER_DTYPES:
                 return self._from_pydf(
                     self._df.take_with_series(self._pos_idxs(item, dim=0)._s)
                 )
 
         # if no data has been returned, the operation is not supported
         raise ValueError(
             f"Cannot __getitem__ on DataFrame with item: '{item}'"
@@ -1765,43 +1765,57 @@
                 self,
                 max_cols=max_cols,
                 max_rows=max_rows,
                 from_series=from_series,
             ).render()
         )
 
-    def item(self) -> Any:
+    def item(self, row: int | None = None, column: int | str | None = None) -> Any:
         """
-        Return the dataframe as a scalar.
+        Return the dataframe as a scalar, or return the element at the given row/column.
 
-        Equivalent to ``df[0,0]``, with a check that the shape is (1,1).
+        Notes
+        -----
+        If row/col not provided, this is equivalent to ``df[0,0]``, with a check that
+        the shape is (1,1). With row/col, this is equivalent to ``df[row,col]``.
+
+        Parameters
+        ----------
+        row
+            Optional row index.
+        column
+            Optional column index or name.
 
         Examples
         --------
         >>> df = pl.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6]})
-        >>> result = df.select((pl.col("a") * pl.col("b")).sum())
-        >>> result
-        shape: (1, 1)
-        ┌─────┐
-        │ a   │
-        │ --- │
-        │ i64 │
-        ╞═════╡
-        │ 32  │
-        └─────┘
-        >>> result.item()
+        >>> df.select((pl.col("a") * pl.col("b")).sum()).item()
         32
+        >>> df.item(1, 1)
+        5
+        >>> df.item(2, "b")
+        6
+
+        See Also
+        --------
+        row: Get the values of a single row, either by index or by predicate.
 
         """
-        if self.shape != (1, 1):
-            raise ValueError(
-                f"Can only call .item() if the dataframe is of shape (1,1), "
-                f"dataframe is of shape {self.shape}"
-            )
-        return self[0, 0]
+        if row is None and column is None:
+            if self.shape != (1, 1):
+                raise ValueError(
+                    f"Can only call '.item()' if the dataframe is of shape (1,1), or if "
+                    f"explicit row/col values are provided; frame has shape {self.shape}"
+                )
+            return self[0, 0]
+
+        elif row is None or column is None:
+            raise ValueError("Cannot call '.item()' with only one of 'row' or 'column'")
+
+        return self[row, column]
 
     def to_arrow(self) -> pa.Table:
         """
         Collect the underlying arrow arrays in an Arrow Table.
 
         This operation is mostly zero copy.
 
@@ -3647,15 +3661,15 @@
             columns = []
             for i, s in enumerate(self.columns):
                 if self[s].is_numeric() or self[s].is_boolean():
                     columns.append(stat[:, i].cast(float))
                 else:
                     # for dates, strings, etc, we cast to string so that all
                     # statistics can be shown
-                    columns.append(stat[:, i].cast(str))
+                    columns.append(stat[:, i].cast(str, strict=False))
             return self.__class__(columns)
 
         # Build output rows
         output_rows = [
             describe_cast(self.__class__({c: [len(self)] for c in self.columns})),
             describe_cast(self.null_count()),
             describe_cast(self.mean()),
@@ -6091,14 +6105,15 @@
         │ str ┆ i64 ┆ i64 ┆ i64 │
         ╞═════╪═════╪═════╪═════╡
         │ one ┆ 1   ┆ 2   ┆ 3   │
         │ two ┆ 4   ┆ 5   ┆ 6   │
         └─────┴─────┴─────┴─────┘
 
         Run an expression as aggregation function
+
         >>> df = pl.DataFrame(
         ...     {
         ...         "col1": ["a", "a", "a", "b", "b", "b"],
         ...         "col2": ["x", "x", "x", "x", "y", "y"],
         ...         "col3": [6, 7, 3, 2, 5, 7],
         ...     }
         ... )
@@ -6821,16 +6836,15 @@
         │ 0         │
         │ 10        │
         └───────────┘
 
         Expressions with multiple outputs can be automatically instantiated as Structs
         by enabling the experimental setting ``Config.set_auto_structify(True)``:
 
-        >>> with pl.Config() as cfg:
-        ...     cfg.set_auto_structify(True)  # doctest: +IGNORE_RESULT
+        >>> with pl.Config(auto_structify=True):
         ...     df.select(
         ...         is_odd=(pl.col(pl.INTEGER_DTYPES) % 2).suffix("_is_odd"),
         ...     )
         ...
         shape: (3, 1)
         ┌───────────┐
         │ is_odd    │
@@ -6977,16 +6991,15 @@
         │ 3   ┆ 10.0 ┆ false ┆ 30.0 ┆ true  │
         │ 4   ┆ 13.0 ┆ true  ┆ 52.0 ┆ false │
         └─────┴──────┴───────┴──────┴───────┘
 
         Expressions with multiple outputs can be automatically instantiated as Structs
         by enabling the experimental setting ``Config.set_auto_structify(True)``:
 
-        >>> with pl.Config() as cfg:
-        ...     cfg.set_auto_structify(True)  # doctest: +IGNORE_RESULT
+        >>> with pl.Config(auto_structify=True):
         ...     df.drop("c").with_columns(
         ...         diffs=pl.col(["a", "b"]).diff().suffix("_diff"),
         ...     )
         ...
         shape: (4, 3)
         ┌─────┬──────┬─────────────┐
         │ a   ┆ b    ┆ diffs       │
@@ -7905,16 +7918,16 @@
 
         When using ``by_predicate`` it is an error condition if anything other than
         one row is returned; more than one row raises ``TooManyRowsReturnedError``, and
         zero rows will raise ``NoRowsReturnedError`` (both inherit from ``RowsError``).
 
         Warnings
         --------
-        You should NEVER use this method to iterate over a DataFrame; if you absolutely
-        require row-iteration you should strongly prefer ``iter_rows()`` instead.
+        You should NEVER use this method to iterate over a DataFrame; if you require
+        row-iteration you should strongly prefer use of ``iter_rows()`` instead.
 
         Examples
         --------
         Specify an index to return the row at the given index as a tuple.
 
         >>> df = pl.DataFrame(
         ...     {
@@ -7937,14 +7950,15 @@
         >>> df.row(by_predicate=(pl.col("ham") == "b"))
         (2, 7, 'b')
 
         See Also
         --------
         iter_rows : Row iterator over frame data (does not materialise all rows).
         rows : Materialises all frame data as a list of rows.
+        item: Return dataframe element as a scalar.
 
         """
         if index is not None and by_predicate is not None:
             raise ValueError(
                 "Cannot set both 'index' and 'by_predicate'; mutually exclusive"
             )
         elif isinstance(index, pli.Expr):
@@ -8116,15 +8130,16 @@
         # to ".row(i)", so it should only be disabled in extremely specific cases.
         if buffer_size and not has_object:
             load_pyarrow_dicts = (
                 named
                 and _PYARROW_AVAILABLE
                 # note: 'ns' precision instantiates values as pandas types - avoid
                 and not any(
-                    (getattr(tp, "time_unit", None) == "ns") for tp in self.dtypes
+                    (getattr(tp, "time_unit", None) == "ns")
+                    for tp in unpack_dtypes(self.dtypes)
                 )
             )
             for offset in range(0, self.height, buffer_size):
                 zerocopy_slice = self.slice(offset, buffer_size)
                 if load_pyarrow_dicts:
                     yield from zerocopy_slice.to_arrow().to_pylist()
                 else:
```

### Comparing `polars_lts_cpu-0.17.5/polars/dataframe/groupby.py` & `polars_lts_cpu-0.17.6/polars/dataframe/groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/datatypes/__init__.py` & `polars_lts_cpu-0.17.6/polars/datatypes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     dtype_to_py_type,
     is_polars_dtype,
     maybe_cast,
     numpy_char_code_to_dtype,
     py_type_to_arrow_type,
     py_type_to_dtype,
     supported_numpy_char_code,
+    unpack_dtypes,
 )
 from polars.type_aliases import (
     OneOrMoreDataTypes,
     PolarsDataType,
     PolarsTemporalType,
     PythonDataType,
     SchemaDefinition,
@@ -124,14 +125,15 @@
     "dtype_to_py_type",
     "is_polars_dtype",
     "maybe_cast",
     "numpy_char_code_to_dtype",
     "py_type_to_arrow_type",
     "py_type_to_dtype",
     "supported_numpy_char_code",
+    "unpack_dtypes",
     # type_aliases
     "OneOrMoreDataTypes",
     "PolarsDataType",
     "PolarsTemporalType",
     "PythonDataType",
     "SchemaDefinition",
     "SchemaDict",
```

### Comparing `polars_lts_cpu-0.17.5/polars/datatypes/classes.py` & `polars_lts_cpu-0.17.6/polars/datatypes/classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import contextlib
+from datetime import timezone
 from inspect import isclass
 from typing import TYPE_CHECKING, Any, Iterator, Mapping, Sequence
 
 import polars.datatypes
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import dtype_str_repr as _dtype_str_repr
@@ -162,15 +163,15 @@
             return True
         elif isinstance(other, Decimal):
             return self.precision == other.precision and self.scale == other.scale
         else:
             return False
 
     def __hash__(self) -> int:
-        return hash((Decimal, self.precision, self.scale))
+        return hash((self.__class__, self.precision, self.scale))
 
 
 class Boolean(DataType):
     """Boolean type."""
 
 
 class Utf8(DataType):
@@ -191,27 +192,32 @@
 
 class Datetime(TemporalType):
     """Calendar date and time type."""
 
     time_unit: TimeUnit | None = None
     time_zone: str | None = None
 
-    def __init__(self, time_unit: TimeUnit | None = "us", time_zone: str | None = None):
+    def __init__(
+        self, time_unit: TimeUnit | None = "us", time_zone: str | timezone | None = None
+    ):
         """
         Calendar date and time type.
 
         Parameters
         ----------
         time_unit : {'us', 'ns', 'ms'}
             Unit of time.
         time_zone
             Time zone string as defined in zoneinfo (run
             ``import zoneinfo; zoneinfo.available_timezones()`` for a full list).
 
         """
+        if isinstance(time_zone, timezone):
+            time_zone = str(time_zone)
+
         self.time_unit = time_unit or "us"
         self.time_zone = time_zone
 
         if self.time_unit not in ("ms", "us", "ns"):
             raise ValueError(
                 f"Invalid time_unit; expected one of {{'ns','us','ms'}}, got {self.time_unit!r}"
             )
@@ -224,15 +230,15 @@
             return (
                 self.time_unit == other.time_unit and self.time_zone == other.time_zone
             )
         else:
             return False
 
     def __hash__(self) -> int:
-        return hash((Datetime, self.time_unit))
+        return hash((self.__class__, self.time_unit, self.time_zone))
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         return (
             f"{class_name}(time_unit={self.time_unit!r}, time_zone={self.time_zone!r})"
         )
 
@@ -264,15 +270,15 @@
             return True
         elif isinstance(other, Duration):
             return self.time_unit == other.time_unit
         else:
             return False
 
     def __hash__(self) -> int:
-        return hash((Duration, self.time_unit))
+        return hash((self.__class__, self.time_unit))
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}(time_unit={self.time_unit!r})"
 
 
 class Categorical(DataType):
@@ -324,15 +330,15 @@
                 return True
             else:
                 return self.inner == other.inner
         else:
             return False
 
     def __hash__(self) -> int:
-        return hash((List, self.inner))
+        return hash((self.__class__, self.inner))
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}({self.inner!r})"
 
 
 class Field:
@@ -350,14 +356,17 @@
         """
         self.name = name
         self.dtype = polars.datatypes.py_type_to_dtype(dtype)
 
     def __eq__(self, other: Field) -> bool:  # type: ignore[override]
         return (self.name == other.name) & (self.dtype == other.dtype)
 
+    def __hash__(self) -> int:
+        return hash((self.name, self.dtype))
+
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
         return f"{class_name}({self.name!r}, {self.dtype})"
 
 
 class Struct(NestedType):
     def __init__(self, fields: Sequence[Field] | SchemaDict):
@@ -386,15 +395,15 @@
             return any((f is None) for f in (self.fields, other.fields)) or (
                 self.fields == other.fields
             )
         else:
             return False
 
     def __hash__(self) -> int:
-        return hash(Struct)
+        return hash((self.__class__, tuple(self.fields)))
 
     def __iter__(self) -> Iterator[tuple[str, PolarsDataType]]:
         for fld in self.fields or []:
             yield fld.name, fld.dtype
 
     def __repr__(self) -> str:
         class_name = self.__class__.__name__
```

### Comparing `polars_lts_cpu-0.17.5/polars/datatypes/constants.py` & `polars_lts_cpu-0.17.6/polars/datatypes/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,21 +23,23 @@
 if TYPE_CHECKING:
     from polars.type_aliases import PolarsDataType, TimeUnit
 
 DTYPE_TEMPORAL_UNITS: frozenset[TimeUnit] = frozenset(["ns", "us", "ms"])
 DATETIME_DTYPES: frozenset[PolarsDataType] = frozenset(
     [
         # TODO: ideally need a mechanism to wildcard timezones here too
+        Datetime,
         Datetime("ms"),
         Datetime("us"),
         Datetime("ns"),
     ]
 )
 DURATION_DTYPES: frozenset[PolarsDataType] = frozenset(
     [
+        Duration,
         Duration("ms"),
         Duration("us"),
         Duration("ns"),
     ]
 )
 TEMPORAL_DTYPES: frozenset[PolarsDataType] = (
     frozenset([Date, Time]) | DATETIME_DTYPES | DURATION_DTYPES
```

### Comparing `polars_lts_cpu-0.17.5/polars/datatypes/constructor.py` & `polars_lts_cpu-0.17.6/polars/datatypes/constructor.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/datatypes/convert.py` & `polars_lts_cpu-0.17.6/polars/datatypes/convert.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,31 +7,37 @@
 import sys
 from datetime import date, datetime, time, timedelta
 from decimal import Decimal as PyDecimal
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
+    Collection,
     ForwardRef,
     Optional,
     TypeVar,
     Union,
+    cast,
     overload,
 )
+from typing import (
+    List as TypingList,
+)
 
 from polars.datatypes import (
     Binary,
     Boolean,
     Categorical,
     DataType,
     DataTypeClass,
     Date,
     Datetime,
     Decimal,
     Duration,
+    Field,
     Float32,
     Float64,
     Int8,
     Int16,
     Int32,
     Int64,
     List,
@@ -44,14 +50,15 @@
     UInt32,
     UInt64,
     Unknown,
     Utf8,
 )
 from polars.dependencies import numpy as np
 from polars.dependencies import pyarrow as pa
+from polars.type_aliases import PolarsDataType
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import dtype_str_repr as _dtype_str_repr
 
 if sys.version_info >= (3, 8):
     from typing import get_args
 else:
@@ -66,15 +73,15 @@
     from types import NoneType, UnionType
 else:
     # infer equivalent class
     NoneType = type(None)
     UnionType = type(Union[int, float])
 
 if TYPE_CHECKING:
-    from polars.type_aliases import PolarsDataType, PythonDataType, SchemaDict, TimeUnit
+    from polars.type_aliases import PythonDataType, SchemaDict, TimeUnit
 
     if sys.version_info >= (3, 8):
         from typing import Literal
     else:
         from typing_extensions import Literal
 
 
@@ -136,26 +143,83 @@
     if python_dtype is object:
         return Object
     if python_dtype is None.__class__:
         return Null
     raise TypeError("Invalid type")
 
 
-def is_polars_dtype(data_type: Any, include_unknown: bool = False) -> bool:
+def is_polars_dtype(dtype: Any, include_unknown: bool = False) -> bool:
     """Indicate whether the given input is a Polars dtype, or dtype specialisation."""
     try:
-        if data_type == Unknown:
+        if dtype == Unknown:
             # does not represent a realisable dtype, so ignore by default
             return include_unknown
         else:
-            return isinstance(data_type, (DataType, DataTypeClass))
+            return isinstance(dtype, (DataType, DataTypeClass))
     except ValueError:
         return False
 
 
+def unpack_dtypes(
+    dtypes: PolarsDataType | Collection[PolarsDataType] | None,
+    include_compound: bool = False,
+) -> set[PolarsDataType]:
+    """
+    Return a set of unique dtypes found in one or more (potentially compound) dtypes.
+
+    Parameters
+    ----------
+    dtypes : PolarsDataType | Collection[PolarsDataType] | None
+        polars dtype, collection of dtypes, or None.
+
+    include_compound : bool, default True
+        * if True, any parent/compound dtypes (List, Struct) are included in the result.
+        * if False, only the child/scalar dtypes are returned from these types.
+
+    Examples
+    --------
+    >>> from polars.datatypes import unpack_dtypes
+    >>> list_dtype = [pl.List(pl.Float64)]
+    >>> struct_dtype = pl.Struct(
+    ...     [
+    ...         pl.Field("a", pl.Int64),
+    ...         pl.Field("b", pl.Utf8),
+    ...         pl.Field("c", pl.List(pl.Float64)),
+    ...     ]
+    ... )
+    >>> unpack_dtypes([struct_dtype, list_dtype])  # doctest: +IGNORE_RESULT
+    {Float64, Int64, Utf8}
+    >>> unpack_dtypes(
+    ...     [struct_dtype, list_dtype], include_compound=True
+    ... )  # doctest: +IGNORE_RESULT
+    {Float64, Int64, Utf8, List(Float64), Struct([Field('a', Int64), Field('b', Utf8), Field('c', List(Float64))])}
+
+    """  # noqa: W505
+    if not dtypes:
+        return set()
+    elif is_polars_dtype(dtypes):
+        dtypes = [dtypes]  # type: ignore[list-item]
+
+    unpacked: set[PolarsDataType] = set()
+    for tp in cast(TypingList[PolarsDataType], dtypes):
+        if isinstance(tp, List):
+            if include_compound:
+                unpacked.add(tp)
+            unpacked.update(unpack_dtypes(tp.inner, include_compound=include_compound))
+        elif isinstance(tp, Struct):
+            if include_compound:
+                unpacked.add(tp)
+            unpacked.update(unpack_dtypes(tp.fields, include_compound=include_compound))  # type: ignore[arg-type]
+        elif isinstance(tp, Field):
+            unpacked.update(unpack_dtypes(tp.dtype, include_compound=include_compound))
+        elif is_polars_dtype(tp):
+            unpacked.add(tp)
+    return unpacked
+
+
 class _DataTypeMappings:
     @property
     @cache
     def DTYPE_TO_FFINAME(self) -> dict[PolarsDataType, str]:
         return {
             Int8: "i8",
             Int16: "i16",
```

### Comparing `polars_lts_cpu-0.17.5/polars/dependencies.py` & `polars_lts_cpu-0.17.6/polars/dependencies.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/exceptions.py` & `polars_lts_cpu-0.17.6/polars/exceptions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/expr/binary.py` & `polars_lts_cpu-0.17.6/polars/expr/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/expr/categorical.py` & `polars_lts_cpu-0.17.6/polars/expr/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/expr/datetime.py` & `polars_lts_cpu-0.17.6/polars/expr/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/expr/expr.py` & `polars_lts_cpu-0.17.6/polars/expr/expr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import annotations
 
 import contextlib
 import math
 import operator
 import os
 import random
-import warnings
 from datetime import timedelta
 from functools import partial, reduce
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Collection,
@@ -43,15 +42,15 @@
 from polars.expr.meta import ExprMetaNameSpace
 from polars.expr.string import ExprStringNameSpace
 from polars.expr.struct import ExprStructNameSpace
 from polars.utils._parse_expr_input import expr_to_lit_or_expr, selection_to_pyexpr_list
 from polars.utils.convert import _timedelta_to_pl_duration
 from polars.utils.decorators import deprecated_alias, redirect
 from polars.utils.meta import threadpool_size
-from polars.utils.various import find_stacklevel, sphinx_accessor
+from polars.utils.various import sphinx_accessor
 
 with contextlib.suppress(ImportError):  # Module not available when building docs
     from polars.polars import arg_where as py_arg_where
     from polars.polars import reduce as pyreduce
 if TYPE_CHECKING:
     import sys
 
@@ -3439,40 +3438,29 @@
 
     def explode(self) -> Self:
         """
         Explode a list or utf8 Series.
 
         This means that every item is expanded to a new row.
 
-        .. deprecated:: 0.15.16
-            `Expr.explode` will be removed in favour of `Expr.arr.explode` and
-            `Expr.str.explode`.
-
         Returns
         -------
         Exploded Series of same dtype
 
         See Also
         --------
         ExprListNameSpace.explode : Explode a list column.
         ExprStringNameSpace.explode : Explode a string column.
 
         """
-        warnings.warn(
-            "`Series/Expr.explode()` is deprecated in favor of the identical method"
-            " under the list and string namespaces. Use `.arr.explode()` or"
-            " `.str.explode()` instead.",
-            DeprecationWarning,
-            stacklevel=find_stacklevel(),
-        )
         return self._from_pyexpr(self._pyexpr.explode())
 
     def implode(self) -> Self:
         """
-        Aggregate all column values into a list.
+        Aggregate values into a list.
 
         Examples
         --------
         >>> df = pl.DataFrame(
         ...     {
         ...         "a": [1, 2, 3],
         ...         "b": [4, 5, 6],
@@ -7475,14 +7463,17 @@
 
 
 def _prepare_rolling_window_args(
     window_size: int | timedelta | str,
     min_periods: int | None = None,
 ) -> tuple[str, int]:
     if isinstance(window_size, int):
+        if window_size < 1:
+            raise ValueError("'window_size' should be positive")
+
         if min_periods is None:
             min_periods = window_size
         window_size = f"{window_size}i"
     elif isinstance(window_size, timedelta):
         window_size = _timedelta_to_pl_duration(window_size)
     if min_periods is None:
         min_periods = 1
```

### Comparing `polars_lts_cpu-0.17.5/polars/expr/list.py` & `polars_lts_cpu-0.17.6/polars/expr/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/expr/meta.py` & `polars_lts_cpu-0.17.6/polars/expr/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/expr/string.py` & `polars_lts_cpu-0.17.6/polars/expr/string.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,18 +59,18 @@
         exact
             - If True, require an exact format match.
             - If False, allow the format to match anywhere in the target string.
         cache
             Use a cache of unique, converted dates to apply the datetime conversion.
         tz_aware
             Parse timezone aware datetimes. This may be automatically toggled by the
-            `fmt` given.
+            `format` given.
 
             .. deprecated:: 0.16.17
-                This is now auto-inferred from the given `fmt`. You can safely drop
+                This is now auto-inferred from the given `format`. You can safely drop
                 this argument, it will be removed in a future version.
         utc
             Parse timezone aware datetimes as UTC. This may be useful if you have data
             with mixed offsets.
 
         Notes
         -----
@@ -118,15 +118,15 @@
         │ 2021-04-22 │
         │ 2022-01-04 │
         │ 2022-01-31 │
         │ 2001-07-08 │
         └────────────┘
 
         """
-        if not is_polars_dtype(dtype):  # pragma: no cover
+        if not is_polars_dtype(dtype):
             raise ValueError(f"expected: {DataType} got: {dtype}")
 
         if format is not None and "%f" in format:
             raise ValueError(
                 "Directive '%f' is not supported in Python Polars, "
                 "as it differs from the Python standard library.\n"
                 "Instead, please use one of:\n"
@@ -143,34 +143,34 @@
                 "`tz_aware` is now auto-inferred from `format` and will be removed "
                 "in a future version. You can safely drop this argument.",
                 category=DeprecationWarning,
                 stacklevel=find_stacklevel(),
             )
 
         if dtype == Date:
-            return wrap_expr(self._pyexpr.str_parse_date(format, strict, exact, cache))
+            return wrap_expr(self._pyexpr.str_to_date(format, strict, exact, cache))
         elif dtype == Datetime:
             time_unit = dtype.time_unit  # type: ignore[union-attr]
             time_zone = dtype.time_zone  # type: ignore[union-attr]
             dtcol = wrap_expr(
-                self._pyexpr.str_parse_datetime(
+                self._pyexpr.str_to_datetime(
                     format,
+                    time_unit,
+                    time_zone,
                     strict,
                     exact,
                     cache,
                     tz_aware,
                     utc,
-                    time_unit,
-                    time_zone,
                 )
             )
             return dtcol if (time_unit is None) else dtcol.dt.cast_time_unit(time_unit)
         elif dtype == Time:
-            return wrap_expr(self._pyexpr.str_parse_time(format, strict, exact, cache))
-        else:  # pragma: no cover
+            return wrap_expr(self._pyexpr.str_to_time(format, strict, exact, cache))
+        else:
             raise ValueError("dtype should be of type {Date, Datetime, Time}")
 
     def lengths(self) -> Expr:
         """
         Get length of the strings as UInt32 (as number of bytes).
 
         Notes
```

### Comparing `polars_lts_cpu-0.17.5/polars/expr/struct.py` & `polars_lts_cpu-0.17.6/polars/expr/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/functions/__init__.py` & `polars_lts_cpu-0.17.6/polars/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/functions/eager.py` & `polars_lts_cpu-0.17.6/polars/functions/eager.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/functions/lazy.py` & `polars_lts_cpu-0.17.6/polars/functions/lazy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1243,14 +1243,22 @@
     >>> pl.lit(pl.Series("x", [1, 2, 3]))  # doctest: +IGNORE_RESULT
 
     Literal list/Series data (2D):
 
     >>> pl.lit([[1, 2], [3, 4]])  # doctest: +IGNORE_RESULT
     >>> pl.lit(pl.Series("y", [[1, 2], [3, 4]]))  # doctest: +IGNORE_RESULT
 
+    Expected datatypes
+
+    - ''pl.lit([])'' -> empty  Series Float32
+    - ''pl.lit([1, 2, 3])'' -> Series Int64
+    - ''pl.lit([[]])''-> empty  Series List<Null>
+    - ''pl.lit([[1, 2, 3]])'' -> Series List<i64>
+    - ''pl.lit(None)'' -> Series Null
+
     """
     time_unit: TimeUnit
 
     if isinstance(value, datetime):
         time_unit = "us" if dtype is None else getattr(dtype, "time_unit", "us")
         time_zone = (
             value.tzinfo
@@ -2440,41 +2448,46 @@
     Expr of type `pl.Duration`
 
     Examples
     --------
     >>> from datetime import datetime
     >>> df = pl.DataFrame(
     ...     {
-    ...         "datetime": [datetime(2022, 1, 1), datetime(2022, 1, 2)],
+    ...         "dt": [datetime(2022, 1, 1), datetime(2022, 1, 2)],
     ...         "add": [1, 2],
     ...     }
     ... )
-    >>> df.select(
-    ...     [
-    ...         (pl.col("datetime") + pl.duration(weeks="add")).alias("add_weeks"),
-    ...         (pl.col("datetime") + pl.duration(days="add")).alias("add_days"),
-    ...         (pl.col("datetime") + pl.duration(seconds="add")).alias("add_seconds"),
-    ...         (pl.col("datetime") + pl.duration(milliseconds="add")).alias(
-    ...             "add_milliseconds"
-    ...         ),
-    ...         (pl.col("datetime") + pl.duration(hours="add")).alias("add_hours"),
-    ...     ]
-    ... )  # doctest: +IGNORE_RESULT
+    >>> print(df)
+    shape: (2, 2)
+    ┌─────────────────────┬─────┐
+    │ dt                  ┆ add │
+    │ ---                 ┆ --- │
+    │ datetime[μs]        ┆ i64 │
+    ╞═════════════════════╪═════╡
+    │ 2022-01-01 00:00:00 ┆ 1   │
+    │ 2022-01-02 00:00:00 ┆ 2   │
+    └─────────────────────┴─────┘
+    >>> with pl.Config(tbl_width_chars=120):
+    ...     df.select(
+    ...         (pl.col("dt") + pl.duration(weeks="add")).alias("add_weeks"),
+    ...         (pl.col("dt") + pl.duration(days="add")).alias("add_days"),
+    ...         (pl.col("dt") + pl.duration(seconds="add")).alias("add_seconds"),
+    ...         (pl.col("dt") + pl.duration(milliseconds="add")).alias("add_millis"),
+    ...         (pl.col("dt") + pl.duration(hours="add")).alias("add_hours"),
+    ...     )
+    ...
     shape: (2, 5)
-    ┌────────────┬────────────┬─────────────────────┬──────────────┬─────────────────────┐
-    │ add_weeks  ┆ add_days   ┆ add_seconds         ┆ add_millisec ┆ add_hours           │
-    │ ---        ┆ ---        ┆ ---                 ┆ onds         ┆ ---                 │
-    │ datetime[m ┆ datetime[m ┆ datetime[ms]        ┆ ---          ┆ datetime[ms]        │
-    │ s]         ┆ s]         ┆                     ┆ datetime[ms] ┆                     │
-    ╞════════════╪════════════╪═════════════════════╪══════════════╪═════════════════════╡
-    │ 2022-01-08 ┆ 2022-01-02 ┆ 2022-01-01 00:00:01 ┆ 2022-01-01   ┆ 2022-01-01 01:00:00 │
-    │ 00:00:00   ┆ 00:00:00   ┆                     ┆ 00:00:00.001 ┆                     │
-    │ 2022-01-16 ┆ 2022-01-04 ┆ 2022-01-02 00:00:02 ┆ 2022-01-02   ┆ 2022-01-02 02:00:00 │
-    │ 00:00:00   ┆ 00:00:00   ┆                     ┆ 00:00:00.002 ┆                     │
-    └────────────┴────────────┴─────────────────────┴──────────────┴─────────────────────┘
+    ┌─────────────────────┬─────────────────────┬─────────────────────┬─────────────────────────┬─────────────────────┐
+    │ add_weeks           ┆ add_days            ┆ add_seconds         ┆ add_millis              ┆ add_hours           │
+    │ ---                 ┆ ---                 ┆ ---                 ┆ ---                     ┆ ---                 │
+    │ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]        ┆ datetime[μs]            ┆ datetime[μs]        │
+    ╞═════════════════════╪═════════════════════╪═════════════════════╪═════════════════════════╪═════════════════════╡
+    │ 2022-01-08 00:00:00 ┆ 2022-01-02 00:00:00 ┆ 2022-01-01 00:00:01 ┆ 2022-01-01 00:00:00.001 ┆ 2022-01-01 01:00:00 │
+    │ 2022-01-16 00:00:00 ┆ 2022-01-04 00:00:00 ┆ 2022-01-02 00:00:02 ┆ 2022-01-02 00:00:00.002 ┆ 2022-01-02 02:00:00 │
+    └─────────────────────┴─────────────────────┴─────────────────────┴─────────────────────────┴─────────────────────┘
 
     """  # noqa: W505
     if hours is not None:
         hours = expr_to_lit_or_expr(hours, str_to_lit=False)._pyexpr
     if minutes is not None:
         minutes = expr_to_lit_or_expr(minutes, str_to_lit=False)._pyexpr
     if seconds is not None:
@@ -2972,15 +2985,15 @@
         exprs.extend(
             expr_to_lit_or_expr(expr, name=name, str_to_lit=False)._pyexpr
             for name, expr in named_exprs.items()
         )
 
     expr = wrap_expr(_as_struct(exprs))
     if schema:
-        expr = expr.cast(Struct(schema))
+        expr = expr.cast(Struct(schema), strict=False)
 
     if eager:
         return select(expr).to_series()
     else:
         return expr
```

### Comparing `polars_lts_cpu-0.17.5/polars/functions/whenthen.py` & `polars_lts_cpu-0.17.6/polars/functions/whenthen.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/__init__.py` & `polars_lts_cpu-0.17.6/polars/io/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/_utils.py` & `polars_lts_cpu-0.17.6/polars/io/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/avro.py` & `polars_lts_cpu-0.17.6/polars/io/avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/csv/_utils.py` & `polars_lts_cpu-0.17.6/polars/io/csv/_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/csv/batched_reader.py` & `polars_lts_cpu-0.17.6/polars/io/csv/batched_reader.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/csv/functions.py` & `polars_lts_cpu-0.17.6/polars/io/csv/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/database.py` & `polars_lts_cpu-0.17.6/polars/io/database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/delta.py` & `polars_lts_cpu-0.17.6/polars/io/delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/excel/_write_utils.py` & `polars_lts_cpu-0.17.6/polars/io/excel/_write_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/excel/functions.py` & `polars_lts_cpu-0.17.6/polars/io/excel/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from io import StringIO
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, BinaryIO, overload
+from typing import TYPE_CHECKING, Any, BinaryIO, NoReturn, overload
 
 from polars.io.csv.functions import read_csv
 from polars.utils.various import normalise_filepath
 
 if TYPE_CHECKING:
     import sys
     from io import BytesIO
@@ -19,50 +19,76 @@
         from typing_extensions import Literal
 
 
 @overload
 def read_excel(
     source: str | BytesIO | Path | BinaryIO | bytes,
     *,
-    sheet_id: Literal[None],
-    sheet_name: Literal[None],
-    xlsx2csv_options: dict[str, Any] | None,
-    read_csv_options: dict[str, Any] | None,
-) -> dict[str, DataFrame]:
+    sheet_id: None = ...,
+    sheet_name: str,
+    xlsx2csv_options: dict[str, Any] | None = ...,
+    read_csv_options: dict[str, Any] | None = ...,
+) -> DataFrame:
     ...
 
 
 @overload
 def read_excel(
     source: str | BytesIO | Path | BinaryIO | bytes,
     *,
-    sheet_id: Literal[None],
-    sheet_name: str,
-    xlsx2csv_options: dict[str, Any] | None = None,
-    read_csv_options: dict[str, Any] | None = None,
+    sheet_id: None = ...,
+    sheet_name: None = ...,
+    xlsx2csv_options: dict[str, Any] | None = ...,
+    read_csv_options: dict[str, Any] | None = ...,
 ) -> DataFrame:
     ...
 
 
 @overload
 def read_excel(
     source: str | BytesIO | Path | BinaryIO | bytes,
     *,
     sheet_id: int,
-    sheet_name: Literal[None],
-    xlsx2csv_options: dict[str, Any] | None = None,
-    read_csv_options: dict[str, Any] | None = None,
+    sheet_name: str,
+    xlsx2csv_options: dict[str, Any] | None = ...,
+    read_csv_options: dict[str, Any] | None = ...,
+) -> NoReturn:
+    ...
+
+
+# mypy wants the return value for Literal[0] to
+# overlap with the return value for other integers.
+@overload  # type: ignore[misc]
+def read_excel(
+    source: str | BytesIO | Path | BinaryIO | bytes,
+    *,
+    sheet_id: Literal[0],
+    sheet_name: None = ...,
+    xlsx2csv_options: dict[str, Any] | None = ...,
+    read_csv_options: dict[str, Any] | None = ...,
+) -> dict[str, DataFrame]:
+    ...
+
+
+@overload
+def read_excel(
+    source: str | BytesIO | Path | BinaryIO | bytes,
+    *,
+    sheet_id: int,
+    sheet_name: None = ...,
+    xlsx2csv_options: dict[str, Any] | None = ...,
+    read_csv_options: dict[str, Any] | None = ...,
 ) -> DataFrame:
     ...
 
 
 def read_excel(
     source: str | BytesIO | Path | BinaryIO | bytes,
     *,
-    sheet_id: int | None = 1,
+    sheet_id: int | None = None,
     sheet_name: str | None = None,
     xlsx2csv_options: dict[str, Any] | None = None,
     read_csv_options: dict[str, Any] | None = None,
 ) -> DataFrame | dict[str, DataFrame]:
     """
     Read Excel (XLSX) sheet into a DataFrame.
 
@@ -72,17 +98,18 @@
     Parameters
     ----------
     source
         Path to a file or a file-like object.
         By file-like object, we refer to objects with a ``read()`` method, such as a
         file handler (e.g. via builtin ``open`` function) or ``BytesIO``.
     sheet_id
-        Sheet number to convert (0 for all sheets).
+        Sheet number to convert (``0`` for all sheets). Defaults to `1` if neither this
+        nor `sheet_name` are specified.
     sheet_name
-        Sheet name to convert.
+        Sheet name to convert. Cannot be used in conjunction with `sheet_id`.
     xlsx2csv_options
         Extra options passed to ``xlsx2csv.Xlsx2csv()``.
         e.g.: ``{"skip_empty_lines": True}``
     read_csv_options
         Extra options passed to :func:`read_csv` for parsing the CSV file returned by
         ``xlsx2csv.Xlsx2csv().convert()``
         e.g.: ``{"has_header": False, "new_columns": ["a", "b", "c"],
@@ -146,23 +173,29 @@
 
     if not read_csv_options:
         read_csv_options = {}
 
     # Convert sheets from XSLX document to CSV.
     parser = xlsx2csv.Xlsx2csv(source, **xlsx2csv_options)
 
-    if (sheet_name is not None) or ((sheet_id is not None) and (sheet_id > 0)):
-        return _read_excel_sheet(parser, sheet_id, sheet_name, read_csv_options)
-    else:
+    if sheet_name is None and sheet_id is None:
+        return _read_excel_sheet(parser, 1, None, read_csv_options)
+    elif sheet_name is None and ((sheet_id is not None) and (sheet_id > 0)):
+        return _read_excel_sheet(parser, sheet_id, None, read_csv_options)
+    elif sheet_name is None and ((sheet_id is not None) and (sheet_id == 0)):
         return {
             sheet["name"]: _read_excel_sheet(
                 parser, sheet["index"], None, read_csv_options
             )
             for sheet in parser.workbook.sheets
         }
+    elif sheet_name is not None and sheet_id is None:
+        return _read_excel_sheet(parser, None, sheet_name, read_csv_options)
+    else:
+        raise ValueError("Cannot specify both `sheet_name` and `sheet_id`")
 
 
 def _read_excel_sheet(
     parser: Any,
     sheet_id: int | None,
     sheet_name: str | None,
     read_csv_options: dict[str, Any],
```

### Comparing `polars_lts_cpu-0.17.5/polars/io/ipc/anonymous_scan.py` & `polars_lts_cpu-0.17.6/polars/io/ipc/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/ipc/functions.py` & `polars_lts_cpu-0.17.6/polars/io/ipc/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/json.py` & `polars_lts_cpu-0.17.6/polars/io/json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/ndjson.py` & `polars_lts_cpu-0.17.6/polars/io/ndjson.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/parquet/anonymous_scan.py` & `polars_lts_cpu-0.17.6/polars/io/parquet/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/parquet/functions.py` & `polars_lts_cpu-0.17.6/polars/io/parquet/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/pyarrow_dataset/anonymous_scan.py` & `polars_lts_cpu-0.17.6/polars/io/pyarrow_dataset/anonymous_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/io/pyarrow_dataset/functions.py` & `polars_lts_cpu-0.17.6/polars/io/pyarrow_dataset/functions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/lazyframe/frame.py` & `polars_lts_cpu-0.17.6/polars/lazyframe/frame.py`

 * *Files 1% similar despite different names*

```diff
@@ -2116,16 +2116,15 @@
         │ 0         │
         │ 10        │
         └───────────┘
 
         Expressions with multiple outputs can be automatically instantiated as Structs
         by enabling the experimental setting ``Config.set_auto_structify(True)``:
 
-        >>> with pl.Config() as cfg:
-        ...     cfg.set_auto_structify(True)  # doctest: +IGNORE_RESULT
+        >>> with pl.Config(auto_structify=True):
         ...     lf.select(
         ...         is_odd=(pl.col(pl.INTEGER_DTYPES) % 2).suffix("_is_odd"),
         ...     ).collect()
         ...
         shape: (3, 1)
         ┌───────────┐
         │ is_odd    │
@@ -3127,16 +3126,15 @@
         │ 3   ┆ 10.0 ┆ false ┆ 30.0 ┆ true  │
         │ 4   ┆ 13.0 ┆ true  ┆ 52.0 ┆ false │
         └─────┴──────┴───────┴──────┴───────┘
 
         Expressions with multiple outputs can be automatically instantiated as Structs
         by enabling the experimental setting ``Config.set_auto_structify(True)``:
 
-        >>> with pl.Config() as cfg:
-        ...     cfg.set_auto_structify(True)  # doctest: +IGNORE_RESULT
+        >>> with pl.Config(auto_structify=True):
         ...     lf.drop("c").with_columns(
         ...         diffs=pl.col(["a", "b"]).diff().suffix("_diff"),
         ...     ).collect()
         ...
         shape: (4, 3)
         ┌─────┬──────┬─────────────┐
         │ a   ┆ b    ┆ diffs       │
```

### Comparing `polars_lts_cpu-0.17.5/polars/lazyframe/groupby.py` & `polars_lts_cpu-0.17.6/polars/lazyframe/groupby.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,14 +115,18 @@
         ╞═════╪═══════╪════════════════╡
         │ a   ┆ 2     ┆ 17.0           │
         │ c   ┆ 3     ┆ 1.0            │
         │ b   ┆ 5     ┆ 10.0           │
         └─────┴───────┴────────────────┘
 
         """
+        if isinstance(aggs, dict):
+            raise ValueError(
+                f"'aggs' argument should be one or multiple expressions, got: '{aggs}'."
+            )
         if aggs is None and not named_aggs:
             raise ValueError("Expected at least one of 'aggs' or '**named_aggs'")
 
         exprs = selection_to_pyexpr_list(aggs)
         if more_aggs:
             exprs.extend(selection_to_pyexpr_list(more_aggs))
         if named_aggs:
```

### Comparing `polars_lts_cpu-0.17.5/polars/series/_numpy.py` & `polars_lts_cpu-0.17.6/polars/series/_numpy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/binary.py` & `polars_lts_cpu-0.17.6/polars/series/binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/categorical.py` & `polars_lts_cpu-0.17.6/polars/series/categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/datetime.py` & `polars_lts_cpu-0.17.6/polars/series/datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/list.py` & `polars_lts_cpu-0.17.6/polars/series/list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/series.py` & `polars_lts_cpu-0.17.6/polars/series/series.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,33 @@
     Union,
     overload,
 )
 
 from polars import functions as F
 from polars import internals as pli
 from polars.datatypes import (
+    FLOAT_DTYPES,
+    INTEGER_DTYPES,
+    NUMERIC_DTYPES,
+    SIGNED_INTEGER_DTYPES,
+    TEMPORAL_DTYPES,
+    UNSIGNED_INTEGER_DTYPES,
     Boolean,
     Categorical,
     Date,
     Datetime,
     Duration,
     Float32,
     Float64,
     Int8,
     Int16,
     Int32,
     Int64,
     List,
+    Object,
     Time,
     UInt8,
     UInt16,
     UInt32,
     UInt64,
     Unknown,
     Utf8,
@@ -768,15 +775,15 @@
                                 "Index positions should be smaller than 2^32."
                             )
                     if idxs.dtype == Int64:
                         if idxs.min() < -(2**32):  # type: ignore[operator]
                             raise ValueError(
                                 "Index positions should be bigger than -2^32 + 1."
                             )
-                if idxs.dtype in {Int8, Int16, Int32, Int64}:
+                if idxs.dtype in SIGNED_INTEGER_DTYPES:
                     if idxs.min() < 0:  # type: ignore[operator]
                         if idx_type == UInt32:
                             if idxs.dtype in {Int8, Int16}:
                                 idxs = idxs.cast(Int32)
                         else:
                             if idxs.dtype in {Int8, Int16, Int32}:
                                 idxs = idxs.cast(Int64)
@@ -845,24 +852,15 @@
 
     def __getitem__(
         self,
         item: (
             int | Series | range | slice | np.ndarray[Any, Any] | list[int] | list[bool]
         ),
     ) -> Any:
-        if isinstance(item, Series) and item.dtype in {
-            UInt8,
-            UInt16,
-            UInt32,
-            UInt64,
-            Int8,
-            Int16,
-            Int32,
-            Int64,
-        }:
+        if isinstance(item, Series) and item.dtype in INTEGER_DTYPES:
             # Unsigned or signed Series (ordered from fastest to slowest).
             #   - pl.UInt32 (polars) or pl.UInt64 (polars_u64_idx) Series indexes.
             #   - Other unsigned Series indexes are converted to pl.UInt32 (polars)
             #     or pl.UInt64 (polars_u64_idx).
             #   - Signed Series indexes are converted pl.UInt32 (polars) or
             #     pl.UInt64 (polars_u64_idx) after negative indexes are converted
             #     to absolute indexes.
@@ -1030,33 +1028,37 @@
                 f" `{method}`."
             )
 
     def _repr_html_(self) -> str:
         """Format output data in HTML for display in Jupyter Notebooks."""
         return self.to_frame()._repr_html_(from_series=True)
 
-    def item(self) -> Any:
+    def item(self, row: int | None = None) -> Any:
         """
-        Return the series as a scalar.
+        Return the series as a scalar, or return the element at the given row index.
 
-        Equivalent to ``s[0]``, with a check that the shape is (1,).
+        If no row index is provided, this is equivalent to ``s[0]``, with a check
+        that the shape is (1,). With a row index, this is equivalent to ``s[row]``.
 
         Examples
         --------
-        >>> s = pl.Series("a", [1])
-        >>> s.item()
+        >>> s1 = pl.Series("a", [1])
+        >>> s1.item()
         1
+        >>> s2 = pl.Series("a", [9, 8, 7])
+        >>> s2.cumsum().item(-1)
+        24
 
         """
-        if len(self) != 1:
+        if row is None and len(self) != 1:
             raise ValueError(
-                f"Can only call .item() if the series is of length 1, "
-                f"series is of length {len(self)}"
+                f"Can only call '.item()' if the series is of length 1, or an "
+                f"explicit row index is provided (series is of length {len(self)})"
             )
-        return self[0]
+        return self[row or 0]
 
     def estimated_size(self, unit: SizeUnit = "b") -> int | float:
         """
         Return an estimation of the total (heap) allocated size of the Series.
 
         Estimated size is given in the specified unit (bytes by default).
 
@@ -2811,18 +2813,14 @@
 
     def explode(self) -> Series:
         """
         Explode a list or utf8 Series.
 
         This means that every item is expanded to a new row.
 
-        .. deprecated:: 0.15.16
-            `Series.explode` will be removed in favour of `Series.arr.explode` and
-            `Series.str.explode`.
-
         Returns
         -------
         Exploded Series of same dtype
 
         See Also
         --------
         ListNameSpace.explode : Explode a list column.
@@ -3077,26 +3075,46 @@
         Examples
         --------
         >>> s = pl.Series("a", [1, 2, 3])
         >>> s.is_numeric()
         True
 
         """
-        return self.dtype in (
-            Int8,
-            Int16,
-            Int32,
-            Int64,
-            UInt8,
-            UInt16,
-            UInt32,
-            UInt64,
-            Float32,
-            Float64,
-        )
+        return self.dtype in NUMERIC_DTYPES
+
+    def is_integer(self, signed: bool | None = None) -> bool:
+        """
+        Check if this Series datatype is an integer (signed or unsigned).
+
+        Parameters
+        ----------
+        signed
+            * if `None`, both signed and unsigned integer dtypes will match.
+            * if `True`, only signed integer dtypes will be considered a match.
+            * if `False`, only unsigned integer dtypes will be considered a match.
+
+        Examples
+        --------
+        >>> s = pl.Series("a", [1, 2, 3], dtype=pl.UInt32)
+        >>> s.is_integer()
+        True
+        >>> s.is_integer(signed=False)
+        True
+        >>> s.is_integer(signed=True)
+        False
+
+        """
+        if signed is None:
+            return self.dtype in INTEGER_DTYPES
+        elif signed is True:
+            return self.dtype in SIGNED_INTEGER_DTYPES
+        elif signed is False:
+            return self.dtype in UNSIGNED_INTEGER_DTYPES
+
+        raise ValueError(f"'signed' must be None, True or False; given {signed!r}")
 
     def is_temporal(self, excluding: OneOrMoreDataTypes | None = None) -> bool:
         """
         Check if this Series datatype is temporal.
 
         Parameters
         ----------
@@ -3115,28 +3133,28 @@
         """
         if excluding is not None:
             if not isinstance(excluding, Iterable):
                 excluding = [excluding]
             if self.dtype in excluding:
                 return False
 
-        return self.dtype in (Date, Datetime, Duration, Time)
+        return self.dtype in TEMPORAL_DTYPES
 
     def is_float(self) -> bool:
         """
         Check if this Series has floating point numbers.
 
         Examples
         --------
         >>> s = pl.Series("a", [1.0, 2.0, 3.0])
         >>> s.is_float()
         True
 
         """
-        return self.dtype in (Float32, Float64)
+        return self.dtype in FLOAT_DTYPES
 
     def is_boolean(self) -> bool:
         """
         Check if this Series is a Boolean.
 
         Examples
         --------
@@ -3235,15 +3253,20 @@
                 tp = "datetime64[D]"
             elif self.dtype == Duration:
                 tp = f"timedelta64[{self.time_unit}]"
             else:
                 tp = f"datetime64[{self.time_unit}]"
             return arr.astype(tp)
 
-        if use_pyarrow and _PYARROW_AVAILABLE and not self.is_temporal(excluding=Time):
+        if (
+            use_pyarrow
+            and _PYARROW_AVAILABLE
+            and self.dtype != Object
+            and not self.is_temporal(excluding=Time)
+        ):
             return self.to_arrow().to_numpy(
                 *args, zero_copy_only=zero_copy_only, writable=writable
             )
         elif self.dtype == Time:
             # note: there is no native numpy "time" dtype
             return np.array(self.to_list(), dtype="object")
         else:
@@ -5732,14 +5755,17 @@
         This can be used to reduce memory pressure.
         """
 
     def get_chunks(self) -> list[Series]:
         """Get the chunks of this Series as a list of Series."""
         return self._s.get_chunks()
 
+    def implode(self) -> Self:
+        """Aggregate values into a list."""
+
     # Below are the namespaces defined. Do not move these up in the definition of
     # Series, as it confuses mypy between the type annotation `str` and the
     # namespace `str`
     @property
     def arr(self) -> ListNameSpace:
         """Create an object namespace of all list related methods."""
         return ListNameSpace(self)
```

### Comparing `polars_lts_cpu-0.17.5/polars/series/string.py` & `polars_lts_cpu-0.17.6/polars/series/string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/struct.py` & `polars_lts_cpu-0.17.6/polars/series/struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/series/utils.py` & `polars_lts_cpu-0.17.6/polars/series/utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/slice.py` & `polars_lts_cpu-0.17.6/polars/slice.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/sql/context.py` & `polars_lts_cpu-0.17.6/polars/sql/context.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/string_cache.py` & `polars_lts_cpu-0.17.6/polars/string_cache.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/testing/_private.py` & `polars_lts_cpu-0.17.6/polars/testing/_private.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/testing/_tempdir.py` & `polars_lts_cpu-0.17.6/polars/testing/_tempdir.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/testing/asserts.py` & `polars_lts_cpu-0.17.6/polars/testing/asserts.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/testing/parametric/primitives.py` & `polars_lts_cpu-0.17.6/polars/testing/parametric/primitives.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,62 +1,70 @@
 from __future__ import annotations
 
 import random
 import warnings
 from dataclasses import dataclass
 from math import isfinite
 from textwrap import dedent
-from typing import TYPE_CHECKING, Any, Sequence
+from typing import TYPE_CHECKING, Any, Collection, Sequence
 
 from hypothesis.errors import InvalidArgument, NonInteractiveExampleWarning
 from hypothesis.strategies import (
     booleans,
     composite,
     lists,
     sampled_from,
 )
 from hypothesis.strategies._internal.utils import defines_strategy
 
 from polars.dataframe import DataFrame
 from polars.datatypes import (
+    DTYPE_TEMPORAL_UNITS,
     FLOAT_DTYPES,
     Categorical,
+    Datetime,
+    Duration,
+    List,
     is_polars_dtype,
     py_type_to_dtype,
 )
 from polars.series import Series
 from polars.string_cache import StringCache
 from polars.testing.asserts import is_categorical_dtype
 from polars.testing.parametric.strategies import (
     between,
+    create_list_strategy,
     scalar_strategies,
 )
 
 if TYPE_CHECKING:
     from hypothesis.strategies import DrawFn, SearchStrategy
 
     from polars.lazyframe import LazyFrame
     from polars.type_aliases import OneOrMoreDataTypes, PolarsDataType
 
 
+_time_units = list(DTYPE_TEMPORAL_UNITS)
+
+
 def empty_list(value: Any, nested: bool) -> bool:
     """Check if value is an empty list, or a list that contains only empty lists."""
     if isinstance(value, list):
         return True if value and not nested else all(empty_list(v, True) for v in value)
     return False
 
 
 # ====================================================================
 # Polars 'hypothesis' primitives for Series, DataFrame, and LazyFrame
 # See: https://hypothesis.readthedocs.io/
 # ====================================================================
-MAX_DATA_SIZE = 10  # max generated frame length
+MAX_DATA_SIZE = 10  # max generated frame/series length
 MAX_COLS = 8  # max number of generated cols
 
-strategy_dtypes = list(scalar_strategies)
+strategy_dtypes = list({dtype.base_type() for dtype in scalar_strategies})
 
 
 @dataclass
 class column:
     """
     Define a column for use with the @dataframes strategy.
 
@@ -65,17 +73,17 @@
     name : str
         string column name.
     dtype : PolarsDataType
         a recognised polars dtype.
     strategy : strategy, optional
         supports overriding the default strategy for the given dtype.
     null_probability : float, optional
-        percentage chance (expressed between 0.0 => 1.0) that a generated value
-        is None. this is applied in addition to any None values output by the
-        given/inferred strategy for the column.
+        percentage chance (expressed between 0.0 => 1.0) that a generated value is
+        None. this is applied independently of any None values generated by the
+        underlying strategy.
     unique : bool, optional
         flag indicating that all values generated for the column should be unique.
 
     Examples
     --------
     >>> from hypothesis.strategies import sampled_from
     >>> from polars.testing.parametric import column
@@ -105,14 +113,21 @@
             tp = getattr(self.strategy, "_dtype", None)
             if is_polars_dtype(tp):
                 self.dtype = tp
 
         if self.dtype is None and self.strategy is None:
             self.dtype = random.choice(strategy_dtypes)
 
+        elif self.dtype == List:
+            if self.strategy is not None:
+                self.dtype = getattr(self.strategy, "_dtype", self.dtype)
+            else:
+                self.strategy = create_list_strategy(getattr(self.dtype, "inner", None))
+                self.dtype = self.strategy._dtype  # type: ignore[union-attr]
+
         elif self.dtype not in scalar_strategies:
             if self.dtype is not None:
                 raise InvalidArgument(
                     f"No strategy (currently) available for {self.dtype} type"
                 )
             else:
                 # given a custom strategy, but no explicit dtype. infer one
@@ -135,15 +150,17 @@
                             )
                         )
                     except StopIteration:
                         raise InvalidArgument(
                             "Unable to determine dtype for strategy"
                         ) from None
                 if sample_value_type is not None:
-                    self.dtype = py_type_to_dtype(sample_value_type)
+                    value_dtype = py_type_to_dtype(sample_value_type)
+                    if value_dtype is not List:
+                        self.dtype = value_dtype
 
 
 def columns(
     cols: int | Sequence[str] | None = None,
     *,
     dtype: OneOrMoreDataTypes | None = None,
     min_cols: int | None = 0,
@@ -235,29 +252,30 @@
     min_size: int | None = 0,
     max_size: int | None = MAX_DATA_SIZE,
     strategy: SearchStrategy[object] | None = None,
     null_probability: float = 0.0,
     allow_infinities: bool = True,
     unique: bool = False,
     chunked: bool | None = None,
-    allowed_dtypes: Sequence[PolarsDataType] | None = None,
-    excluded_dtypes: Sequence[PolarsDataType] | None = None,
+    allowed_dtypes: Collection[PolarsDataType] | None = None,
+    excluded_dtypes: Collection[PolarsDataType] | None = None,
 ) -> SearchStrategy[Series]:
     """
     Strategy for producing a polars Series.
 
     Parameters
     ----------
     name : {str, strategy}, optional
         literal string or a strategy for strings (or None), passed to the Series
         constructor name-param.
     dtype : PolarsDataType, optional
         a valid polars DataType for the resulting series.
     size : int, optional
-        if set, creates a Series of exactly this size (ignoring min/max params).
+        if set, creates a Series of exactly this size (ignoring min_size/max_size
+        params).
     min_size : int, optional
         if not passing an exact size, can set a minimum here (defaults to 0).
         no-op if `size` is set.
     max_size : int, optional
         if not passing an exact size, can set a maximum value here (defaults to
         MAX_DATA_SIZE). no-op if `size` is set.
     strategy : strategy, optional
@@ -320,18 +338,26 @@
     null_probability = float(null_probability or 0.0)
 
     @composite
     def draw_series(draw: DrawFn) -> Series:
         with StringCache():
             # create/assign series dtype and retrieve matching strategy
             series_dtype = (
-                draw(sampled_from(selectable_dtypes)) if dtype is None else dtype
+                draw(sampled_from(selectable_dtypes))
+                if dtype is None and strategy is None
+                else dtype
             )
             if strategy is None:
-                dtype_strategy = scalar_strategies[series_dtype]
+                if series_dtype is Datetime or series_dtype is Duration:
+                    series_dtype = series_dtype(random.choice(_time_units))  # type: ignore[operator]
+                dtype_strategy = scalar_strategies[
+                    series_dtype
+                    if series_dtype in scalar_strategies
+                    else series_dtype.base_type()  # type: ignore[union-attr]
+                ]
             else:
                 dtype_strategy = strategy
 
             if series_dtype in FLOAT_DTYPES and not allow_infinities:
                 dtype_strategy = dtype_strategy.filter(
                     lambda x: not isinstance(x, float) or isfinite(x)
                 )
@@ -397,16 +423,16 @@
     size: int | None = None,
     min_size: int | None = 0,
     max_size: int | None = MAX_DATA_SIZE,
     chunked: bool | None = None,
     include_cols: Sequence[column] | None = None,
     null_probability: float | dict[str, float] = 0.0,
     allow_infinities: bool = True,
-    allowed_dtypes: Sequence[PolarsDataType] | None = None,
-    excluded_dtypes: Sequence[PolarsDataType] | None = None,
+    allowed_dtypes: Collection[PolarsDataType] | None = None,
+    excluded_dtypes: Collection[PolarsDataType] | None = None,
 ) -> SearchStrategy[DataFrame | LazyFrame]:
     """
     Provides a strategy for producing a DataFrame or LazyFrame.
 
     Parameters
     ----------
     cols : {int, columns}, optional
@@ -416,16 +442,16 @@
         produce a LazyFrame instead of a DataFrame.
     min_cols : int, optional
         if not passing an exact size, can set a minimum here (defaults to 0).
     max_cols : int, optional
         if not passing an exact size, can set a maximum value here (defaults to
         MAX_COLS).
     size : int, optional
-        if set, will create a DataFrame of exactly this size (and ignore min/max len
-        params).
+        if set, will create a DataFrame of exactly this size (and ignore
+        the min_size/max_size len params).
     min_size : int, optional
         if not passing an exact size, set the minimum number of rows in the
         DataFrame.
     max_size : int, optional
         if not passing an exact size, set the maximum number of rows in the
         DataFrame.
     chunked : bool, optional
@@ -562,15 +588,15 @@
                     )
                 )
                 for c in coldefs
             }
 
             # note: randomly change between column-wise and row-wise frame init
             orient = "col"
-            if draw(booleans()):
+            if draw(booleans()) and not any(c.dtype == List for c in coldefs):
                 data = list(zip(*data.values()))  # type: ignore[assignment]
                 orient = "row"
 
             schema = [(c.name, c.dtype) for c in coldefs]
             try:
                 df = DataFrame(data=data, schema=schema, orient=orient)  # type: ignore[arg-type]
 
@@ -580,19 +606,27 @@
                     df = df[:split_at].vstack(df[split_at:])
 
                 _failed_frame_init_msgs_.clear()
                 return df.lazy() if lazy else df
 
             except Exception:
                 # print code that will allow any init failure to be reproduced
+                if isinstance(data, dict):
+                    frame_cols = ", ".join(
+                        f"{col!r}: {s.to_init_repr()}" for col, s in data.items()
+                    )
+                    frame_data = f"{{{frame_cols}}}"
+                else:
+                    frame_data = repr(data)
+
                 failed_frame_init = dedent(
                     f"""
                     # failed frame init: reproduce with...
                     pl.DataFrame(
-                        data={data!r},
+                        data={frame_data},
                         schema={repr(schema).replace("', ","', pl.")},
                         orient={orient!r},
                     )
                     """.replace(
                         "datetime.", ""
                     )
                 )
```

### Comparing `polars_lts_cpu-0.17.5/polars/type_aliases.py` & `polars_lts_cpu-0.17.6/polars/type_aliases.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/__init__.py` & `polars_lts_cpu-0.17.6/polars/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/_construction.py` & `polars_lts_cpu-0.17.6/polars/utils/_construction.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/_parse_expr_input.py` & `polars_lts_cpu-0.17.6/polars/utils/_parse_expr_input.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/_scan.py` & `polars_lts_cpu-0.17.6/polars/utils/_scan.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/_wrap.py` & `polars_lts_cpu-0.17.6/polars/utils/_wrap.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/build_info.py` & `polars_lts_cpu-0.17.6/polars/utils/build_info.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/convert.py` & `polars_lts_cpu-0.17.6/polars/utils/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,24 +127,24 @@
     else:
         raise ValueError(
             f"time_unit must be one of {{'ns', 'us', 'ms'}}, got {time_unit}"
         )
 
 
 def _to_python_time(value: int) -> time:
+    """Convert polars int64 (ns) timestamp to python time object."""
     if value == 0:
         return time(microsecond=0)
-    value = value // 1_000
-    microsecond = value
-    seconds = (microsecond // 1000_000) % 60
-    minutes = (microsecond // (1000_000 * 60)) % 60
-    hours = (microsecond // (1000_000 * 60 * 60)) % 24
-    microsecond = microsecond - (seconds + minutes * 60 + hours * 3600) * 1000_000
-
-    return time(hour=hours, minute=minutes, second=seconds, microsecond=microsecond)
+    else:
+        seconds, nanoseconds = divmod(value, 1_000_000_000)
+        minutes, seconds = divmod(seconds, 60)
+        hours, minutes = divmod(minutes, 60)
+        return time(
+            hour=hours, minute=minutes, second=seconds, microsecond=nanoseconds // 1000
+        )
 
 
 def _to_python_timedelta(value: int | float, time_unit: TimeUnit = "ns") -> timedelta:
     if time_unit == "ns":
         return timedelta(microseconds=value // 1e3)
     elif time_unit == "us":
         return timedelta(microseconds=value)
@@ -153,67 +153,60 @@
     else:
         raise ValueError(
             f"time_unit must be one of {{'ns', 'us', 'ms'}}, got {time_unit}"
         )
 
 
 EPOCH = datetime(1970, 1, 1).replace(tzinfo=None)
+EPOCH_UTC = datetime(1970, 1, 1, tzinfo=timezone.utc)
+
+_fromtimestamp = datetime.fromtimestamp
 
 
 def _to_python_datetime(
     value: int | float,
     dtype: PolarsDataType,
     time_unit: TimeUnit | None = "ns",
     time_zone: str | None = None,
 ) -> date | datetime:
+    """Convert polars int64 timestamp to Python date/datetime."""
     if dtype == Date:
-        # days to seconds
-        # important to create from utc. Not doing this leads
-        # to inconsistencies dependent on the timezone you are in.
-        dt = datetime(1970, 1, 1, tzinfo=timezone.utc)
-        dt += timedelta(seconds=value * 3600 * 24)
-        return dt.date()
+        # important to create from utc; not doing this leads to
+        # inconsistencies dependent on the timezone you are in.
+        return (EPOCH_UTC + timedelta(seconds=value * 86400)).date()
+
     elif dtype == Datetime:
-        if time_zone is None or time_zone == "":
+        if not time_zone:
             if time_unit == "ns":
-                # nanoseconds to seconds
-                dt = EPOCH + timedelta(microseconds=value / 1000)
+                return EPOCH + timedelta(microseconds=value // 1000)
             elif time_unit == "us":
-                dt = EPOCH + timedelta(microseconds=value)
+                return EPOCH + timedelta(microseconds=value)
             elif time_unit == "ms":
-                # milliseconds to seconds
-                dt = datetime.utcfromtimestamp(value / 1000)
+                return EPOCH + timedelta(milliseconds=value)
             else:
                 raise ValueError(
-                    f"time_unit must be one of {{'ns', 'us', 'ms'}}, got {time_unit}"
-                )
-        else:
-            if not _ZONEINFO_AVAILABLE:
-                raise ImportError(
-                    "Install polars[timezone] to handle datetimes with timezones."
+                    f"time_unit must be one of {{'ns','us','ms'}}, got {time_unit}"
                 )
 
-            utc = get_zoneinfo("UTC")
+        elif _ZONEINFO_AVAILABLE:
             if time_unit == "ns":
-                # nanoseconds to seconds
-                dt = datetime.fromtimestamp(0, tz=utc) + timedelta(
-                    microseconds=value / 1000
-                )
+                dt = EPOCH_UTC + timedelta(microseconds=value // 1000)
             elif time_unit == "us":
-                dt = datetime.fromtimestamp(0, tz=utc) + timedelta(microseconds=value)
+                dt = EPOCH_UTC + timedelta(microseconds=value)
             elif time_unit == "ms":
-                # milliseconds to seconds
-                dt = datetime.fromtimestamp(value / 1000, tz=utc)
+                dt = EPOCH_UTC + timedelta(milliseconds=value)
             else:
                 raise ValueError(
-                    f"time_unit must be one of {{'ns', 'us', 'ms'}}, got {time_unit}"
+                    f"time_unit must be one of {{'ns','us','ms'}}, got {time_unit}"
                 )
             return _localize(dt, time_zone)
-
-        return dt
+        else:
+            raise ImportError(
+                "Install polars[timezone] to handle datetimes with timezones."
+            )
     else:
         raise NotImplementedError  # pragma: no cover
 
 
 def _localize(dt: datetime, time_zone: str) -> datetime:
     # zone info installation should already be checked
     _tzinfo: ZoneInfo | tzinfo
```

### Comparing `polars_lts_cpu-0.17.5/polars/utils/decorators.py` & `polars_lts_cpu-0.17.6/polars/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/meta.py` & `polars_lts_cpu-0.17.6/polars/utils/meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/polars_version.py` & `polars_lts_cpu-0.17.6/polars/utils/polars_version.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/show_versions.py` & `polars_lts_cpu-0.17.6/polars/utils/show_versions.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/polars/utils/various.py` & `polars_lts_cpu-0.17.6/polars/utils/various.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/pyproject.toml` & `polars_lts_cpu-0.17.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -139,15 +139,14 @@
   # flake8-pytest-style:
   "PT011", # pytest.raises({exception}) is too broad, set the match parameter or use a more specific exception
   # flake8-simplify
   "SIM102", # Use a single `if` statement instead of nested `if` statements
   # ruff
   "RUF005", # unpack-instead-of-concatenating-to-collection-literal
   # pycodestyle
-  "W191", # Indentation contains tabs - disabled because of https://github.com/charliermarsh/ruff/issues/3438
   # TODO: Remove errors below to further improve docstring linting
   # Ordered from most common to least common errors.
   "D105",
   "D100",
   "D103",
   "D102",
   "D104",
@@ -161,30 +160,35 @@
 ban-relative-imports = "all"
 
 [tool.ruff.flake8-type-checking]
 strict = true
 
 [tool.ruff.per-file-ignores]
 "polars/datatypes.py" = ["B019"]
-"tests/**/*.py" = ["D100", "D103"]
+"tests/**/*.py" = ["D100", "D103", "B018"]
 
 [tool.pytest.ini_options]
 addopts = [
   "--strict-config",
   "--strict-markers",
   "--import-mode=importlib",
   # Default to running fast tests only. To run ALL tests, run: pytest -m ""
   "-m not slow and not hypothesis and not benchmark and not write_disk",
 ]
 markers = [
   "write_disk: Tests that write to disk",
   "slow: Tests with a longer than average runtime.",
   "benchmark: Tests that should be run on a Polars release build.",
 ]
-filterwarnings = "error" # Fail on warnings
+filterwarnings = [
+  # Fail on warnings...
+  "error",
+  # ...except where it prevents test debugging in an IPython console
+  "ignore:.*unrecognized arguments.*PyDevIPCompleter:DeprecationWarning",
+]
 xfail_strict = true
 
 [tool.coverage.run]
 source = ["polars"]
 branch = true
 
 [tool.coverage.report]
```

### Comparing `polars_lts_cpu-0.17.5/requirements-dev.txt` & `polars_lts_cpu-0.17.6/requirements-dev.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 tzdata; platform_system == 'Windows'
 xlsx2csv
 XlsxWriter
 adbc_driver_sqlite; python_version >= '3.9' and platform_system != 'Windows'
 connectorx==0.3.2a2; python_version >= '3.8'  # Latest full release is broken - unpin when 0.3.2 released
 
 # Tooling
-hypothesis==6.71.0
+hypothesis==6.72.0
 maturin==0.14.10
 pytest==7.3.0
 pytest-cov==4.0.0
 pytest-xdist==3.2.0
 
 # Stub files
 pandas-stubs==1.2.0.62
```

### Comparing `polars_lts_cpu-0.17.5/scripts/check_stacklevels.py` & `polars_lts_cpu-0.17.6/scripts/check_stacklevels.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/apply/dataframe.rs` & `polars_lts_cpu-0.17.6/src/apply/dataframe.rs`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,17 @@
                         inference_size,
                     )
                     .map_err(PyPolarsErr::from)?,
                 )
                 .into_py(py),
                 true,
             ));
-        } else if out.is_instance_of::<PyList>().unwrap() {
+        } else if out.is_instance_of::<PyList>().unwrap()
+            || out.is_instance_of::<PyTuple>().unwrap()
+        {
             return Err(PyPolarsErr::Other(
                 "A list output type is invalid. Do you mean to create polars List Series?\
 Then return a Series object."
                     .into(),
             )
             .into());
         } else {
```

### Comparing `polars_lts_cpu-0.17.5/src/apply/mod.rs` & `polars_lts_cpu-0.17.6/src/apply/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/apply/series.rs` & `polars_lts_cpu-0.17.6/src/apply/series.rs`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     } else if out.hasattr("_s")? {
         let py_pyseries = out.getattr("_s").unwrap();
         let series = py_pyseries.extract::<PySeries>().unwrap().series;
         let dt = series.dtype();
         applyer
             .apply_lambda_with_list_out_type(py, lambda.to_object(py), null_count, &series, dt)
             .map(|ca| ca.into_series().into())
-    } else if out.is_instance_of::<PyList>().unwrap() {
+    } else if out.is_instance_of::<PyList>().unwrap() || out.is_instance_of::<PyTuple>().unwrap() {
         let series = SERIES.call1(py, (out,))?;
         let py_pyseries = series.getattr(py, "_s").unwrap();
         let series = py_pyseries.extract::<PySeries>(py).unwrap().series;
 
         // empty dtype is incorrect use anyvalues.
         if series.is_empty() {
             let av = out.extract::<Wrap<AnyValue>>()?;
```

### Comparing `polars_lts_cpu-0.17.5/src/arrow_interop/to_py.rs` & `polars_lts_cpu-0.17.6/src/arrow_interop/to_py.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/arrow_interop/to_rust.rs` & `polars_lts_cpu-0.17.6/src/arrow_interop/to_rust.rs`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 pub fn field_to_rust(obj: &PyAny) -> PyResult<Field> {
     let schema = Box::new(ffi::ArrowSchema::empty());
     let schema_ptr = &*schema as *const ffi::ArrowSchema;
 
     // make the conversion through PyArrow's private API
     obj.call_method1("_export_to_c", (schema_ptr as Py_uintptr_t,))?;
     let field = unsafe { ffi::import_field_from_c(schema.as_ref()).map_err(PyPolarsErr::from)? };
-    Ok(Field::from(&field))
+    Ok((&field).into())
 }
 
 // PyList<Field> which you get by calling `list(schema)`
 pub fn pyarrow_schema_to_rust(obj: &PyList) -> PyResult<Schema> {
     obj.into_iter().map(field_to_rust).collect()
 }
```

### Comparing `polars_lts_cpu-0.17.5/src/batched_csv.rs` & `polars_lts_cpu-0.17.6/src/batched_csv.rs`

 * *Files 3% similar despite different names*

```diff
@@ -71,19 +71,21 @@
                 Some(s.as_bytes()[0])
             }
         } else {
             None
         };
 
         let overwrite_dtype = overwrite_dtype.map(|overwrite_dtype| {
-            let fields = overwrite_dtype.iter().map(|(name, dtype)| {
-                let dtype = dtype.0.clone();
-                Field::new(name, dtype)
-            });
-            Schema::from(fields)
+            overwrite_dtype
+                .iter()
+                .map(|(name, dtype)| {
+                    let dtype = dtype.0.clone();
+                    Field::new(name, dtype)
+                })
+                .collect::<Schema>()
         });
 
         let overwrite_dtype_slice = overwrite_dtype_slice.map(|overwrite_dtype| {
             overwrite_dtype
                 .iter()
                 .map(|dt| dt.0.clone())
                 .collect::<Vec<_>>()
```

### Comparing `polars_lts_cpu-0.17.5/src/conversion.rs` & `polars_lts_cpu-0.17.6/src/conversion.rs`

 * *Files 1% similar despite different names*

```diff
@@ -383,15 +383,15 @@
                     "Time" => DataType::Time,
                     "Duration" => DataType::Duration(TimeUnit::Microseconds),
                     "Decimal" => DataType::Decimal(None, None), // "none" scale => "infer"
                     "Float32" => DataType::Float32,
                     "Float64" => DataType::Float64,
                     #[cfg(feature = "object")]
                     "Object" => DataType::Object(OBJECT_NAME),
-                    "List" => DataType::List(Box::new(DataType::Boolean)),
+                    "List" => DataType::List(Box::new(DataType::Null)),
                     "Null" => DataType::Null,
                     "Unknown" => DataType::Unknown,
                     dt => {
                         return Err(PyValueError::new_err(format!(
                             "{dt} is not a correct polars DataType.",
                         )))
                     }
@@ -683,15 +683,15 @@
                 let key = k.extract::<&str>()?;
                 let val = v.extract::<Wrap<AnyValue>>()?.0;
                 let dtype = DataType::from(&val);
                 keys.push(Field::new(key, dtype));
                 vals.push(val)
             }
             Ok(Wrap(AnyValue::StructOwned(Box::new((vals, keys)))))
-        } else if ob.is_instance_of::<PyList>()? {
+        } else if ob.is_instance_of::<PyList>()? || ob.is_instance_of::<PyTuple>()? {
             materialize_list(ob)
         } else if let Ok(value) = ob.extract::<u64>() {
             Ok(AnyValue::UInt64(value).into())
         } else if ob.hasattr("_s")? {
             let py_pyseries = ob.getattr("_s").unwrap();
             let series = py_pyseries.extract::<PySeries>().unwrap().series;
             Ok(Wrap(AnyValue::List(series)))
```

### Comparing `polars_lts_cpu-0.17.5/src/dataframe.rs` & `polars_lts_cpu-0.17.6/src/dataframe.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,19 +64,19 @@
             }
             DataType::Decimal(_, _) => {
                 fld.coerce(DataType::Decimal(None, None));
                 fld
             }
             _ => fld,
         });
-        let mut schema = Schema::from(fields);
+        let mut schema = Schema::from_iter(fields);
 
         if let Some(schema_overwrite) = schema_overwrite {
             for (i, (name, dtype)) in schema_overwrite.into_iter().enumerate() {
-                if let Some((name_, dtype_)) = schema.get_index_mut(i) {
+                if let Some((name_, dtype_)) = schema.get_at_index_mut(i) {
                     *name_ = name;
 
                     // if user sets dtype unknown, we use the inferred datatype
                     if !matches!(dtype, DataType::Unknown) {
                         *dtype_ = dtype;
                     }
                 } else {
@@ -129,15 +129,15 @@
             .iter()
             .map(|s| format!("{}", s.dtype()))
             .collect()
     }
 
     #[staticmethod]
     #[allow(clippy::too_many_arguments)]
-    #[cfg(feature = "csv-file")]
+    #[cfg(feature = "csv")]
     #[pyo3(signature = (
         py_f, infer_schema_length, chunk_size, has_header, ignore_errors, n_rows,
         skip_rows, projection, separator, rechunk, columns, encoding, n_threads, path,
         overwrite_dtype, overwrite_dtype_slice, low_memory, comment_char, quote_char,
         null_values, missing_utf8_is_empty_string, try_parse_dates, skip_rows_after_header,
         row_count, sample_size, eol_char)
     )]
@@ -180,19 +180,21 @@
                 Some(s.as_bytes()[0])
             }
         } else {
             None
         };
 
         let overwrite_dtype = overwrite_dtype.map(|overwrite_dtype| {
-            let fields = overwrite_dtype.iter().map(|(name, dtype)| {
-                let dtype = dtype.0.clone();
-                Field::new(name, dtype)
-            });
-            Schema::from(fields)
+            overwrite_dtype
+                .iter()
+                .map(|(name, dtype)| {
+                    let dtype = dtype.0.clone();
+                    Field::new(name, dtype)
+                })
+                .collect::<Schema>()
         });
 
         let overwrite_dtype_slice = overwrite_dtype_slice.map(|overwrite_dtype| {
             overwrite_dtype
                 .iter()
                 .map(|dt| dt.0.clone())
                 .collect::<Vec<_>>()
```

### Comparing `polars_lts_cpu-0.17.5/src/datatypes.rs` & `polars_lts_cpu-0.17.6/src/datatypes.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/error.rs` & `polars_lts_cpu-0.17.6/src/error.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/file.rs` & `polars_lts_cpu-0.17.6/src/file.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/lazy/apply.rs` & `polars_lts_cpu-0.17.6/src/lazy/apply.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/lazy/dataframe.rs` & `polars_lts_cpu-0.17.6/src/lazy/dataframe.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 use std::borrow::Cow;
 use std::collections::HashMap;
 use std::io::BufWriter;
 use std::path::PathBuf;
 
 use polars::io::RowCount;
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 use polars::lazy::frame::LazyCsvReader;
 #[cfg(feature = "json")]
 use polars::lazy::frame::LazyJsonLineReader;
 use polars::lazy::frame::{AllowedOptimizations, LazyFrame, LazyGroupBy};
 use polars::lazy::prelude::col;
 use polars::prelude::{ClosedWindow, CsvEncoding, DataFrame, Field, JoinType, Schema};
 use polars::time::*;
@@ -211,15 +211,15 @@
             .finish()
             .map_err(PyPolarsErr::from)?;
         Ok(lf.into())
     }
 
     #[staticmethod]
     #[allow(clippy::too_many_arguments)]
-    #[cfg(feature = "csv-file")]
+    #[cfg(feature = "csv")]
     #[pyo3(signature = (path, separator, has_header, ignore_errors, skip_rows, n_rows, cache, overwrite_dtype,
         low_memory, comment_char, quote_char, null_values, missing_utf8_is_empty_string,
         infer_schema_length, with_schema_modify, rechunk, skip_rows_after_header,
         encoding, row_count, try_parse_dates, eol_char,
     )
     )]
     pub fn new_from_csv(
@@ -249,18 +249,18 @@
         let comment_char = comment_char.map(|s| s.as_bytes()[0]);
         let quote_char = quote_char.map(|s| s.as_bytes()[0]);
         let delimiter = separator.as_bytes()[0];
         let eol_char = eol_char.as_bytes()[0];
         let row_count = row_count.map(|(name, offset)| RowCount { name, offset });
 
         let overwrite_dtype = overwrite_dtype.map(|overwrite_dtype| {
-            let fields = overwrite_dtype
+            overwrite_dtype
                 .into_iter()
-                .map(|(name, dtype)| Field::new(name, dtype.0));
-            Schema::from(fields)
+                .map(|(name, dtype)| Field::new(name, dtype.0))
+                .collect::<Schema>()
         });
         let mut r = LazyCsvReader::new(path)
             .with_infer_schema_length(infer_schema_length)
             .with_delimiter(delimiter)
             .has_header(has_header)
             .with_ignore_errors(ignore_errors)
             .with_skip_rows(skip_rows)
@@ -287,19 +287,19 @@
 
                     let out = lambda.call1(py, (names,)).expect("python function failed");
                     let new_names = out
                         .extract::<Vec<String>>(py)
                         .expect("python function should return List[str]");
                     assert_eq!(new_names.len(), schema.len(), "The length of the new names list should be equal to the original column length");
 
-                    let fields = schema
+                    Ok(schema
                         .iter_dtypes()
                         .zip(new_names)
-                        .map(|(dtype, name)| Field::from_owned(name.into(), dtype.clone()));
-                    Ok(Schema::from(fields))
+                        .map(|(dtype, name)| Field::from_owned(name.into(), dtype.clone()))
+                        .collect())
                 })
             };
             r = r.with_schema_modify(f).map_err(PyPolarsErr::from)?
         }
 
         Ok(r.finish().map_err(PyPolarsErr::from)?.into())
     }
```

### Comparing `polars_lts_cpu-0.17.5/src/lazy/dsl.rs` & `polars_lts_cpu-0.17.6/src/lazy/dsl.rs`

 * *Files 1% similar despite different names*

```diff
@@ -546,96 +546,96 @@
         self.clone().inner.product().into()
     }
 
     pub fn shrink_dtype(&self) -> PyExpr {
         self.inner.clone().shrink_dtype().into()
     }
 
-    #[pyo3(signature = (fmt, strict, exact, cache))]
-    pub fn str_parse_date(
+    #[pyo3(signature = (format, strict, exact, cache))]
+    pub fn str_to_date(
         &self,
-        fmt: Option<String>,
+        format: Option<String>,
         strict: bool,
         exact: bool,
         cache: bool,
     ) -> PyExpr {
         self.inner
             .clone()
             .str()
             .strptime(StrpTimeOptions {
                 date_dtype: DataType::Date,
-                fmt,
+                format,
                 strict,
                 exact,
                 cache,
                 tz_aware: false,
                 utc: false,
             })
             .into()
     }
 
-    #[pyo3(signature = (fmt, strict, exact, cache, tz_aware, utc, time_unit, time_zone))]
+    #[pyo3(signature = (format, time_unit, time_zone, strict, exact, cache, tz_aware, utc))]
     #[allow(clippy::too_many_arguments)]
-    pub fn str_parse_datetime(
+    pub fn str_to_datetime(
         &self,
-        fmt: Option<String>,
+        format: Option<String>,
+        time_unit: Option<Wrap<TimeUnit>>,
+        time_zone: Option<TimeZone>,
         strict: bool,
         exact: bool,
         cache: bool,
         tz_aware: bool,
         utc: bool,
-        time_unit: Option<Wrap<TimeUnit>>,
-        time_zone: Option<TimeZone>,
     ) -> PyExpr {
-        let result_time_unit = match (&fmt, time_unit) {
+        let result_time_unit = match (&format, time_unit) {
             (_, Some(time_unit)) => time_unit.0,
-            (Some(fmt), None) => {
-                if fmt.contains("%.9f")
-                    || fmt.contains("%9f")
-                    || fmt.contains("%f")
-                    || fmt.contains("%.f")
+            (Some(format), None) => {
+                if format.contains("%.9f")
+                    || format.contains("%9f")
+                    || format.contains("%f")
+                    || format.contains("%.f")
                 {
                     TimeUnit::Nanoseconds
-                } else if fmt.contains("%.3f") || fmt.contains("%3f") {
+                } else if format.contains("%.3f") || format.contains("%3f") {
                     TimeUnit::Milliseconds
                 } else {
                     TimeUnit::Microseconds
                 }
             }
             (None, None) => TimeUnit::Microseconds,
         };
         self.inner
             .clone()
             .str()
             .strptime(StrpTimeOptions {
                 date_dtype: DataType::Datetime(result_time_unit, time_zone),
-                fmt,
+                format,
                 strict,
                 exact,
                 cache,
                 tz_aware,
                 utc,
             })
             .into()
     }
 
-    #[pyo3(signature = (fmt, strict, exact, cache))]
-    pub fn str_parse_time(
+    #[pyo3(signature = (format, strict, exact, cache))]
+    pub fn str_to_time(
         &self,
-        fmt: Option<String>,
+        format: Option<String>,
         strict: bool,
         exact: bool,
         cache: bool,
     ) -> PyExpr {
         self.inner
             .clone()
             .str()
             .strptime(StrpTimeOptions {
                 date_dtype: DataType::Time,
-                fmt,
+                format,
                 strict,
                 exact,
                 cache,
                 tz_aware: false,
                 utc: false,
             })
             .into()
@@ -1364,14 +1364,15 @@
         window_size: &str,
         weights: Option<Vec<f64>>,
         min_periods: usize,
         center: bool,
         by: Option<String>,
         closed: Option<Wrap<ClosedWindow>>,
     ) -> Self {
+        dbg!(window_size);
         let options = RollingOptions {
             window_size: Duration::parse(window_size),
             weights,
             min_periods,
             center,
             by,
             closed_window: closed.map(|c| c.0),
```

### Comparing `polars_lts_cpu-0.17.5/src/lazy/meta.rs` & `polars_lts_cpu-0.17.6/src/lazy/meta.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/lazy/mod.rs` & `polars_lts_cpu-0.17.6/src/lazy/mod.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/lib.rs` & `polars_lts_cpu-0.17.6/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 #[allow(dead_code)]
 mod build {
     include!(concat!(env!("OUT_DIR"), "/built.rs"));
 }
 
 pub mod apply;
 pub mod arrow_interop;
-#[cfg(feature = "csv-file")]
+#[cfg(feature = "csv")]
 mod batched_csv;
 pub mod conversion;
 pub mod dataframe;
 pub mod datatypes;
 pub mod error;
 pub mod file;
 pub mod lazy;
@@ -139,16 +139,16 @@
 
 #[pyfunction]
 fn cumreduce(lambda: PyObject, exprs: Vec<PyExpr>) -> PyExpr {
     dsl::cumreduce(lambda, exprs)
 }
 
 #[pyfunction]
-fn arange(low: PyExpr, high: PyExpr, step: usize) -> PyExpr {
-    polars_rs::lazy::dsl::arange(low.inner, high.inner, step).into()
+fn arange(start: PyExpr, end: PyExpr, step: i64) -> PyExpr {
+    polars_rs::lazy::dsl::arange(start.inner, end.inner, step).into()
 }
 
 #[pyfunction]
 fn repeat(value: &PyAny, n_times: PyExpr) -> PyResult<PyExpr> {
     if let Ok(true) = value.is_instance_of::<PyBool>() {
         let val = value.extract::<bool>().unwrap();
         Ok(polars_rs::lazy::dsl::repeat(val, n_times.inner).into())
@@ -662,15 +662,15 @@
     )?;
 
     m.add_class::<PySeries>().unwrap();
     m.add_class::<PyDataFrame>().unwrap();
     m.add_class::<PyLazyFrame>().unwrap();
     m.add_class::<PyLazyGroupBy>().unwrap();
     m.add_class::<dsl::PyExpr>().unwrap();
-    #[cfg(feature = "csv-file")]
+    #[cfg(feature = "csv")]
     m.add_class::<batched_csv::PyBatchedCsv>().unwrap();
     #[cfg(feature = "sql")]
     m.add_class::<sql::PySQLContext>().unwrap();
     m.add_wrapped(wrap_pyfunction!(col)).unwrap();
     m.add_wrapped(wrap_pyfunction!(count)).unwrap();
     m.add_wrapped(wrap_pyfunction!(first)).unwrap();
     m.add_wrapped(wrap_pyfunction!(last)).unwrap();
```

### Comparing `polars_lts_cpu-0.17.5/src/npy.rs` & `polars_lts_cpu-0.17.6/src/npy.rs`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 use polars_core::prelude::*;
 use polars_core::utils::arrow::types::NativeType;
 use polars_core::with_match_physical_numeric_polars_type;
 use pyo3::prelude::*;
 use pyo3::types::PyTuple;
 
 use crate::error::PyPolarsErr;
+use crate::prelude::ObjectValue;
 use crate::raise_err;
 use crate::series::PySeries;
 
 /// Create an empty numpy array arrows 64 byte alignment
 ///
 /// # Safety
 /// All elements in the array are non initialized
@@ -155,49 +156,63 @@
                 let msg = "Cannot take pointer of nested type";
                 raise_err!(msg, ComputeError);
             }
         }
     }
 
     /// For numeric types, this should only be called for Series with null types.
-    /// This will cast to floats so that `None = np.nan`
+    /// Non-nullable types are handled with `view()`.
+    /// This will cast to floats so that `None = np.nan`.
     pub fn to_numpy(&self, py: Python) -> PyResult<PyObject> {
         let s = &self.series;
         match s.dtype() {
-            DataType::Utf8 => {
-                let ca = s.utf8().unwrap();
-
-                let np_arr = PyArray1::from_iter(py, ca.into_iter().map(|s| s.into_py(py)));
-                Ok(np_arr.into_py(py))
-            }
             dt if dt.is_numeric() => {
                 if s.bit_repr_is_large() {
                     let s = s.cast(&DataType::Float64).unwrap();
                     let ca = s.f64().unwrap();
                     let np_arr = PyArray1::from_iter(
                         py,
-                        ca.into_iter().map(|opt_v| match opt_v {
-                            Some(v) => v,
-                            None => f64::NAN,
-                        }),
+                        ca.into_iter().map(|opt_v| opt_v.unwrap_or(f64::NAN)),
                     );
                     Ok(np_arr.into_py(py))
                 } else {
                     let s = s.cast(&DataType::Float32).unwrap();
                     let ca = s.f32().unwrap();
                     let np_arr = PyArray1::from_iter(
                         py,
-                        ca.into_iter().map(|opt_v| match opt_v {
-                            Some(v) => v,
-                            None => f32::NAN,
-                        }),
+                        ca.into_iter().map(|opt_v| opt_v.unwrap_or(f32::NAN)),
                     );
                     Ok(np_arr.into_py(py))
                 }
             }
+            DataType::Utf8 => {
+                let ca = s.utf8().unwrap();
+                let np_arr = PyArray1::from_iter(py, ca.into_iter().map(|s| s.into_py(py)));
+                Ok(np_arr.into_py(py))
+            }
+            DataType::Binary => {
+                let ca = s.binary().unwrap();
+                let np_arr = PyArray1::from_iter(py, ca.into_iter().map(|s| s.into_py(py)));
+                Ok(np_arr.into_py(py))
+            }
+            DataType::Boolean => {
+                let ca = s.bool().unwrap();
+                let np_arr = PyArray1::from_iter(py, ca.into_iter().map(|s| s.into_py(py)));
+                Ok(np_arr.into_py(py))
+            }
+            #[cfg(feature = "object")]
+            DataType::Object(_) => {
+                let ca = s
+                    .as_any()
+                    .downcast_ref::<ObjectChunked<ObjectValue>>()
+                    .unwrap();
+                let np_arr =
+                    PyArray1::from_iter(py, ca.into_iter().map(|opt_v| opt_v.to_object(py)));
+                Ok(np_arr.into_py(py))
+            }
             dt => {
                 raise_err!(
                     format!("'to_numpy' not supported for dtype: {dt:?}"),
                     ComputeError
                 );
             }
         }
```

### Comparing `polars_lts_cpu-0.17.5/src/object.rs` & `polars_lts_cpu-0.17.6/src/object.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/series.rs` & `polars_lts_cpu-0.17.6/src/series.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 use numpy::PyArray1;
 use polars_algo::{cut, hist, qcut};
 use polars_core::prelude::QuantileInterpolOptions;
 use polars_core::series::IsSorted;
-use polars_core::utils::{flatten_series, CustomIterTools};
+use polars_core::utils::flatten::flatten_series;
+use polars_core::utils::CustomIterTools;
 use pyo3::exceptions::{PyRuntimeError, PyValueError};
 use pyo3::prelude::*;
 use pyo3::types::{PyBytes, PyList};
 use pyo3::Python;
 
 use crate::apply::series::{call_lambda_and_extract, ApplyLambda};
 use crate::arrow_interop::to_rust::array_to_rust;
```

### Comparing `polars_lts_cpu-0.17.5/src/set.rs` & `polars_lts_cpu-0.17.6/src/set.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/sql.rs` & `polars_lts_cpu-0.17.6/src/sql.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/src/utils.rs` & `polars_lts_cpu-0.17.6/src/utils.rs`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/README.md` & `polars_lts_cpu-0.17.6/tests/README.md`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/benchmark/groupby-datagen.R` & `polars_lts_cpu-0.17.6/tests/benchmark/groupby-datagen.R`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/benchmark/run_h2oai_benchmark.py` & `polars_lts_cpu-0.17.6/tests/benchmark/run_h2oai_benchmark.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/benchmark/test_release.py` & `polars_lts_cpu-0.17.6/tests/benchmark/test_release.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/docs/run_doctest.py` & `polars_lts_cpu-0.17.6/tests/docs/run_doctest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/parametric/test_dataframe.py` & `polars_lts_cpu-0.17.6/tests/parametric/test_dataframe.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,24 +14,35 @@
 @given(df=dataframes())
 @settings(max_examples=50)
 def test_repr(df: pl.DataFrame) -> None:
     assert isinstance(repr(df), str)
     assert_frame_equal(df, df, check_exact=True, nans_compare_equal=True)
 
 
-@given(df=dataframes(cols=10, max_size=1, allowed_dtypes=[pl.UInt8, pl.Int8]))
+@given(
+    df=dataframes(
+        cols=10,
+        max_size=1,
+        allowed_dtypes=[pl.Int8, pl.UInt16, pl.List(pl.Int32)],
+    )
+)
 @settings(max_examples=3)
 def test_dtype_integer_cols(df: pl.DataFrame) -> None:
     # ensure dtype constraint works in conjunction with 'n' cols
-    assert all(tp in (pl.UInt8, pl.Int8) for tp in df.schema.values())
+    assert all(
+        tp in (pl.Int8, pl.UInt16, pl.List(pl.Int32)) for tp in df.schema.values()
+    )
 
 
 @given(
     df=dataframes(
-        min_size=1, min_cols=1, null_probability=0.25, excluded_dtypes=[pl.Utf8]
+        min_size=1,
+        min_cols=1,
+        null_probability=0.25,
+        excluded_dtypes=[pl.Utf8],
     )
 )
 @example(df=pl.DataFrame(schema=["x", "y", "z"]))
 @example(df=pl.DataFrame())
 def test_null_count(df: pl.DataFrame) -> None:
     # note: the zero-row and zero-col cases are always passed as explicit examples
     null_count, ncols = df.null_count(), len(df.columns)
```

### Comparing `polars_lts_cpu-0.17.5/tests/parametric/test_lazyframe.py` & `polars_lts_cpu-0.17.6/tests/parametric/test_lazyframe.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/parametric/test_series.py` & `polars_lts_cpu-0.17.6/tests/parametric/test_series.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # -------------------------------------------------
 # Validate Series behaviour with parametric tests
 # -------------------------------------------------
 from __future__ import annotations
 
-from decimal import Decimal
 from typing import no_type_check
 
 import numpy as np
 from hypothesis import given, settings
 from hypothesis.strategies import booleans, floats, sampled_from
 from numpy.testing import assert_array_equal
 
@@ -116,49 +115,71 @@
     sliced_pl_data = srs[s].to_list()
 
     assert sliced_py_data == sliced_pl_data, f"slice [{start}:{stop}:{step}] failed"
     assert_series_equal(srs, srs, check_exact=True)
 
 
 @given(
-    s1=series(min_size=1, max_size=10, dtype=pl.Datetime),
-    s2=series(min_size=1, max_size=10, dtype=pl.Duration),
+    s=series(min_size=1, max_size=10, dtype=pl.Datetime),
 )
-def test_series_timeunits(
-    s1: pl.Series,
-    s2: pl.Series,
+def test_series_datetime_timeunits(
+    s: pl.Series,
 ) -> None:
     # datetime
-    assert s1.to_list() == list(s1)
-    assert list(s1.dt.millisecond()) == [v.microsecond // 1000 for v in s1]
-    assert list(s1.dt.nanosecond()) == [v.microsecond * 1000 for v in s1]
-    assert list(s1.dt.microsecond()) == [v.microsecond for v in s1]
-
-    # duration
-    millis = s2.dt.milliseconds().to_list()
-    micros = s2.dt.microseconds().to_list()
-
-    assert s1.to_list() == list(s1)
-    assert millis == [int(Decimal(v) / 1000) for v in s2.cast(int)]
-    assert micros == list(s2.cast(int))
+    assert s.to_list() == list(s)
+    assert list(s.dt.millisecond()) == [v.microsecond // 1000 for v in s]
+    assert list(s.dt.nanosecond()) == [v.microsecond * 1000 for v in s]
+    assert list(s.dt.microsecond()) == [v.microsecond for v in s]
+
+
+@given(
+    s=series(min_size=1, max_size=10, dtype=pl.Duration),
+)
+def test_series_duration_timeunits(
+    s: pl.Series,
+) -> None:
+    nanos = s.dt.nanoseconds().to_list()
+    micros = s.dt.microseconds().to_list()
+    millis = s.dt.milliseconds().to_list()
+
+    scale = {
+        "ns": 1,
+        "us": 1_000,
+        "ms": 1_000_000,
+    }
+    assert nanos == [v * scale[s.dtype.time_unit] for v in s.to_physical()]  # type: ignore[union-attr]
+    assert micros == [int(v / 1_000) for v in nanos]
+    assert millis == [int(v / 1_000) for v in micros]
 
     # special handling for ns timeunit (as we may generate a microsecs-based
     # timedelta that results in 64bit overflow on conversion to nanosecs)
+    micros = s.dt.microseconds().to_list()
     lower_bound, upper_bound = -(2**63), (2**63) - 1
     if all(
         (lower_bound <= (us * 1000) <= upper_bound)
         for us in micros
         if isinstance(us, int)
     ):
-        for ns, us in zip(s2.dt.nanoseconds(), micros):
+        for ns, us in zip(s.dt.nanoseconds(), micros):
             assert ns == (us * 1000)
 
 
 @given(
-    s=series(min_size=1, max_size=10, excluded_dtypes=[pl.Categorical]),
+    s=series(min_size=1, max_size=10, excluded_dtypes=[pl.Categorical]).filter(
+        lambda x: (
+            getattr(x.dtype, "time_unit", None) in (None, "us", "ns")
+            and (x.dtype != pl.Utf8 or not x.str.contains("\x00").any())
+        )
+    ),
 )
+@settings(max_examples=250)
 def test_series_to_numpy(
     s: pl.Series,
 ) -> None:
-    if s.dtype != pl.Utf8 or not s.str.contains("\x00").any():
-        np_array = np.array(s.to_list())
-        assert_array_equal(np_array, s.to_numpy())
+    dtype = {
+        pl.Datetime("ns"): "datetime64[ns]",
+        pl.Datetime("us"): "datetime64[us]",
+        pl.Duration("ns"): "timedelta64[ns]",
+        pl.Duration("us"): "timedelta64[us]",
+    }
+    np_array = np.array(s.to_list(), dtype=dtype.get(s.dtype))  # type: ignore[call-overload]
+    assert_array_equal(np_array, s.to_numpy())
```

### Comparing `polars_lts_cpu-0.17.5/tests/parametric/test_testing.py` & `polars_lts_cpu-0.17.6/tests/parametric/test_testing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # ------------------------------------------------
 # Test/validate Polars' hypothesis strategy units
 # ------------------------------------------------
 from __future__ import annotations
 
 import warnings
+from datetime import datetime
 from typing import Any
 
 import pytest
 from hypothesis import given, settings
 from hypothesis.errors import InvalidArgument, NonInteractiveExampleWarning
 from hypothesis.strategies import sampled_from
 
 import polars as pl
+from polars.datatypes import TEMPORAL_DTYPES
 from polars.testing.parametric import (
     column,
     columns,
+    create_list_strategy,
     dataframes,
     series,
 )
 
-# TODO: make dtype categories flexible and available from datatypes module
-TEMPORAL_DTYPES = [pl.Datetime, pl.Date, pl.Time, pl.Duration]
-
 
 @given(df=dataframes(), lf=dataframes(lazy=True), srs=series())
 @settings(max_examples=5)
 def test_strategy_classes(df: pl.DataFrame, lf: pl.LazyFrame, srs: pl.Series) -> None:
     assert isinstance(df, pl.DataFrame)
     assert isinstance(lf, pl.LazyFrame)
     assert isinstance(srs, pl.Series)
@@ -176,15 +176,17 @@
     assert s1.n_chunks() == 1
     if len(s2) > 1:
         assert s2.n_chunks() > 1
 
 
 @given(
     df=dataframes(
-        allowed_dtypes=[pl.Float32, pl.Float64], max_cols=4, allow_infinities=False
+        allowed_dtypes=[pl.Float32, pl.Float64],
+        allow_infinities=False,
+        max_cols=4,
     ),
     s=series(dtype=pl.Float64, allow_infinities=False),
 )
 def test_infinities(
     df: pl.DataFrame,
     s: pl.Series,
 ) -> None:
@@ -196,14 +198,45 @@
         return False
 
     assert all(finite_float(val) for val in s.to_list())
     for col in df.columns:
         assert all(finite_float(val) for val in df[col].to_list())
 
 
+@given(
+    df=dataframes(
+        cols=[
+            column("colx", dtype=pl.List(pl.UInt8)),
+            column("coly", dtype=pl.List(pl.Datetime("ms"))),
+            column(
+                name="colz",
+                strategy=create_list_strategy(
+                    inner_dtype=pl.List(pl.Utf8),
+                    select_from=["aa", "bb", "cc"],
+                    min_size=1,
+                ),
+            ),
+        ]
+    ),
+)
+def test_list_strategy(df: pl.DataFrame) -> None:
+    assert df.schema == {
+        "colx": pl.List(pl.UInt8),
+        "coly": pl.List(pl.Datetime("ms")),
+        "colz": pl.List(pl.List(pl.Utf8)),
+    }
+    uint8_max = (2**8) - 1
+
+    for colx, coly, colz in df.iter_rows():
+        assert all(i <= uint8_max for i in colx)
+        assert all(isinstance(d, datetime) for d in coly)
+        for inner_list in colz:
+            assert all(s in ("aa", "bb", "cc") for s in inner_list)
+
+
 @pytest.mark.hypothesis()
 def test_invalid_arguments() -> None:
     for invalid_probability in (-1.0, +2.0):
         with pytest.raises(InvalidArgument, match="between 0.0 and 1.0"):
             column("colx", dtype=pl.Boolean, null_probability=invalid_probability)
 
         with warnings.catch_warnings():
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/conftest.py` & `polars_lts_cpu-0.17.6/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_bool.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_bool.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_categorical.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_categorical.py`

 * *Files 3% similar despite different names*

```diff
@@ -347,7 +347,33 @@
 
 def test_nested_categorical_cast() -> None:
     values = [["x"], ["y"], ["x"]]
     dtype = pl.List(pl.Categorical)
     s = pl.Series(values).cast(dtype)
     assert s.dtype == dtype
     assert s.to_list() == values
+
+
+def test_struct_categorical_nesting() -> None:
+    # this triggers a lot of materialization
+    df = pl.DataFrame(
+        {"cats": ["Value1", "Value2", "Value1"]},
+        schema_overrides={"cats": pl.Categorical},
+    )
+    s = df.select(pl.struct(pl.col("cats")))["cats"].implode()
+    assert s.dtype == pl.List(pl.Struct([pl.Field("cats", pl.Categorical)]))
+    # triggers recursive conversion
+    assert s.to_list() == [[{"cats": "Value1"}, {"cats": "Value2"}, {"cats": "Value1"}]]
+    # triggers different recursive conversion
+    assert len(s.to_arrow()) == 1
+
+
+def test_categorical_fill_null_existing_category() -> None:
+    # ensure physical types align
+    assert pl.DataFrame(
+        {"col": ["a", None, "a"]}, schema={"col": pl.Categorical}
+    ).fill_null("a").with_columns(pl.col("col").to_physical().alias("code")).to_dict(
+        False
+    ) == {
+        "col": ["a", "a", "a"],
+        "code": [0, 0, 0],
+    }
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_decimal.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_decimal.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_list.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -243,31 +243,14 @@
 
     assert pl.concat([df1, df2], how="diagonal").to_dict(False) == {
         "a": [1, 2, None],
         "b": [None, None, [1]],
     }
 
 
-def test_is_in_empty_list_4559() -> None:
-    assert pl.Series(["a"]).is_in([]).to_list() == [False]
-
-
-def test_is_in_empty_list_4639() -> None:
-    df = pl.DataFrame({"a": [1, None]})
-    empty_list: list[int] = []
-
-    assert df.with_columns([pl.col("a").is_in(empty_list).alias("a_in_list")]).to_dict(
-        False
-    ) == {"a": [1, None], "a_in_list": [False, False]}
-    df = pl.DataFrame()
-    assert df.with_columns(
-        [pl.lit(None).cast(pl.Int64).is_in(empty_list).alias("in_empty_list")]
-    ).to_dict(False) == {"in_empty_list": [False]}
-
-
 def test_inner_type_categorical_on_rechunk() -> None:
     df = pl.DataFrame({"cats": ["foo", "bar"]}).select(
         pl.col(pl.Utf8).cast(pl.Categorical).implode()
     )
 
     assert pl.concat([df, df], rechunk=True).dtypes == [pl.List(pl.Categorical)]
 
@@ -467,7 +450,73 @@
     ).to_dict(False) == {"": [[["a", "b"]]]}
 
 
 def test_null_list_construction_and_materialization() -> None:
     s = pl.Series([None, []])
     assert s.dtype == pl.List(pl.Null)
     assert s.to_list() == [None, []]
+
+
+def test_logical_type_struct_agg_list() -> None:
+    df = pl.DataFrame(
+        {"cats": ["Value1", "Value2", "Value1"]},
+        schema_overrides={"cats": pl.Categorical},
+    )
+    out = df.groupby(1).agg(pl.struct("cats"))
+    assert out.dtypes == [
+        pl.Int32,
+        pl.List(pl.Struct([pl.Field("cats", pl.Categorical)])),
+    ]
+    assert out["cats"].to_list() == [
+        [{"cats": "Value1"}, {"cats": "Value2"}, {"cats": "Value1"}]
+    ]
+
+
+def test_logical_parallel_list_collect() -> None:
+    # this triggers the anonymous builder in par collect
+    out = (
+        pl.DataFrame(
+            {
+                "Group": ["GroupA", "GroupA", "GroupA"],
+                "Values": ["Value1", "Value2", "Value1"],
+            },
+            schema_overrides={"Values": pl.Categorical},
+        )
+        .groupby("Group")
+        .agg(pl.col("Values").value_counts(sort=True))
+        .explode("Values")
+        .unnest("Values")
+    )
+    assert out.dtypes == [pl.Utf8, pl.Categorical, pl.UInt32]
+    assert out.to_dict(False) == {
+        "Group": ["GroupA", "GroupA"],
+        "Values": ["Value1", "Value2"],
+        "counts": [2, 1],
+    }
+
+
+def test_list_recursive_categorical_cast() -> None:
+    # go 3 deep, just to show off
+    dtype = pl.List(pl.List(pl.List(pl.Categorical)))
+    values = [[[["x"], ["y"]]], [[["x"]]]]
+    s = pl.Series(values).cast(dtype)
+    assert s.dtype == dtype
+    assert s.to_list() == values
+
+
+def test_list_new_from_index_logical() -> None:
+    s = (
+        pl.select(pl.struct(pl.Series("a", [date(2001, 1, 1)])).implode())
+        .to_series()
+        .new_from_index(0, 1)
+    )
+    assert s.dtype == pl.List(pl.Struct([pl.Field("a", pl.Date)]))
+    assert s.to_list() == [[{"a": date(2001, 1, 1)}]]
+
+
+def test_list_recursive_time_unit_cast() -> None:
+    values = [[datetime(2000, 1, 1, 0, 0, 0)]]
+    dtype = pl.List(pl.Datetime("ns"))
+    s = pl.Series(values)
+    out = s.cast(dtype)
+    assert out.dtype == dtype
+    assert out.to_list() == values
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_object.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_object.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_struct.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,23 @@
             "e": [None, "foo", "foo", "foo"],
         }
     )
 
     assert_frame_equal(df, expected)
 
 
+def test_struct_hashes() -> None:
+    dtypes = (
+        pl.Struct,
+        pl.Struct([pl.Field("a", pl.Int64)]),
+        pl.Struct([pl.Field("a", pl.Int64), pl.Field("b", pl.List(pl.Int64))]),
+    )
+    assert len({hash(tp) for tp in (dtypes)}) == 3
+
+
 def test_struct_unnesting() -> None:
     df = pl.DataFrame({"a": [1, 2]})
     out = df.select(
         [
             pl.all().alias("a_original"),
             pl.col("a")
             .apply(lambda x: {"a": x, "b": x * 2, "c": x % 2 == 0})
@@ -544,31 +553,14 @@
     assert len(unique) == 1
     unique_el = unique[0]
     assert len(unique_el) == 2
     assert {"a": 2, "b": 12} in unique_el
     assert {"a": 1, "b": 11} in unique_el
 
 
-def test_is_in_struct() -> None:
-    df = pl.DataFrame(
-        {
-            "struct_elem": [{"a": 1, "b": 11}, {"a": 1, "b": 90}],
-            "struct_list": [
-                [{"a": 1, "b": 11}, {"a": 2, "b": 12}, {"a": 3, "b": 13}],
-                [{"a": 3, "b": 3}],
-            ],
-        }
-    )
-
-    assert df.filter(pl.col("struct_elem").is_in("struct_list")).to_dict(False) == {
-        "struct_elem": [{"a": 1, "b": 11}],
-        "struct_list": [[{"a": 1, "b": 11}, {"a": 2, "b": 12}, {"a": 3, "b": 13}]],
-    }
-
-
 def test_nested_explode_4026() -> None:
     df = pl.DataFrame(
         {
             "data": [
                 [
                     {"account_id": 10, "values": [1, 2]},
                     {"account_id": 11, "values": [10, 20]},
@@ -963,7 +955,23 @@
                 {"val": 0, "counts": 1},
                 {"val": 1, "counts": 1},
                 {"val": 2, "counts": 1},
                 {"val": 3, "counts": 1},
             ]
         ],
     }
+
+
+def test_struct_lit_cast() -> None:
+    df = pl.DataFrame({"a": [1, 2, 3]})
+    schema = {"a": pl.Int64, "b": pl.List(pl.Int64)}
+
+    for lit in [pl.lit(None), pl.lit([[]])]:
+        s = df.select(pl.struct([pl.col("a"), lit.alias("b")], schema=schema))["a"]  # type: ignore[arg-type]
+        assert s.dtype == pl.Struct(
+            [pl.Field("a", pl.Int64), pl.Field("b", pl.List(pl.Int64))]
+        )
+        assert s.to_list() == [
+            {"a": 1, "b": None},
+            {"a": 2, "b": None},
+            {"a": 3, "b": None},
+        ]
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/datatypes/test_temporal.py` & `polars_lts_cpu-0.17.6/tests/unit/datatypes/test_temporal.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import io
 from datetime import date, datetime, time, timedelta, timezone
-from typing import TYPE_CHECKING, cast, no_type_check
+from typing import TYPE_CHECKING, Any, cast, no_type_check
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pytest
 
 import polars as pl
@@ -1751,24 +1751,14 @@
             [pl.Series("dt", [date(2015, 6, 24), date(2015, 6, 23)], dtype=pl.Date)]
         )
         .sort("dt")
         .unique()
     ).to_dict(False) == {"dt": [date(2015, 6, 23), date(2015, 6, 24)]}
 
 
-def test_time_zero_3828() -> None:
-    assert pl.Series(values=[time(0)], dtype=pl.Time).to_list() == [time(0)]
-
-
-def test_time_microseconds_3843() -> None:
-    in_val = [time(0, 9, 11, 558332)]
-    s = pl.Series(in_val)
-    assert s.to_list() == in_val
-
-
 def test_date_to_time_cast_5111() -> None:
     # check date -> time casts (fast-path: always 00:00:00)
     df = pl.DataFrame(
         {
             "xyz": [
                 date(1969, 1, 1),
                 date(1990, 3, 8),
@@ -1857,14 +1847,24 @@
     ).to_dict(False) == {
         "date": [date(2001, 1, 1), date(2001, 1, 2), date(2001, 1, 3)],
         "date_plus_one": [date(2001, 1, 2), date(2001, 1, 3), date(2001, 1, 4)],
         "date_min_one": [date(2000, 12, 31), date(2001, 1, 1), date(2001, 1, 2)],
     }
 
 
+def test_datetime_hashes() -> None:
+    dtypes = (
+        pl.Datetime,
+        pl.Datetime("us"),
+        pl.Datetime("us", "UTC"),
+        pl.Datetime("us", "Zulu"),
+    )
+    assert len({hash(tp) for tp in (dtypes)}) == 4
+
+
 def test_datetime_string_casts() -> None:
     df = pl.DataFrame(
         {
             "x": [1661855445123],
             "y": [1661855445123456],
             "z": [1661855445123456789],
         },
@@ -2785,12 +2785,54 @@
         assert s.is_temporal() is True
 
     s = pl.Series([datetime(2023, 2, 14, 11, 12, 13)], dtype=pl.Datetime)
     for tp in (pl.Datetime, [pl.Datetime], [pl.Time, pl.Datetime]):  # type: ignore[assignment]
         assert s.is_temporal(excluding=tp) is False
 
 
-def test_microsecond_precision_any_value_conversion() -> None:
-    dt = datetime(2514, 5, 30, 1, 53, 4, 986754, tzinfo=timezone.utc)
-    assert pl.Series([dt]).to_list() == [dt]
-    dt = datetime(2514, 5, 30, 1, 53, 4, 986754)
+@pytest.mark.parametrize(
+    "time_zone",
+    [
+        None,
+        timezone.utc,
+        "America/Caracas",
+        "Asia/Kathmandu",
+        "Asia/Taipei",
+        "Europe/Amsterdam",
+        "Europe/Lisbon",
+        "Indian/Maldives",
+        "Pacific/Norfolk",
+        "Pacific/Samoa",
+        "Turkey",
+        "US/Eastern",
+        "UTC",
+        "Zulu",
+    ],
+)
+def test_misc_precision_any_value_conversion(time_zone: Any) -> None:
+    tz = ZoneInfo(time_zone) if isinstance(time_zone, str) else time_zone
+
+    # default precision (μs)
+    dt = datetime(2514, 5, 30, 1, 53, 4, 986754, tzinfo=tz)
     assert pl.Series([dt]).to_list() == [dt]
+
+    # ms precision
+    dt = datetime(2243, 1, 1, 0, 0, 0, 1000, tzinfo=tz)
+    assert pl.Series([dt]).cast(pl.Datetime("ms", time_zone)).to_list() == [dt]
+
+    # ns precision
+    dt = datetime(2256, 1, 1, 0, 0, 0, 1, tzinfo=tz)
+    assert pl.Series([dt]).cast(pl.Datetime("ns", time_zone)).to_list() == [dt]
+
+
+@pytest.mark.parametrize(
+    "tm",
+    [
+        time(0, 20, 30, 1),
+        time(8, 40, 15, 8888),
+        time(15, 10, 20, 123456),
+        time(23, 59, 59, 999999),
+    ],
+)
+def test_pytime_conversion(tm: time) -> None:
+    s = pl.Series("tm", [tm])
+    assert s.to_list() == [tm]
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json` & `polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000000.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json` & `polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/_delta_log/00000000000000000001.json`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet` & `polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/part-00000-e42312d7-60e5-454d-acbc-db192d220e73-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet` & `polars_lts_cpu-0.17.6/tests/unit/io/files/delta-table/part-00000-e4a999da-df45-4fb0-bdc4-d999fc0f58aa-c000.snappy.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/example.xlsx` & `polars_lts_cpu-0.17.6/tests/unit/io/files/example.xlsx`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.ipc` & `polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.ndjson` & `polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/foods1.parquet` & `polars_lts_cpu-0.17.6/tests/unit/io/files/foods1.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.ipc` & `polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.ipc`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.ndjson` & `polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.ndjson`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/foods2.parquet` & `polars_lts_cpu-0.17.6/tests/unit/io/files/foods2.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/files/small.parquet` & `polars_lts_cpu-0.17.6/tests/unit/io/files/small.parquet`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_avro.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_avro.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_csv.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_csv.py`

 * *Files 1% similar despite different names*

```diff
@@ -825,40 +825,53 @@
 def test_csv_multiple_null_values() -> None:
     df = pl.DataFrame(
         {
             "a": [1, 2, None, 4],
             "b": ["2022-01-01", "__NA__", "", "NA"],
         }
     )
-
     f = io.BytesIO()
     df.write_csv(f)
     f.seek(0)
 
     df2 = pl.read_csv(f, null_values=["__NA__", "NA"])
     expected = pl.DataFrame(
         {
             "a": [1, 2, None, 4],
             "b": ["2022-01-01", None, "", None],
         }
     )
-
     assert_frame_equal(df2, expected)
 
 
 def test_different_eol_char() -> None:
     csv = "a,1,10;b,2,20;c,3,30"
     expected = pl.DataFrame(
         {"column_1": ["a", "b", "c"], "column_2": [1, 2, 3], "column_3": [10, 20, 30]}
     )
     assert_frame_equal(
         pl.read_csv(csv.encode(), eol_char=";", has_header=False), expected
     )
 
 
+def test_csv_write_escape_headers() -> None:
+    df0 = pl.DataFrame({"col,1": ["data,1"], 'col"2': ['data"2'], "col:3": ["data:3"]})
+    out = io.BytesIO()
+    df0.write_csv(out)
+    assert out.getvalue() == b'"col,1","col""2",col:3\n"data,1","data""2",data:3\n'
+
+    df1 = pl.DataFrame({"c,o,l,u,m,n": [123]})
+    out = io.BytesIO()
+    df1.write_csv(out)
+
+    df2 = pl.read_csv(out)
+    assert_frame_equal(df1, df2)
+    assert df2.schema == {"c,o,l,u,m,n": pl.Int64}
+
+
 def test_csv_write_escape_newlines() -> None:
     df = pl.DataFrame({"escape": ["n\nn"]})
     f = io.BytesIO()
     df.write_csv(f)
     f.seek(0)
     read_df = pl.read_csv(f)
     assert_frame_equal(df, read_df)
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_database.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_database.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_delta.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_delta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_excel.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_excel.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,30 @@
     df = pl.read_excel(excel_file_path, sheet_name="Sheet1", sheet_id=None)
 
     expected = pl.DataFrame({"hello": ["Row 1", "Row 2"]})
     assert_frame_equal(df, expected)
 
 
 def test_read_excel_all_sheets(excel_file_path: Path) -> None:
-    df = pl.read_excel(excel_file_path, sheet_id=None)  # type: ignore[call-overload]
+    df = pl.read_excel(excel_file_path, sheet_id=0)
 
     expected1 = pl.DataFrame({"hello": ["Row 1", "Row 2"]})
     expected2 = pl.DataFrame({"world": ["Row 3", "Row 4"]})
 
     assert_frame_equal(df["Sheet1"], expected1)
     assert_frame_equal(df["Sheet2"], expected2)
 
 
+def test_read_excel_all_sheets_with_sheet_name(excel_file_path: Path) -> None:
+    with pytest.raises(
+        ValueError, match="Cannot specify both `sheet_name` and `sheet_id`"
+    ):
+        pl.read_excel(excel_file_path, sheet_id=1, sheet_name="Sheet1")
+
+
 # the parameters don't change the data, only the formatting, so we expect
 # the same result each time. however, it's important to validate that the
 # parameter permutations don't raise exceptions, or interfere with the
 # values written to the worksheet, so test multiple variations.
 @pytest.mark.parametrize(
     "write_params",
     [
@@ -150,15 +157,15 @@
         fmt_strptime = "%d-%m-%Y"
 
     # write to an xlsx with polars, using various parameters...
     xls = BytesIO()
     _wb = df.write_excel(workbook=xls, worksheet="data", **write_params)
 
     # ...and read it back again:
-    xldf = pl.read_excel(  # type: ignore[call-overload]
+    xldf = pl.read_excel(
         xls,
         sheet_name="data",
         read_csv_options=header_opts,
     )[:3]
     xldf = xldf.select(xldf.columns[:3]).with_columns(
         pl.col("dtm").str.strptime(pl.Date, fmt_strptime)
     )
@@ -169,15 +176,15 @@
     df = pl.DataFrame(
         {"x": [[1, 2], [3, 4], [5, 6]], "y": ["a", "b", "c"], "z": [9, 8, 7]}
     ).select("x", pl.struct(["y", "z"]))
 
     xls = BytesIO()
     df.write_excel(xls, worksheet="data")
 
-    xldf = pl.read_excel(xls, sheet_name="data")  # type: ignore[call-overload]
+    xldf = pl.read_excel(xls, sheet_name="data")
     assert xldf.rows() == [
         ("[1, 2]", "{'y': 'a', 'z': 9}"),
         ("[3, 4]", "{'y': 'b', 'z': 8}"),
         ("[5, 6]", "{'y': 'c', 'z': 7}"),
     ]
 
 
@@ -229,15 +236,15 @@
             row_heights=35,
             sheet_zoom=125,
         )
 
     tables = {tbl["name"] for tbl in wb.get_worksheet_by_name("frame_data").tables}
     assert "Frame0" in tables
 
-    xldf = pl.read_excel(xls, sheet_name="frame_data")  # type: ignore[call-overload]
+    xldf = pl.read_excel(xls, sheet_name="frame_data")
     # ┌─────┬──────┬─────┬─────┬─────┬─────┬───────┬─────┬─────┐
     # │ id  ┆ +/-  ┆ q1  ┆ q2  ┆ q3  ┆ q4  ┆ trend ┆ h1  ┆ h2  │
     # │ --- ┆ ---  ┆ --- ┆ --- ┆ --- ┆ --- ┆ ---   ┆ --- ┆ --- │
     # │ str ┆ str  ┆ i64 ┆ i64 ┆ i64 ┆ i64 ┆ str   ┆ i64 ┆ i64 │
     # ╞═════╪══════╪═════╪═════╪═════╪═════╪═══════╪═════╪═════╡
     # │ aaa ┆ null ┆ 100 ┆ 30  ┆ -50 ┆ 75  ┆ null  ┆ 0   ┆ 0   │
     # │ bbb ┆ null ┆ 55  ┆ -10 ┆ 0   ┆ 55  ┆ null  ┆ 0   ┆ 0   │
@@ -285,8 +292,8 @@
 
     table_names: set[str] = set()
     for sheet in ("sheet1", "sheet2", "sheet3"):
         table_names.update(
             tbl["name"] for tbl in wb.get_worksheet_by_name(sheet).tables
         )
     assert table_names == {f"Frame{n}" for n in range(4)}
-    assert pl.read_excel(xls, sheet_name="sheet3").rows() == []  # type: ignore[call-overload]
+    assert pl.read_excel(xls, sheet_name="sheet3").rows() == []
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_ipc.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_json.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_json.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import io
+import json
 from pathlib import Path
 
 import pytest
 
 import polars as pl
 from polars.testing import assert_frame_equal, assert_frame_equal_local_categoricals
 from polars.testing._tempdir import TemporaryDirectory
@@ -110,7 +111,18 @@
     data = {"column": ["test1", "test2", "test3", "test4"]}
     df = pl.DataFrame(data).with_columns(pl.col("column").cast(pl.Categorical))
 
     assert (
         df.write_json(row_oriented=True, file=None)
         == '[{"column":"test1"},{"column":"test2"},{"column":"test3"},{"column":"test4"}]'
     )
+
+
+def test_json_supertype_infer() -> None:
+    json_string = """[
+{"c":[{"b": [], "a": "1"}]},
+{"c":[{"b":[]}]},
+{"c":[{"b":["1"], "a": "1"}]}]
+"""
+    python_infer = pl.from_records(json.loads(json_string))
+    polars_infer = pl.read_json(io.StringIO(json_string))
+    assert_frame_equal(python_infer, polars_infer)
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_csv.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_csv.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_ipc.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_ipc.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_json.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_json.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_lazy_parquet.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_lazy_parquet.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_other.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_other.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_parquet.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,7 +440,26 @@
     # write as parquet
     df.to_parquet(f)
     f.seek(0)
 
     # read it with polars
     polars_df = pl.read_parquet(f)
     assert_frame_equal(pl.DataFrame(df), polars_df)
+
+
+def test_nested_null_roundtrip() -> None:
+    f = io.BytesIO()
+    df = pl.DataFrame(
+        {
+            "experiences": [
+                [
+                    {"company": "Google", "years": None},
+                    {"company": "Facebook", "years": None},
+                ],
+            ]
+        }
+    )
+
+    df.write_parquet(f)
+    f.seek(0)
+    df_read = pl.read_parquet(f)
+    assert_frame_equal(df_read, df)
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_pickle.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_pickle.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/io/test_pyarrow_dataset.py` & `polars_lts_cpu-0.17.6/tests/unit/io/test_pyarrow_dataset.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_binary.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_binary.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_categorical.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_categorical.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_datetime.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_datetime.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_list.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_list.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_meta.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_meta.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_string.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_string.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_strptime.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_strptime.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,16 +446,16 @@
         pl.Series(ts).str.strptime(pl.Datetime, fmt, utc=False)
 
 
 def test_tz_aware_without_fmt() -> None:
     with pytest.raises(
         ComputeError,
         match=(
-            r"^passing 'tz_aware=True' without 'fmt' is not yet supported, "
-            r"please specify 'fmt'$"
+            r"^passing 'tz_aware=True' without 'format' is not yet supported, "
+            r"please specify 'format'$"
         ),
     ), pytest.warns(
         DeprecationWarning,
-        match="`tz_aware` is now auto-inferred from `fmt` and will be removed "
+        match="`tz_aware` is now auto-inferred from `format` and will be removed "
         "in a future version. You can safely drop this argument.",
     ):
         pl.Series(["2020-01-01"]).str.strptime(pl.Datetime, tz_aware=True)
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/namespaces/test_struct.py` & `polars_lts_cpu-0.17.6/tests/unit/namespaces/test_struct.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_aggregations.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_aggregations.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_apply.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_apply.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_arithmetic.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_arithmetic.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_comparison.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_comparison.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_drop.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_drop.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_explode.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_explode.py`

 * *Files 6% similar despite different names*

```diff
@@ -275,7 +275,22 @@
             "col2": [["A", "B", "C"], ["C"], ["D", "E"]],
         }
     ).with_row_count()
     with pytest.raises(
         pl.ShapeError, match=r"exploded columns must have matching element counts"
     ):
         df.explode(["col1", "col2"])
+
+
+def test_logical_explode() -> None:
+    out = (
+        pl.DataFrame(
+            {"cats": ["Value1", "Value2", "Value1"]},
+            schema_overrides={"cats": pl.Categorical},
+        )
+        .groupby(1)
+        .agg(pl.struct("cats"))
+        .explode("cats")
+        .unnest("cats")
+    )
+    assert out["cats"].dtype == pl.Categorical
+    assert out["cats"].to_list() == ["Value1", "Value2", "Value1"]
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_filter.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_filter.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,22 +70,14 @@
     ) == {
         "group": [1, 2],
         "any": [[False, True, True], [True]],
         "filtered": [[3, 4], [2]],
     }
 
 
-def test_is_in_bool() -> None:
-    bool_value_to_filter_on = [True, None]
-    df = pl.DataFrame({"A": [True, False, None]})
-    assert df.filter(pl.col("A").is_in(bool_value_to_filter_on)).to_dict(False) == {
-        "A": [True, False]
-    }
-
-
 def test_predicate_order_explode_5950() -> None:
     df = pl.from_dict(
         {
             "i": [[0, 1], [1, 2]],
             "n": [0, None],
         }
     )
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_folds.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_folds.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_groupby.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_groupby.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_join.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_join.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_join_asof.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_join_asof.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_melt.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_melt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_pivot.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_pivot.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_rolling.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_rolling.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_sort.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_sort.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_statistics.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_statistics.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_transpose.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_transpose.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_unique.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_unique.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/operations/test_window.py` & `polars_lts_cpu-0.17.6/tests/unit/operations/test_window.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_api.py` & `polars_lts_cpu-0.17.6/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_arity.py` & `polars_lts_cpu-0.17.6/tests/unit/test_arity.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_cfg.py` & `polars_lts_cpu-0.17.6/tests/unit/test_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,15 @@
         yield
 
 
 def test_ascii_tables() -> None:
     df = pl.DataFrame({"a": [1, 2, 3], "b": [4, 5, 6], "c": [7, 8, 9]})
 
     # note: expect to render ascii only within the given scope
-    with pl.Config() as cfg:
-        cfg.set_ascii_tables(True)
+    with pl.Config(set_ascii_tables=True):
         assert (
             str(df) == "shape: (3, 3)\n"
             "+-----+-----+-----+\n"
             "| a   | b   | c   |\n"
             "| --- | --- | --- |\n"
             "| i64 | i64 | i64 |\n"
             "+=================+\n"
@@ -274,31 +273,32 @@
         "|-----|-----|-----|\n"
         "| 1   | 6.0 | a   |\n"
         "| 2   | 7.0 | b   |\n"
         "| 3   | 8.0 | c   |"
     )
 
     pl.Config().set_tbl_formatting("ASCII_BORDERS_ONLY_CONDENSED")
-    with pl.Config() as cfg:
-        cfg.set_tbl_hide_dtype_separator(True)
+    with pl.Config(tbl_hide_dtype_separator=True):
         assert str(df) == (
             "shape: (3, 3)\n"
             "+-----------------+\n"
             "| foo   bar   ham |\n"
             "| i64   f64   str |\n"
             "+=================+\n"
             "| 1     6.0   a   |\n"
             "| 2     7.0   b   |\n"
             "| 3     8.0   c   |\n"
             "+-----------------+"
         )
 
     # temporarily scope "nothing" style, with no data types
-    with pl.Config() as cfg:
-        cfg.set_tbl_formatting("NOTHING").set_tbl_hide_column_data_types(True)
+    with pl.Config(
+        tbl_formatting="NOTHING",
+        tbl_hide_column_data_types=True,
+    ):
         assert str(df) == (
             "shape: (3, 3)\n"
             " foo  bar  ham \n"
             " 1    6.0  a   \n"
             " 2    7.0  b   \n"
             " 3    8.0  c   "
         )
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_constructors.py` & `polars_lts_cpu-0.17.6/tests/unit/test_constructors.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_cse.py` & `polars_lts_cpu-0.17.6/tests/unit/test_cse.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_datatypes.py` & `polars_lts_cpu-0.17.6/tests/unit/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_df.py` & `polars_lts_cpu-0.17.6/tests/unit/test_df.py`

 * *Files 0% similar despite different names*

```diff
@@ -2652,23 +2652,14 @@
             .is_between(time(0, 45), time(10, 30), closed="right")
             .alias("tm_between")
         )[:, 0],
         pl.Series("tm_between", [True, False, False]),
     )
 
 
-def test_is_in() -> None:
-    df = pl.DataFrame({"a": [1, 2, 3]})
-    assert df.select(pl.col("a").is_in([1, 2]))["a"].to_list() == [
-        True,
-        True,
-        False,
-    ]
-
-
 def test_empty_is_in() -> None:
     df_empty_isin = pl.DataFrame({"foo": ["a", "b", "c", "d"]}).filter(
         pl.col("foo").is_in([])
     )
     assert df_empty_isin.shape == (0, 1)
     assert df_empty_isin.rows() == []
     assert df_empty_isin.schema == {"foo": pl.Utf8}
@@ -3424,18 +3415,24 @@
     df = pl.DataFrame({"a": [1]})
     assert df.item() == 1
 
     df = pl.DataFrame({"a": [1, 2]})
     with pytest.raises(ValueError):
         df.item()
 
+    assert df.item(0, 0) == 1
+    assert df.item(1, "a") == 2
+
     df = pl.DataFrame({"a": [1], "b": [2]})
     with pytest.raises(ValueError):
         df.item()
 
+    assert df.item(0, "a") == 1
+    assert df.item(0, "b") == 2
+
     df = pl.DataFrame({})
     with pytest.raises(ValueError):
         df.item()
 
 
 @pytest.mark.parametrize(
     ("subset", "keep", "expected_mask"),
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_empty.py` & `polars_lts_cpu-0.17.6/tests/unit/test_empty.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,7 +26,13 @@
 
 def test_empty_string_replace() -> None:
     s = pl.Series("", [], dtype=pl.Utf8)
     assert s.str.replace("a", "b", literal=True).series_equal(s)
     assert s.str.replace("a", "b").series_equal(s)
     assert s.str.replace("ab", "b", literal=True).series_equal(s)
     assert s.str.replace("ab", "b").series_equal(s)
+
+
+def test_empty_duration() -> None:
+    s = pl.DataFrame([], {"days": pl.Int32}).select(pl.duration(days="days"))
+    assert s.dtypes == [pl.Duration("ns")]
+    assert s.shape == (0, 1)
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_errors.py` & `polars_lts_cpu-0.17.6/tests/unit/test_errors.py`

 * *Files 2% similar despite different names*

```diff
@@ -547,7 +547,42 @@
             pl.col("weight")
         )
 
 
 def test_lit_agg_err() -> None:
     with pytest.raises(pl.ComputeError, match=r"cannot aggregate a literal"):
         pl.DataFrame({"y": [1]}).with_columns(pl.lit(1).sum().over("y"))
+
+
+def test_window_size_validation() -> None:
+    df = pl.DataFrame({"x": [1.0]})
+
+    with pytest.raises(ValueError, match=r"'window_size' should be positive"):
+        df.with_columns(trailing_min=pl.col("x").rolling_min(window_size=-3))
+
+
+@typing.no_type_check
+def test_invalid_getitem_key_err() -> None:
+    df = pl.DataFrame({"x": [1.0], "y": [1.0]})
+
+    with pytest.raises(KeyError, match=r"('x', 'y')"):
+        df["x", "y"]
+
+
+def test_invalid_groupby_arg() -> None:
+    df = pl.DataFrame({"a": [1]})
+    with pytest.raises(
+        ValueError,
+        match=r"'aggs' argument should be one or multiple expressions, got: '{'a': 'sum'}'",
+    ):
+        df.groupby(1).agg({"a": "sum"})
+
+
+def test_no_sorted_warning(capfd: typing.Any) -> None:
+    df = pl.DataFrame(
+        {
+            "dt": [datetime(2001, 1, 1), datetime(2001, 1, 2)],
+        }
+    )
+    df.groupby_dynamic("dt", every="1h").agg(pl.all().count().suffix("_foo"))
+    (_, err) = capfd.readouterr()
+    assert "argument is not explicitly sorted" in err
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_expr_multi_cols.py` & `polars_lts_cpu-0.17.6/tests/unit/test_expr_multi_cols.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_exprs.py` & `polars_lts_cpu-0.17.6/tests/unit/test_exprs.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_fmt.py` & `polars_lts_cpu-0.17.6/tests/unit/test_fmt.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_functions.py` & `polars_lts_cpu-0.17.6/tests/unit/test_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -378,7 +378,11 @@
         pl.DataFrame({"b": pl.Series(values=[3], dtype=pl.UInt32)}),
     )
 
     assert_frame_equal(
         df1.select(pl.col("b").approx_unique()),
         pl.DataFrame({"b": pl.Series(values=[3], dtype=pl.UInt32)}),
     )
+
+
+def test_range_decreasing() -> None:
+    assert pl.arange(10, 1, -2, eager=True).to_list() == list(range(10, 1, -2))
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_interchange.py` & `polars_lts_cpu-0.17.6/tests/unit/test_interchange.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_interop.py` & `polars_lts_cpu-0.17.6/tests/unit/test_interop.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,91 +11,66 @@
 import pytest
 from numpy.testing import assert_array_equal
 
 import polars as pl
 from polars.testing import assert_frame_equal, assert_series_equal
 
 
-def test_df_from_numpy() -> None:
-    df = pl.DataFrame(
-        {
-            "int8": np.array([1, 3, 2], dtype=np.int8),
-            "int16": np.array([1, 3, 2], dtype=np.int16),
-            "int32": np.array([1, 3, 2], dtype=np.int32),
-            "int64": np.array([1, 3, 2], dtype=np.int64),
-            "uint8": np.array([1, 3, 2], dtype=np.uint8),
-            "uint16": np.array([1, 3, 2], dtype=np.uint16),
-            "uint32": np.array([1, 3, 2], dtype=np.uint32),
-            "uint64": np.array([1, 3, 2], dtype=np.uint64),
-            "float16": np.array([21.7, 21.8, 21], dtype=np.float16),
-            "float32": np.array([21.7, 21.8, 21], dtype=np.float32),
-            "float64": np.array([21.7, 21.8, 21], dtype=np.float64),
-            "intc": np.array([1, 3, 2], dtype=np.intc),
-            "uintc": np.array([1, 3, 2], dtype=np.uintc),
-            "str": np.array(["string1", "string2", "string3"], dtype=np.str_),
-            "bytes": np.array(
-                ["byte_string1", "byte_string2", "byte_string3"], dtype=np.bytes_
-            ),
-        }
-    )
-    out = [
-        pl.datatypes.Int8,
-        pl.datatypes.Int16,
-        pl.datatypes.Int32,
-        pl.datatypes.Int64,
-        pl.datatypes.UInt8,
-        pl.datatypes.UInt16,
-        pl.datatypes.UInt32,
-        pl.datatypes.UInt64,
-        # np.float16 gets converted to float32 as Rust does not support float16.
-        pl.datatypes.Float32,
-        pl.datatypes.Float32,
-        pl.datatypes.Float64,
-        pl.datatypes.Int32,
-        pl.datatypes.UInt32,
-        pl.datatypes.Utf8,
-        pl.datatypes.Binary,
-    ]
-    assert out == df.dtypes
-
-
-def test_to_numpy() -> None:
-    def test_series_to_numpy(
-        name: str,
-        values: list[object],
-        pl_dtype: type[pl.DataType],
-        np_dtype: (
-            type[np.signedinteger[Any]]
-            | type[np.unsignedinteger[Any]]
-            | type[np.floating[Any]]
-            | type[np.object_]
+@pytest.fixture(
+    params=[
+        ("int8", [1, 3, 2], pl.Int8, np.int8),
+        ("int16", [1, 3, 2], pl.Int16, np.int16),
+        ("int32", [1, 3, 2], pl.Int32, np.int32),
+        ("int64", [1, 3, 2], pl.Int64, np.int64),
+        ("uint8", [1, 3, 2], pl.UInt8, np.uint8),
+        ("uint16", [1, 3, 2], pl.UInt16, np.uint16),
+        ("uint32", [1, 3, 2], pl.UInt32, np.uint32),
+        ("uint64", [1, 3, 2], pl.UInt64, np.uint64),
+        ("float32", [21.7, 21.8, 21], pl.Float32, np.float32),
+        ("float64", [21.7, 21.8, 21], pl.Float64, np.float64),
+        ("bool", [True, False, False], pl.Boolean, np.bool_),
+        ("object", [21.7, "string1", object()], pl.Object, np.object_),
+        ("str", ["string1", "string2", "string3"], pl.Utf8, np.str_),
+        ("intc", [1, 3, 2], pl.Int32, np.intc),
+        ("uintc", [1, 3, 2], pl.UInt32, np.uintc),
+        ("str_fixed", ["string1", "string2", "string3"], pl.Utf8, np.str_),
+        (
+            "bytes",
+            [b"byte_string1", b"byte_string2", b"byte_string3"],
+            pl.Binary,
+            np.bytes_,
         ),
-    ) -> None:
-        pl_series_to_numpy_array = np.array(pl.Series(name, values, pl_dtype))
-        numpy_array = np.array(values, dtype=np_dtype)
-        assert_array_equal(pl_series_to_numpy_array, numpy_array)
-
-    test_series_to_numpy("int8", [1, 3, 2], pl.Int8, np.int8)
-    test_series_to_numpy("int16", [1, 3, 2], pl.Int16, np.int16)
-    test_series_to_numpy("int32", [1, 3, 2], pl.Int32, np.int32)
-    test_series_to_numpy("int64", [1, 3, 2], pl.Int64, np.int64)
-
-    test_series_to_numpy("uint8", [1, 3, 2], pl.UInt8, np.uint8)
-    test_series_to_numpy("uint16", [1, 3, 2], pl.UInt16, np.uint16)
-    test_series_to_numpy("uint32", [1, 3, 2], pl.UInt32, np.uint32)
-    test_series_to_numpy("uint64", [1, 3, 2], pl.UInt64, np.uint64)
-
-    test_series_to_numpy("float32", [21.7, 21.8, 21], pl.Float32, np.float32)
-    test_series_to_numpy("float64", [21.7, 21.8, 21], pl.Float64, np.float64)
-
-    test_series_to_numpy("str", ["string1", "string2", "string3"], pl.Utf8, np.object_)
-    # without pyarrow
-    arr = pl.Series(["a", "b", None]).to_numpy(use_pyarrow=False)
-    assert arr.dtype == np.dtype("O")
-    assert list(arr) == ["a", "b", None]
+    ]
+)
+@no_type_check
+def numpy_interop_test_data(request):
+    return request.param
+
+
+def test_df_from_numpy(numpy_interop_test_data: Any) -> None:
+    name, values, pl_dtype, np_dtype = numpy_interop_test_data
+    df = pl.DataFrame({name: np.array(values, dtype=np_dtype)})
+    assert [pl_dtype] == df.dtypes
+
+
+def test_asarray(numpy_interop_test_data: Any) -> None:
+    name, values, pl_dtype, np_dtype = numpy_interop_test_data
+    pl_series_to_numpy_array = np.asarray(pl.Series(name, values, pl_dtype))
+    numpy_array = np.asarray(values, dtype=np_dtype)
+    assert_array_equal(pl_series_to_numpy_array, numpy_array)
+
+
+@pytest.mark.parametrize("use_pyarrow", [True, False])
+def test_to_numpy(numpy_interop_test_data: Any, use_pyarrow: bool) -> None:
+    name, values, pl_dtype, np_dtype = numpy_interop_test_data
+    pl_series_to_numpy_array = pl.Series(name, values, pl_dtype).to_numpy(
+        use_pyarrow=use_pyarrow
+    )
+    numpy_array = np.asarray(values, dtype=np_dtype)
+    assert_array_equal(pl_series_to_numpy_array, numpy_array)
 
 
 def test_from_pandas() -> None:
     df = pd.DataFrame(
         {
             "bools": [False, True, False],
             "bools_nulls": [None, True, False],
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_lazy.py` & `polars_lts_cpu-0.17.6/tests/unit/test_lazy.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_polars_import.py` & `polars_lts_cpu-0.17.6/tests/unit/test_polars_import.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_predicates.py` & `polars_lts_cpu-0.17.6/tests/unit/test_predicates.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_projections.py` & `polars_lts_cpu-0.17.6/tests/unit/test_projections.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_queries.py` & `polars_lts_cpu-0.17.6/tests/unit/test_queries.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_rows.py` & `polars_lts_cpu-0.17.6/tests/unit/test_rows.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_schema.py` & `polars_lts_cpu-0.17.6/tests/unit/test_schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import typing
+
 import pytest
 
 import polars as pl
 from polars.testing import assert_frame_equal
 
 
 def test_schema_on_agg() -> None:
@@ -371,11 +373,83 @@
     df = pl.DataFrame({"a": [1.1, 2.3, 3.4, 4.5]}, schema={"a": pl.Float32()})
     assert df.with_columns(pl.col("a") - pl.col("a").median()).dtypes == [pl.Float32]
     assert df.with_columns(
         (pl.col("a") - pl.col("a").mean()) / (pl.col("a").std() + 0.001)
     ).dtypes == [pl.Float32]
 
 
-def test_bool_sum_schema() -> None:
-    assert pl.LazyFrame({"a": [True, False]}).select(pl.col("a").sum()).schema == {
-        "a": pl.UInt32
-    }
+def test_absence_off_null_prop_8224() -> None:
+    # a reminder to self to not do null propagation
+    # it is inconsistent and makes output dtype
+    # dependent of the data, big no!
+
+    def sub_col_min(column: str, min_column: str) -> pl.Expr:
+        return pl.col(column).sub(pl.col(min_column).min())
+
+    df = pl.DataFrame(
+        {
+            "group": [1, 1, 2, 2],
+            "vals_num": [10.0, 11.0, 12.0, 13.0],
+            "vals_partial": [None, None, 12.0, 13.0],
+            "vals_null": [None, None, None, None],
+        }
+    )
+
+    q = (
+        df.lazy()
+        .groupby("group")
+        .agg(
+            [
+                sub_col_min("vals_num", "vals_num").alias("sub_num"),
+                sub_col_min("vals_num", "vals_partial").alias("sub_partial"),
+                sub_col_min("vals_num", "vals_null").alias("sub_null"),
+            ]
+        )
+    )
+
+    assert q.collect().dtypes == [
+        pl.Int64,
+        pl.List(pl.Float64),
+        pl.List(pl.Float64),
+        pl.List(pl.Float64),
+    ]
+
+
+@typing.no_type_check
+def test_schemas() -> None:
+    # add all expression output tests here:
+    args = [
+        # coalesce
+        {
+            "data": {"x": ["x"], "y": ["y"]},
+            "expr": pl.coalesce(pl.col("x"), pl.col("y")),
+            "expected_select": {"x": pl.Utf8},
+            "expected_gb": {"x": pl.List(pl.Utf8)},
+        },
+        # boolean sum
+        {
+            "data": {"x": [True]},
+            "expr": pl.col("x").sum(),
+            "expected_select": {"x": pl.UInt32},
+            "expected_gb": {"x": pl.UInt32},
+        },
+    ]
+    for arg in args:
+        df = pl.DataFrame(arg["data"])
+
+        # test selection schema
+        schema = df.select(arg["expr"]).schema
+        for key, dtype in arg["expected_select"].items():
+            assert schema[key] == dtype
+
+        # test groupby schema
+        schema = df.groupby(pl.lit(1)).agg(arg["expr"]).schema
+        for key, dtype in arg["expected_gb"].items():
+            assert schema[key] == dtype
+
+
+def test_list_null_constructor_schema() -> None:
+    expected = pl.List(pl.Null)
+    assert pl.Series([[]]).dtype == expected
+    assert pl.Series([[]], dtype=pl.List).dtype == expected
+    assert pl.DataFrame({"a": [[]]}).dtypes[0] == expected
+    assert pl.DataFrame(schema={"a": pl.List}).dtypes[0] == expected
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_serde.py` & `polars_lts_cpu-0.17.6/tests/unit/test_serde.py`

 * *Files 22% similar despite different names*

```diff
@@ -80,7 +80,13 @@
 
 
 def test_pickle_lazyframe() -> None:
     q = pl.LazyFrame({"a": [1, 4, 3]}).sort("a")
 
     s = pickle.dumps(q)
     assert_frame_equal(pickle.loads(s).collect(), pl.DataFrame({"a": [1, 3, 4]}))
+
+
+def test_deser_empty_list() -> None:
+    s = pickle.loads(pickle.dumps(pl.Series([[[42.0]], []])))
+    assert s.dtype == pl.List(pl.List(pl.Float64))
+    assert s.to_list() == [[[42.0]], []]
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_series.py` & `polars_lts_cpu-0.17.6/tests/unit/test_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -848,14 +848,27 @@
 @pytest.mark.parametrize("idx", [[0, 2], (0, 2)])
 def test_set_list_and_tuple(idx: list[int] | tuple[int]) -> None:
     a = pl.Series("a", [1, 2, 3])
     a[idx] = 4
     assert_series_equal(a, pl.Series("a", [4, 2, 4]))
 
 
+def test_init_nested_tuple() -> None:
+    s1 = pl.Series("s", (1, 2, 3))
+    assert s1.to_list() == [1, 2, 3]
+
+    s2 = pl.Series("s", ((1, 2, 3),), dtype=pl.List(pl.UInt8))
+    assert s2.to_list() == [[1, 2, 3]]
+    assert s2.dtype == pl.List(pl.UInt8)
+
+    s3 = pl.Series("s", ((1, 2, 3), (1, 2, 3)), dtype=pl.List(pl.Int32))
+    assert s3.to_list() == [[1, 2, 3], [1, 2, 3]]
+    assert s3.dtype == pl.List(pl.Int32)
+
+
 def test_fill_null() -> None:
     s = pl.Series("a", [1, 2, None])
     assert_series_equal(s.fill_null(strategy="forward"), pl.Series("a", [1, 2, 2]))
     assert_series_equal(s.fill_null(14), pl.Series("a", [1, 2, 14], dtype=Int64))
 
     a = pl.Series("a", [0.0, 1.0, None, 2.0, None, 3.0])
 
@@ -1178,39 +1191,14 @@
         "null_count": "0",
     }
 
     with pytest.raises(ValueError):
         assert empty_s.describe()
 
 
-def test_is_in() -> None:
-    s = pl.Series(["a", "b", "c"])
-
-    out = s.is_in(["a", "b"])
-    assert out.to_list() == [True, True, False]
-
-    # Check if empty list is converted to pl.Utf8.
-    out = s.is_in([])
-    assert out.to_list() == [False]  # one element?
-
-    for x_y_z in (["x", "y", "z"], {"x", "y", "z"}):
-        out = s.is_in(x_y_z)
-        assert out.to_list() == [False, False, False]
-
-    df = pl.DataFrame({"a": [1.0, 2.0], "b": [1, 4], "c": ["e", "d"]})
-    assert df.select(pl.col("a").is_in(pl.col("b"))).to_series().to_list() == [
-        True,
-        False,
-    ]
-    assert df.select(pl.col("b").is_in([])).to_series().to_list() == [False]
-
-    with pytest.raises(pl.ComputeError, match=r"cannot compare"):
-        df.select(pl.col("b").is_in(["x", "x"]))
-
-
 def test_slice() -> None:
     s = pl.Series(name="a", values=[0, 1, 2, 3, 4, 5], dtype=pl.UInt8)
     for srs_slice, expected in (
         [s.slice(2, 3), [2, 3, 4]],
         [s.slice(4, 1), [4]],
         [s.slice(4, None), [4, 5]],
         [s.slice(3), [3, 4, 5]],
@@ -2472,14 +2460,17 @@
     s = pl.Series("a", [1])
     assert s.item() == 1
 
     s = pl.Series("a", [1, 2])
     with pytest.raises(ValueError):
         s.item()
 
+    assert s.item(0) == 1
+    assert s.item(-1) == 2
+
     s = pl.Series("a", [])
     with pytest.raises(ValueError):
         s.item()
 
 
 def test_ptr() -> None:
     # not much to test on the ptr value itself.
```

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_sql.py` & `polars_lts_cpu-0.17.6/tests/unit/test_sql.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_streaming.py` & `polars_lts_cpu-0.17.6/tests/unit/test_streaming.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/test_testing.py` & `polars_lts_cpu-0.17.6/tests/unit/test_testing.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/tests/unit/utils/test_utils.py` & `polars_lts_cpu-0.17.6/tests/unit/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `polars_lts_cpu-0.17.5/Cargo.lock` & `polars_lts_cpu-0.17.6/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  "getrandom",
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
 name = "alloc-no-stdlib"
 version = "2.0.4"
@@ -83,15 +83,15 @@
  "planus",
  "serde",
 ]
 
 [[package]]
 name = "arrow2"
 version = "0.17.0"
-source = "git+https://github.com/jorgecarleitao/arrow2?rev=1491c6e8f4fd100f53c358e4f3ef1536d9e75090#1491c6e8f4fd100f53c358e4f3ef1536d9e75090"
+source = "git+https://github.com/ritchie46/arrow2?branch=polars_2023-04-20#48c24de7ed852bfbac50d3923908043fdcde12a7"
 dependencies = [
  "ahash",
  "arrow-format",
  "avro-schema",
  "base64",
  "bytemuck",
  "chrono",
@@ -108,53 +108,53 @@
  "json-deserializer",
  "lexical-core",
  "lz4",
  "multiversion",
  "num-traits",
  "parquet2",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
  "rustc_version",
  "simdutf8",
  "streaming-iterator",
  "strength_reduce",
  "zstd",
 ]
 
 [[package]]
 name = "async-stream"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ad445822218ce64be7a341abfb0b1ea43b5c23aa83902542a4542e78309d8e5e"
+checksum = "cd56dd203fef61ac097dd65721a419ddccb106b2d2b70ba60a6b529f03961a51"
 dependencies = [
  "async-stream-impl",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-stream-impl"
-version = "0.3.4"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4655ae1a7b0cdf149156f780c5bf3f1352bc53cbd9e0a361a7ef7b22947e965"
+checksum = "16e62a023e7c117e27523144c5d2459f4397fcc3cab0085af8e2224f643a0193"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 1.0.109",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "async-trait"
 version = "0.1.68"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9ccdd8f2a161be9bd5c023df56f1b2a0bd1d83872ae53b71a84a12c9bf6e842"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "atoi"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f28d99ec8bfea296261ca1af174f24225171fea9664ba9003cbebee704810528"
@@ -245,15 +245,15 @@
 name = "bytemuck_derive"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fdde5c9cd29ebd706ce1b35600920a33550e402fc998a2e53ad3b42c3c47a192"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "14c189c53d098945499cdfa7ecc63567cf3886b3332b312a5b4585d8d3a6a610"
@@ -305,17 +305,17 @@
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "chrono-tz"
-version = "0.8.1"
+version = "0.8.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa48fa079165080f11d7753fd0bc175b7d391f276b965fe4b55bfad67856e463"
+checksum = "cf9cc2b23599e6d7479755f3594285efb3f74a1bdca7a7374948bc831e23a552"
 dependencies = [
  "chrono",
  "chrono-tz-build",
  "phf",
 ]
 
 [[package]]
@@ -406,17 +406,17 @@
 checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.7"
+version = "0.5.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf2b3e8478797446514c91ef04bafcb59faba183e621ad488df88983cc14128c"
+checksum = "a33c2bf77f2df06183c3aa30d1e96c0695a313d4f9c453cc3762a6db39f99200"
 dependencies = [
  "cfg-if",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
@@ -479,15 +479,15 @@
 [[package]]
 name = "ctor"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dd4056f63fce3b82d852c3da92b08ea59959890813a7f4ce9c0ff85b10cf301b"
 dependencies = [
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxx"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f61f1b6389c3fe1c316bf8a4dccc90a38208354b330925bce1f74a6c4756eb93"
@@ -506,15 +506,15 @@
 dependencies = [
  "cc",
  "codespan-reporting",
  "once_cell",
  "proc-macro2",
  "quote",
  "scratch",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "cxxbridge-flags"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7944172ae7e4068c533afbb984114a56c46e9ccddda550499caa222902c7f7bb"
@@ -523,15 +523,15 @@
 name = "cxxbridge-macro"
 version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2345488264226bf682893e25de0769f3360aac9957980ec49361b083ddaa5bc5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "dirs"
 version = "5.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dece029acd3353e3a58ac2e3eb3c8d6c35827a892edc6cc4138ef9c33df46ecd"
@@ -678,15 +678,15 @@
 name = "futures-macro"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89ca545a94061b6365f2c7355b4b32bd20df3ff95f02da9329b34ccc3bd6ee72"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f43be4fe21a13b9781a69afa4985b0f6ee0e1afab2c6f454a8cf30e2b2237b6e"
@@ -722,17 +722,17 @@
 checksum = "c31b6d751ae2c7f11320402d34e41349dd1016f8d5d45e48c4312bc8625af50c"
 dependencies = [
  "byteorder",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.8"
+version = "0.2.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c05aeb6a22b8f62540c194aac980f2115af067bfe15a0734d7277a768d396b31"
+checksum = "c85e1d9ab2eadba7e5040d4e09cbd6d072b76a557ad64e797c2cb9d4da21d7e4"
 dependencies = [
  "cfg-if",
  "js-sys",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "wasm-bindgen",
 ]
@@ -741,15 +741,15 @@
 name = "ghost"
 version = "0.1.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e77ac7b51b8e6313251737fcef4b1c01a2ea102bde68415b62c0ee9268fec357"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "git2"
 version = "0.16.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ccf7f68c2995f392c49fffb4f95ae2c873297830eb25c6bc4c114ce8f4562acc"
@@ -825,17 +825,17 @@
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.54"
+version = "0.1.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c17cc76786e99f8d2f055c11159e7f0091c42474dcc3189fbab96072e873e6d"
+checksum = "0722cd7114b7de04316e7ea5456a0bbb20e4adb46fd27a3697adb812cff0f37c"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows",
@@ -1037,17 +1037,17 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.140"
+version = "0.2.142"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "99227334921fae1a979cf0bfdfcc6b3e5ce376ef57e16fb6fb3ea2ed6095f80c"
+checksum = "6a987beff54b60ffa6d51982e1aa1146bc42f19bd26be28b0586f252fccf5317"
 
 [[package]]
 name = "libflate"
 version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97822bf791bd4d5b403713886a5fbe8bf49520fe78e323b0dc480ca1a03e50b0"
 dependencies = [
@@ -1081,17 +1081,17 @@
 name = "libm"
 version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "348108ab3fba42ec82ff6e9564fc4ca0247bdccdc68dd8af9764bbc79c3c8ffb"
 
 [[package]]
 name = "libmimalloc-sys"
-version = "0.1.31"
+version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef2c45001fb108f37d41bed8efd715769acb14674c1ce3e266ef0e317ef5f877"
+checksum = "43a558e3d911bc3c7bfc8c78bc580b404d6e51c1cefbf656e176a94b49b0df40"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "libz-sys"
@@ -1151,17 +1151,17 @@
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
 name = "matrixmultiply"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "add85d4dd35074e6fedc608f8c8f513a3548619a9024b751949ef0e8e45a4d84"
+checksum = "bb99c395ae250e1bf9133673f03ca9f97b7e71b705436bf8f089453445d1e9fe"
 dependencies = [
  "rawpointer",
 ]
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
@@ -1184,17 +1184,17 @@
 checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mimalloc"
-version = "0.1.35"
+version = "0.1.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92666043c712f7f5c756d07443469ddcda6dd971cc15258bb7f3c3216fd1b7aa"
+checksum = "3d88dad3f985ec267a3fcb7a1726f5cb1a7e8cad8b646e70a84f967210df23da"
 dependencies = [
  "libmimalloc-sys",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.6.2"
@@ -1258,17 +1258,17 @@
 checksum = "6d89e9874397a1f0a52fc1f197a8effd9735223cb2390e9dcc83ac6cd02923d0"
 dependencies = [
  "chrono",
 ]
 
 [[package]]
 name = "ntapi"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc51db7b362b205941f71232e56c625156eb9a929f8cf74a428fd5bc094a4afc"
+checksum = "e8a3895c6391c39d7fe7ebc444a87eb2991b2a0bc718fdabd071eec617fc68e4"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "num-complex"
 version = "0.4.3"
@@ -1735,24 +1735,24 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.55"
+version = "1.0.56"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1d0dd4be24fcdcfeaa12a432d588dc59bbad6cad3510c67e74a2b6b2fc950564"
+checksum = "2b63bdb0cd06f1f4dedf69b254734f9b45af66e4a031e42a7480257d9898b435"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "py-polars"
-version = "0.17.5"
+version = "0.17.6"
 dependencies = [
  "ahash",
  "built",
  "ciborium",
  "jemallocator",
  "lexical-core",
  "libc",
@@ -1769,17 +1769,17 @@
  "serde_json",
  "smartstring",
  "thiserror",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb848f80438f926a9ebddf0a539ed6065434fd7aae03a89312a9821f81b8501"
+checksum = "e3b1ac5b3731ba34fdaa9785f8d74d17448cd18f30cf19e0c7e7b1fdb5272109"
 dependencies = [
  "cfg-if",
  "indoc",
  "inventory",
  "libc",
  "memoffset",
  "parking_lot 0.12.1",
@@ -1787,55 +1787,55 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98a42e7f42e917ce6664c832d5eee481ad514c98250c49e0b03b20593e2c7ed0"
+checksum = "9cb946f5ac61bb61a5014924910d936ebd2b23b705f7a4a3c40b05c720b079a3"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-built"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "be6d574e0f8cab2cdd1eeeb640cbf845c974519fa9e9b62fa9c08ecece0ca5de"
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a0707f0ab26826fe4ccd59b69106e9df5e12d097457c7b8f9c0fd1d2743eec4d"
+checksum = "fd4d7c5337821916ea2a1d21d1092e8443cf34879e53a0ac653fbb98f44ff65c"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "978d18e61465ecd389e1f235ff5a467146dc4e3c3968b90d274fe73a5dd4a438"
+checksum = "a9d39c55dab3fc5a4b25bbd1ac10a2da452c4aca13bb450f22818a002e29648d"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.2"
+version = "0.18.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8e0e1128f85ce3fca66e435e08aa2089a2689c1c48ce97803e13f63124058462"
+checksum = "97daff08a4c48320587b5224cc98d609e3c27b6d437315bd40b605c98eeb5918"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
@@ -1933,30 +1933,36 @@
  "getrandom",
  "redox_syscall",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.3"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b1f693b24f6ac912f4893ef08244d70b6067480d2f1a46e950c9691e6749d1d"
+checksum = "ac6cf59af1067a3fb53fbe5c88c053764e930f932be1d71d3ffe032cbe147f59"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-syntax",
+ "regex-syntax 0.7.0",
 ]
 
 [[package]]
 name = "regex-syntax"
 version = "0.6.29"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
 
 [[package]]
+name = "regex-syntax"
+version = "0.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b6868896879ba532248f33598de5181522d8b3d9d724dfd230911e1a7d4822f5"
+
+[[package]]
 name = "rle-decode-fast"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3582f63211428f83597b51b2ddb88e2a91a9d52d12831f9d08f5e624e8977422"
 
 [[package]]
 name = "rustc-hash"
@@ -2010,37 +2016,37 @@
 name = "seq-macro"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6b44e8fc93a14e66336d230954dda83d18b4605ccace8fe09bc7514a71ad0bc"
 
 [[package]]
 name = "serde"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3c04e8343c3daeec41f58990b9d77068df31209f2af111e059e9fe9646693065"
+checksum = "bb2f3770c8bce3bcda7e149193a069a0f4365bda1fa5cd88e03bca26afc1216c"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.159"
+version = "1.0.160"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c614d17805b093df4b147b51339e7e44bf05ef59fba1e45d83500bcfb4d8585"
+checksum = "291a097c63d8497e00160b166a967a4a79c64f3facdd01cbd7502231688d77df"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.95"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d721eca97ac802aa7777b701877c8004d950fc142651367300d21c1cc0194744"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "indexmap",
  "itoa",
  "ryu",
  "serde",
 ]
 
@@ -2073,15 +2079,15 @@
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simd-json"
 version = "0.7.0"
-source = "git+https://github.com/ritchie46/simd-json?branch=alignment#8e8d7c67d781f48ccecddf8d8dea318a0a37c019"
+source = "git+https://github.com/ritchie46/simd-json?branch=alignment#cbd37361769d900620944618a39123f37edf3d83"
 dependencies = [
  "halfbrown",
  "lexical-core",
  "serde",
  "serde_json",
  "simdutf8",
  "value-trait",
@@ -2206,17 +2212,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.13"
+version = "2.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c9da457c5285ac1f936ebd076af6dac17a61cfe7826f2076b4d015cf47bc8ec"
+checksum = "a34fcf3e8b60f57e6a14301a2e916d323af98b0ea63c599441eec8558660c822"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2267,15 +2273,15 @@
 name = "thiserror-impl"
 version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.13",
+ "syn 2.0.15",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -2523,88 +2529,145 @@
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
-version = "0.46.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cdacb41e6a96a052c6cb63a144f24900236121c6f63f4f8219fef5977ecb0c25"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.0",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.45.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "75283be5efb2831d37ea142365f009c02ec203cd29a3ebecbc093d52315b66d0"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.42.2",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
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
 name = "xxhash-rust"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "735a71d46c4d68d71d4b24d03fdc2b98e38cea81730595801db779c04fe80d70"
 
 [[package]]
 name = "zstd"
@@ -2613,25 +2676,25 @@
 checksum = "76eea132fb024e0e13fd9c2f5d5d595d8a967aa72382ac2f9d39fcc95afd0806"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "6.0.4+zstd.1.5.4"
+version = "6.0.5+zstd.1.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7afb4b54b8910cf5447638cb54bf4e8a65cbedd783af98b98c62ffe91f185543"
+checksum = "d56d9e60b4b1758206c238a10165fbcae3ca37b01744e394c463463f6529d23b"
 dependencies = [
  "libc",
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.7+zstd.1.5.4"
+version = "2.0.8+zstd.1.5.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94509c3ba2fe55294d752b79842c530ccfab760192521df74a081a78d2b3c7f5"
+checksum = "5556e6ee25d32df2586c098bbfa278803692a20d0ab9565e049480d52707ec8c"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
 ]
```

### Comparing `polars_lts_cpu-0.17.5/PKG-INFO` & `polars_lts_cpu-0.17.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polars-lts-cpu
-Version: 0.17.5
+Version: 0.17.6
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -13,51 +13,51 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: typing_extensions >= 4.0.1; python_version < '3.11'
-Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
-Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
+Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
+Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
+Requires-Dist: connectorx; extra == 'connectorx'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow'
 Requires-Dist: pyarrow>=7.0.0; extra == 'pandas'
 Requires-Dist: pandas; extra == 'pandas'
-Requires-Dist: connectorx; extra == 'connectorx'
+Requires-Dist: fsspec; extra == 'fsspec'
 Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv'
-Requires-Dist: matplotlib; extra == 'matplotlib'
 Requires-Dist: sqlalchemy; extra == 'sqlalchemy'
 Requires-Dist: pandas; extra == 'sqlalchemy'
-Requires-Dist: fsspec; extra == 'fsspec'
-Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra == 'timezone'
-Requires-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone'
+Requires-Dist: matplotlib; extra == 'matplotlib'
 Requires-Dist: xlsxwriter; extra == 'xlsxwriter'
-Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
-Provides-Extra: all
-Provides-Extra: deltalake
+Requires-Dist: polars[pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter]; extra == 'all'
+Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
+Provides-Extra: numpy
+Provides-Extra: timezone
+Provides-Extra: connectorx
 Provides-Extra: pyarrow
 Provides-Extra: pandas
-Provides-Extra: connectorx
+Provides-Extra: fsspec
 Provides-Extra: xlsx2csv
-Provides-Extra: matplotlib
 Provides-Extra: sqlalchemy
-Provides-Extra: fsspec
-Provides-Extra: timezone
+Provides-Extra: matplotlib
 Provides-Extra: xlsxwriter
-Provides-Extra: numpy
+Provides-Extra: all
+Provides-Extra: deltalake
 License-File: LICENSE
 Summary: Blazingly fast DataFrame library
 Keywords: dataframe,arrow,out-of-core
 Author-email: Ritchie Vink <ritchie46@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Changelog, https://github.com/pola-rs/polars/releases
-Project-URL: Repository, https://github.com/pola-rs/polars
 Project-URL: Homepage, https://www.pola.rs/
+Project-URL: Changelog, https://github.com/pola-rs/polars/releases
 Project-URL: Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/index.html
+Project-URL: Repository, https://github.com/pola-rs/polars
 
 <h1 align="center">
   <img src="https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/polars_github_logo_rect_dark_name.svg">
   <br>
 </h1>
 
 <div align="center">
@@ -72,33 +72,40 @@
   </a>
   <a href="https://pypi.org/project/polars/">
     <img src="https://img.shields.io/pypi/v/polars.svg" alt="PyPi Latest Release"/>
   </a>
   <a href="https://www.npmjs.com/package/nodejs-polars">
     <img src="https://img.shields.io/npm/v/nodejs-polars.svg" alt="NPM Latest Release"/>
   </a>
+  <a href="https://rpolars.r-universe.dev">
+    <img src="https://rpolars.r-universe.dev/badges/polars" alt="R-universe Latest Release"/>
+  </a>
   <a href="https://doi.org/10.5281/zenodo.7697217">
     <img src="https://zenodo.org/badge/DOI/10.5281/zenodo.7697217.svg" alt="DOI Latest Release"/>
   </a>
 </div>
 
 <p align="center">
   <b>Documentation</b>:
   <a href="https://pola-rs.github.io/polars/py-polars/html/reference/index.html">Python</a>
   -
   <a href="https://pola-rs.github.io/polars/polars/index.html">Rust</a>
   -
   <a href="https://pola-rs.github.io/nodejs-polars/index.html">Node.js</a>
+  -
+  <a href="https://rpolars.github.io/index.html">R</a>
   |
   <b>StackOverflow</b>:
   <a href="https://stackoverflow.com/questions/tagged/python-polars">Python</a>
   -
   <a href="https://stackoverflow.com/questions/tagged/rust-polars">Rust</a>
   -
   <a href="https://stackoverflow.com/questions/tagged/nodejs-polars">Node.js</a>
+  -
+  <a href="https://stackoverflow.com/questions/tagged/r-polars">R</a>
   |
   <a href="https://pola-rs.github.io/polars-book/">User Guide</a>
   |
   <a href="https://discord.gg/4UfP5cfBE7">Discord</a>
 </p>
 
 ## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL
@@ -108,15 +115,15 @@
 
 - Lazy | eager execution
 - Multi-threaded
 - SIMD
 - Query optimization
 - Powerful expression API
 - Hybrid Streaming (larger than RAM datasets)
-- Rust | Python | NodeJS | ...
+- Rust | Python | NodeJS | R | ...
 
 To learn more, read the [User Guide](https://pola-rs.github.io/polars-book/).
 
 ## Python
 
 ```python
 >>> import polars as pl
@@ -187,20 +194,37 @@
 >>> (lf.join(other_table)
 ...      .groupby("foo")
 ...      .agg(
 ...     pl.col("sum_v1").count()
 ... ).collect())
 ```
 
+SQL commands can also be ran directly from your terminal.
+
+```bash
+> cargo install polars-cli --locked
+# run an inline sql query
+> polars -c "SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE id1 = 'id016' LIMIT 10"
+
+# run interactively
+> polars
+Polars CLI v0.1.0
+Type .help for help.
+
+> SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE id1 = 'id016' LIMIT 10;
+```
+
+Refer to [polars-cli](./polars-cli/README.md) for more information.
+
 ## Performance 🚀🚀
 
 ### Blazingly fast
 
 Polars is very fast. In fact, it is one of the best performing solutions available.
-See the results in [h2oai's db-benchmark](https://h2oai.github.io/db-benchmark/).
+See the results in [DuckDB's db-benchmark](https://duckdblabs.github.io/db-benchmark/).
 
 In the [TPCH benchmarks](https://www.pola.rs/benchmarks.html) polars is orders of magnitudes faster than pandas, dask, modin and vaex
 on full queries (including IO).
 
 ### Lightweight
 
 Polars is also very lightweight. It comes with zero required dependencies, and this shows in the import times:
```

#### html2text {}

```diff
@@ -1,56 +1,57 @@
-Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.5 Classifier:
+Metadata-Version: 2.1 Name: polars-lts-cpu Version: 0.17.6 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Rust Classifier: Topic ::
 Scientific/Engineering Requires-Dist: typing_extensions >= 4.0.1;
-python_version < '3.11' Requires-Dist: polars
+python_version < '3.11' Requires-Dist: numpy >= 1.16.0; extra == 'numpy'
+Requires-Dist: backports.zoneinfo; (python_version < '3.9') and extra ==
+'timezone' Requires-Dist: tzdata; (platform_system == 'Windows') and extra ==
+'timezone' Requires-Dist: connectorx; extra == 'connectorx' Requires-Dist:
+pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist: pyarrow>=7.0.0; extra ==
+'pandas' Requires-Dist: pandas; extra == 'pandas' Requires-Dist: fsspec; extra
+== 'fsspec' Requires-Dist: xlsx2csv >= 0.8.0; extra == 'xlsx2csv' Requires-
+Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra ==
+'sqlalchemy' Requires-Dist: matplotlib; extra == 'matplotlib' Requires-Dist:
+xlsxwriter; extra == 'xlsxwriter' Requires-Dist: polars
 [pyarrow,pandas,numpy,fsspec,connectorx,xlsx2csv,deltalake,timezone,matplotlib,sqlalchemy,xlsxwriter];
 extra == 'all' Requires-Dist: deltalake >= 0.8.0; extra == 'deltalake'
-Requires-Dist: pyarrow>=7.0.0; extra == 'pyarrow' Requires-Dist:
-pyarrow>=7.0.0; extra == 'pandas' Requires-Dist: pandas; extra == 'pandas'
-Requires-Dist: connectorx; extra == 'connectorx' Requires-Dist: xlsx2csv >=
-0.8.0; extra == 'xlsx2csv' Requires-Dist: matplotlib; extra == 'matplotlib'
-Requires-Dist: sqlalchemy; extra == 'sqlalchemy' Requires-Dist: pandas; extra
-== 'sqlalchemy' Requires-Dist: fsspec; extra == 'fsspec' Requires-Dist:
-backports.zoneinfo; (python_version < '3.9') and extra == 'timezone' Requires-
-Dist: tzdata; (platform_system == 'Windows') and extra == 'timezone' Requires-
-Dist: xlsxwriter; extra == 'xlsxwriter' Requires-Dist: numpy >= 1.16.0; extra
-== 'numpy' Provides-Extra: all Provides-Extra: deltalake Provides-Extra:
-pyarrow Provides-Extra: pandas Provides-Extra: connectorx Provides-Extra:
-xlsx2csv Provides-Extra: matplotlib Provides-Extra: sqlalchemy Provides-Extra:
-fsspec Provides-Extra: timezone Provides-Extra: xlsxwriter Provides-Extra:
-numpy License-File: LICENSE Summary: Blazingly fast DataFrame library Keywords:
+Provides-Extra: numpy Provides-Extra: timezone Provides-Extra: connectorx
+Provides-Extra: pyarrow Provides-Extra: pandas Provides-Extra: fsspec Provides-
+Extra: xlsx2csv Provides-Extra: sqlalchemy Provides-Extra: matplotlib Provides-
+Extra: xlsxwriter Provides-Extra: all Provides-Extra: deltalake License-File:
+LICENSE Summary: Blazingly fast DataFrame library Keywords:
 dataframe,arrow,out-of-core Author-email: Ritchie Vink
 gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown;
-charset=UTF-8; variant=GFM Project-URL: Changelog, https://github.com/pola-rs/
-polars/releases Project-URL: Repository, https://github.com/pola-rs/polars
-Project-URL: Homepage, https://www.pola.rs/ Project-URL: Documentation, https:/
-/pola-rs.github.io/polars/py-polars/html/reference/index.html
+charset=UTF-8; variant=GFM Project-URL: Homepage, https://www.pola.rs/ Project-
+URL: Changelog, https://github.com/pola-rs/polars/releases Project-URL:
+Documentation, https://pola-rs.github.io/polars/py-polars/html/reference/
+index.html Project-URL: Repository, https://github.com/pola-rs/polars
  ****** [https://raw.githubusercontent.com/pola-rs/polars-static/master/logos/
                     polars_github_logo_rect_dark_name.svg]
                                      ******
 [rust_docs] [Build_and_test] [https://img.shields.io/crates/v/polars.svg] [PyPi
-           Latest_Release] [NPM_Latest_Release] [DOI_Latest_Release]
-Documentation: Python - Rust - Node.js | StackOverflow: Python - Rust - Node.js
-                            | User_Guide | Discord
+ Latest_Release] [NPM_Latest_Release] [R-universe_Latest_Release] [DOI_Latest
+                                   Release]
+  Documentation: Python - Rust - Node.js - R | StackOverflow: Python - Rust -
+                      Node.js - R | User_Guide | Discord
 ## Polars: Blazingly fast DataFrames in Rust, Python, Node.js, R and SQL Polars
 is a DataFrame interface on top of an OLAP Query Engine implemented in Rust
 using [Apache Arrow Columnar Format](https://arrow.apache.org/docs/format/
 Columnar.html) as the memory model. - Lazy | eager execution - Multi-threaded -
 SIMD - Query optimization - Powerful expression API - Hybrid Streaming (larger
-than RAM datasets) - Rust | Python | NodeJS | ... To learn more, read the [User
-Guide](https://pola-rs.github.io/polars-book/). ## Python ```python >>> import
-polars as pl >>> df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ...
+than RAM datasets) - Rust | Python | NodeJS | R | ... To learn more, read the
+[User Guide](https://pola-rs.github.io/polars-book/). ## Python ```python >>>
+import polars as pl >>> df = pl.DataFrame( ... { ... "A": [1, 2, 3, 4, 5], ...
 "fruits": ["banana", "banana", "apple", "apple", "banana"], ... "B": [5, 4, 3,
 2, 1], ... "cars": ["beetle", "audi", "beetle", "beetle", "beetle"], ... } ...
 ) # embarrassingly parallel execution & very expressive query language >>>
 df.sort("fruits").select( ... "fruits", ... "cars", ... pl.lit("fruits").alias
 ("literal_string_fruits"), ... pl.col("B").filter(pl.col("cars") ==
 "beetle").sum(), ... pl.col("A").filter(pl.col("B") > 2).sum().over
 ("cars").alias("sum_A_by_cars"), ... pl.col("A").sum().over("fruits").alias
@@ -78,48 +79,55 @@
 materialization >>> context.query(query) shape: (1, 2)
 ââââââââââ¬âââââââââ â sum_v1 â min_v2
 â â --- â --- â â i64 â i64 â
 ââââââââââªâââââââââ¡ â 298268 â 1 â
 ââââââââââ´âââââââââ >>> ## OPTION 2 >>> #
 Don't materialize the query, but return as LazyFrame >>> # and continue in
 python >>> lf = context.execute(query) >>> (lf.join(other_table) ... .groupby
-("foo") ... .agg( ... pl.col("sum_v1").count() ... ).collect()) ``` ##
-Performance ðð ### Blazingly fast Polars is very fast. In fact, it is one
-of the best performing solutions available. See the results in [h2oai's db-
-benchmark](https://h2oai.github.io/db-benchmark/). In the [TPCH benchmarks]
-(https://www.pola.rs/benchmarks.html) polars is orders of magnitudes faster
-than pandas, dask, modin and vaex on full queries (including IO). ###
-Lightweight Polars is also very lightweight. It comes with zero required
-dependencies, and this shows in the import times: - polars: 70ms - numpy: 104ms
-- pandas: 520ms ### Handles larger than RAM data If you have data that does not
-fit into memory, polars lazy is able to process your query (or parts of your
-query) in a streaming fashion, this drastically reduces memory requirements so
-you might be able to process your 250GB dataset on your laptop. Collect with
-`collect(streaming=True)` to run the query streaming. (This might be a little
-slower, but it is still very fast!) ## Setup ### Python Install the latest
-polars version with: ```sh pip install polars ``` We also have a conda package
-(`conda install -c conda-forge polars`), however pip is the preferred way to
-install Polars. Install Polars with all optional dependencies. ```sh pip
-install 'polars[all]' pip install 'polars[numpy,pandas,pyarrow]' # install a
-subset of all optional dependencies ``` You can also install the dependencies
-directly. | Tag | Description | | ---------- | --------------------------------
--------------------------------------------------------------------------------
----------------------- | | all | Install all optional dependencies (all of the
-following) | | pandas | Install with Pandas for converting data to and from
-Pandas Dataframes/Series | | numpy | Install with numpy for converting data to
-and from numpy arrays | | pyarrow | Reading data formats using PyArrow | |
-fsspec | Support for reading from remote file systems | | connectorx | Support
-for reading from SQL databases | | xlsx2csv | Support for reading from Excel
-files | | deltalake | Support for reading from Delta Lake Tables | | timezone |
-Timezone support, only needed if 1. you are on Python < 3.9 and/or 2. you are
-on Windows, otherwise no dependencies will be installed | Releases happen quite
-often (weekly / every few days) at the moment, so updating polars regularly to
-get the latest bugfixes / features might not be a bad idea. ### Rust You can
-take latest release from `crates.io`, or if you want to use the latest features
-/ performance improvements point to the `main` branch of this repo. ```toml
+("foo") ... .agg( ... pl.col("sum_v1").count() ... ).collect()) ``` SQL
+commands can also be ran directly from your terminal. ```bash > cargo install
+polars-cli --locked # run an inline sql query > polars -c "SELECT sum(v1) as
+sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE id1 = 'id016' LIMIT
+10" # run interactively > polars Polars CLI v0.1.0 Type .help for help. >
+SELECT sum(v1) as sum_v1, min(v2) as min_v2 FROM read_ipc('file.arrow') WHERE
+id1 = 'id016' LIMIT 10; ``` Refer to [polars-cli](./polars-cli/README.md) for
+more information. ## Performance ðð ### Blazingly fast Polars is very
+fast. In fact, it is one of the best performing solutions available. See the
+results in [DuckDB's db-benchmark](https://duckdblabs.github.io/db-benchmark/).
+In the [TPCH benchmarks](https://www.pola.rs/benchmarks.html) polars is orders
+of magnitudes faster than pandas, dask, modin and vaex on full queries
+(including IO). ### Lightweight Polars is also very lightweight. It comes with
+zero required dependencies, and this shows in the import times: - polars: 70ms
+- numpy: 104ms - pandas: 520ms ### Handles larger than RAM data If you have
+data that does not fit into memory, polars lazy is able to process your query
+(or parts of your query) in a streaming fashion, this drastically reduces
+memory requirements so you might be able to process your 250GB dataset on your
+laptop. Collect with `collect(streaming=True)` to run the query streaming.
+(This might be a little slower, but it is still very fast!) ## Setup ### Python
+Install the latest polars version with: ```sh pip install polars ``` We also
+have a conda package (`conda install -c conda-forge polars`), however pip is
+the preferred way to install Polars. Install Polars with all optional
+dependencies. ```sh pip install 'polars[all]' pip install 'polars
+[numpy,pandas,pyarrow]' # install a subset of all optional dependencies ``` You
+can also install the dependencies directly. | Tag | Description | | ---------
+- | ---------------------------------------------------------------------------
+---------------------------------------------------------- | | all | Install
+all optional dependencies (all of the following) | | pandas | Install with
+Pandas for converting data to and from Pandas Dataframes/Series | | numpy |
+Install with numpy for converting data to and from numpy arrays | | pyarrow |
+Reading data formats using PyArrow | | fsspec | Support for reading from remote
+file systems | | connectorx | Support for reading from SQL databases | |
+xlsx2csv | Support for reading from Excel files | | deltalake | Support for
+reading from Delta Lake Tables | | timezone | Timezone support, only needed if
+1. you are on Python < 3.9 and/or 2. you are on Windows, otherwise no
+dependencies will be installed | Releases happen quite often (weekly / every
+few days) at the moment, so updating polars regularly to get the latest
+bugfixes / features might not be a bad idea. ### Rust You can take latest
+release from `crates.io`, or if you want to use the latest features /
+performance improvements point to the `main` branch of this repo. ```toml
 polars = { git = "https://github.com/pola-rs/polars", rev = "" } ``` Required
 Rust version `>=1.62` ## Contributing Want to contribute? Read our
 [contribution guideline](./CONTRIBUTING.md). ## Python: compile polars from
 source If you want a bleeding edge release or maximal performance you should
 compile **polars** from source. This can be done by going through the following
 steps in sequence: 1. Install the latest [Rust compiler](https://www.rust-
 lang.org/tools/install) 2. Install [maturin](https://maturin.rs/): `pip install
```

