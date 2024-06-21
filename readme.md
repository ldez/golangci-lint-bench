# Benchmark golangci-lint

Open an [issue](https://github.com/ldez/golangci-lint-bench/issues/new/choose) to run the benchmarks.

## Notes

GitHub Actions are not an isolated environment so statistical outliers can happen.

I use issues (`labeled` event) instead of `workflow_dispatch` as trigger because it allows to have easily only one issue for a PR (if you need to run the benchmark several times).

I use issues (`labeled` event) instead of issue comments to limit the number of useless triggers on all comments.
