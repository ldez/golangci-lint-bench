# Benchmark golangci-lint

Open an [issue](https://github.com/ldez/golangci-lint-bench/issues/new/choose) to run the benchmarks.

## Notes

GitHub Actions are not an isolated environment so statistical outliers can happen.

I use issues (`labeled` event) instead of `workflow_dispatch` as trigger because it allows to have easily only one issue for a PR (if you need to run the benchmark several times).

I use issues (`labeled` event) instead of issue comments to limit the number of useless triggers on all comments.

One approach can be to use `workflow_dispatch` as trigger and add the comments inside the targeted PR, this will work for PR, but the benchmark of all linters (not related to a PR) will not work.
