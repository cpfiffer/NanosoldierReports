# NanosoldierReports

[![github pages](https://github.com/JuliaCI/NanosoldierReports/workflows/github%20pages/badge.svg)](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html)

This repository stores markdown reports generated by the [Nanosoldier.jl](https://github.com/JuliaCI/Nanosoldier.jl) CI system.

## Benchmark reports

Benchmark reports compare the performance of two builds of Julia on [select benchmarks](https://github.com/JuliaCI/BaseBenchmarks.jl/) using the [BenchmarkTools.jl](https://github.com/JuliaCI/BenchmarkTools.jl) infrastructure.

If you use Chrome to view these reports, it's recommended that you install the [Wide GitHub Chrome extension](https://chrome.google.com/webstore/detail/wide-github/kaalofacklcidaampbokdplbklpeldpj?hl=en) for the best report-viewing experience.

## PkgEval reports

PkgEval reports run the tests of all registered packages using the [PkgEval.jl](https://github.com/JuliaCI/PkgEval.jl) infrastructure. The reports are grouped in two folder: `by_date`, for daily evaluations of the current Julia master branch, and `by_hash` for specifically requested builds (e.g., on a pull request to determine breakage of a change).

Click [here](https://juliaci.github.io/NanosoldierReports/pkgeval_badges/report.html) to open the latest daily report.

### Badges

The test results of the latest daily is also used to generate a PkgEval badge. You can use these badges in your package's README to keep track of PkgEval-compatibility, which is important to make sure that your package is taken into account when evaluating changes to Julia itself.

Use the following code to embed the PkgEval badge and a link to the latest report (changing `E/Example` to your package name, prefixed by its initial):

```
[pkgeval-img]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.svg
[pkgeval-url]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img]][pkgeval-url]
```

The result will look as follows:

[pkgeval-img-1]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.svg
[pkgeval-url-1]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img-1]][pkgeval-url-1]

Alternatively, you can embed a badge that includes the name of your package in the badge itself. Use the following code (changing `E/Example` to your package name, prefixed by its initial):

```
[pkgeval-img]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.named.svg
[pkgeval-url]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img]][pkgeval-url]
```

The result will look as follows:

[pkgeval-img-2]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.named.svg
[pkgeval-url-2]: https://juliaci.github.io/NanosoldierReports/pkgeval_badges/E/Example.html

[![PkgEval][pkgeval-img-2]][pkgeval-url-2]
