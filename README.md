# HPX performance history

The results of the performance tests of [HPX](https://github.com/TheHPXProject/hpx) for the commits of its master branch, measured by its Jenkins CI on the Rostam cluster at LSU (see `.jenkins/lsu-perftests` and `tools/perftests_ci` in the HPX repository). The graphs below show the median time of every measurement over the date of the commit; lower is faster.

## Layout

- `<year>/<node>/<commit date>-<commit>-b<build>/`: one run, with its report (`README.md`), the commit, when and where the benchmarks ran and the configuration (`metadata.json`), the medians of all measurements (`summary.json`), the results of all benchmarks as measured (`results.tar.gz`), and the comparison with the references of the node.
- `runs.tsv`: all runs. `timeline.csv`: the medians of all measurements of all runs, as written by `tools/perftests_ci/perftests_history.py`, which rebuilds it from the run directories. `timeline/`: the graphs below, drawn by `tools/perftests_ci/perftests_timeline.py`.

## Runs

- [2026](2026/README.md)

## Performance over time

### benchmark_inplace_merge

![benchmark_inplace_merge](timeline/benchmark_inplace_merge.svg)

### benchmark_is_heap

![benchmark_is_heap](timeline/benchmark_is_heap.svg)

### benchmark_is_heap_until

![benchmark_is_heap_until](timeline/benchmark_is_heap_until.svg)

### benchmark_merge

![benchmark_merge](timeline/benchmark_merge.svg)

### benchmark_nth_element

![benchmark_nth_element](timeline/benchmark_nth_element.svg)

### benchmark_nth_element_parallel

![benchmark_nth_element_parallel](timeline/benchmark_nth_element_parallel.svg)

### benchmark_partial_sort

![benchmark_partial_sort](timeline/benchmark_partial_sort.svg)

### benchmark_partial_sort_parallel

![benchmark_partial_sort_parallel](timeline/benchmark_partial_sort_parallel.svg)

### benchmark_remove

![benchmark_remove](timeline/benchmark_remove.svg)

### benchmark_remove_if

![benchmark_remove_if](timeline/benchmark_remove_if.svg)

### foreach_report

![foreach_report](timeline/foreach_report.svg)

### future_overhead_report

![future_overhead_report](timeline/future_overhead_report.svg)

### small_vector_benchmark

![small_vector_benchmark](timeline/small_vector_benchmark.svg)

### stream_report

![stream_report](timeline/stream_report.svg)

### transform_reduce_scaling

![transform_reduce_scaling](timeline/transform_reduce_scaling.svg)

## License

Distributed under the Boost Software License, Version 1.0, see [LICENSE_1_0.txt](LICENSE_1_0.txt).
