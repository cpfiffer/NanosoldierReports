# NanosoldierReports

[![GitHub pages](https://github.com/JuliaCI/NanosoldierReports/actions/workflows/pages.yml/badge.svg)](https://github.com/JuliaCI/NanosoldierReports/actions/workflows/pages.yml) [![latest PkgEval report](https://img.shields.io/badge/PkgEval-latest%20report-green)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html)

This repository stores data and markdown reports generated by the
[Nanosoldier.jl](https://github.com/JuliaCI/Nanosoldier.jl) CI system.


## Benchmark reports

Benchmark reports compare the performance of two builds of Julia on [select
benchmarks](https://github.com/JuliaCI/BaseBenchmarks.jl/) using the
[BenchmarkTools.jl](https://github.com/JuliaCI/BenchmarkTools.jl) infrastructure. The
reports are grouped in two folder: `by_date`, for daily evaluations of the current Julia
master branch, and `by_hash` for specifically requested jobs (e.g., on a pull request).

If you use Chrome to view these reports, it's recommended that you install the [Wide GitHub
Chrome
extension](https://chrome.google.com/webstore/detail/wide-github/kaalofacklcidaampbokdplbklpeldpj?hl=en)
for the best report-viewing experience.


## PkgEval reports

PkgEval reports run the tests of all registered packages using the
[PkgEval.jl](https://github.com/JuliaCI/PkgEval.jl) infrastructure. Similar to benchmark
reports, they are grouped in `by_date` and `by_hash` folders.

Click [here](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) to
open the latest daily report.

### Charts

History test data is visualized in charts that are generated for every push to this
repository, and are meant to make it easy to keep an eye on the state of the Julia package
ecosystem and its compatibility with the current development version of Julia:

![Overview of daily PkgEval test
results](https://github.com/JuliaCI/NanosoldierReports/raw/gh-pages/pkgeval_charts/daily.png)

We also keep track of the time it takes to test packages. The chart below visualizes the time
it takes to test all packages, relative to the latest master:

![Package test time
visualization](https://github.com/JuliaCI/NanosoldierReports/raw/gh-pages/pkgeval_charts/daily_time_full.png)

### Badges

The test results of the latest daily is also used to generate a PkgEval badge. You can use
these badges in your package's README to keep track of PkgEval-compatibility, which is
important to make sure that your package is taken into account when evaluating changes to
Julia itself.

Use the following code to embed the PkgEval badge and a link to the latest report (changing
`E/Example` to your package name, prefixed by its initial):

```
[pkgeval-img]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.svg
[pkgeval-url]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img]][pkgeval-url]
```

The result will look as follows:

[pkgeval-img-1]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.svg
[pkgeval-url-1]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img-1]][pkgeval-url-1]

Alternatively, you can embed a badge that includes the name of your package in the badge
itself. Use the following code (changing `E/Example` to your package name, prefixed by its
initial):

```
[pkgeval-img]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.named.svg
[pkgeval-url]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img]][pkgeval-url]
```

The result will look as follows:

[pkgeval-img-2]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.named.svg
[pkgeval-url-2]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img-2]][pkgeval-url-2]
