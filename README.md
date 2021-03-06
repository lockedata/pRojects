
# starters <img src="man/figures/logo.png" align="right" height=140/>

<!-- README.md is generated from README.Rmd. Please edit that file -->

<!-- badges: start -->

[![Build
Status](https://travis-ci.org/lockedata/starters.svg?branch=master)](https://travis-ci.org/lockedata/starters)
[![Coverage
Status](https://img.shields.io/coveralls/lockedata/starters.svg)](https://coveralls.io/r/lockedata/starters?branch=master)
[![Locke Data
Slack](https://img.shields.io/badge/Slack-discuss-blue.svg?logo=slack&longCache=true&style=flat)](https://join.slack.com/t/lockedata/shared_invite/enQtMjkwNjY3ODkwMzg2LTI1OGU1NTM3ZGIyZGFiNTdlODI3MzU2N2ZlNDczMjM4M2U2OWVmNDMzZTQ1ZGNlZDQ3MGM2MGVjMjI2MWIyMjI)
[![Project Status: Active - The project has reached a stable, usable
state and is being actively
developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
<!-- badges: end -->

This package is designed to take away some grunt work around setting up
new projects.

All projects get setup with Git, GitHub and Travis by default.

  - Use `create_package_project()` to setup a project with code
    coverage, vignettes, unit testing etc. out of the box

  - Use `create_analysis_project()` to get a project ready for a typical
    analysis project. It includes
    [renv](https://rstudio.github.io/renv/articles/renv.html) to help
    with reproducibility.

  - Use `create_training_project()` to get a project ready for
    delivering training that often involves handouts and presentation
    materials. It includes
    [renv](https://rstudio.github.io/renv/articles/renv.html) to help
    with reproducibility.

All functions implement name validation based on the guidance in
[“Writing R
Extensions”](https://cran.r-project.org/doc/manuals/r-release/R-exts.html#The-DESCRIPTION-file),
“\[The name\] should contain only (ASCII) letters, numbers and dot, have
at least two characters and start with a letter and not end in a dot”.

## Setup for `starters`

### Installation

    remotes::install_github("lockedata/starters")

### `start_here()` function

Run

``` r
starters::start_here()
```

This function checks different aspects of your setup (git installation,
gitconfig, `GITHUB_PAT`, `DESCRIPTION` default values, GitHub username
guessing), that will help automatic steps later on. Most of these
aspects are inspired from [`usethis` setup
article](https://usethis.r-lib.org/articles/articles/usethis-setup.html).
For each aspect, if your setup needs improvements an informative error
message will be thrown so you might be able to know how to proceed.

## RStudio gadget

If you want to set up a project without using the R functions,
[@jonmcalder](https://github.com/jonmcalder) made a nifty [RStudio
addin](https://rstudio.github.io/rstudioaddins/). Install the package to
get it added to your RStudio instance.

## Related work

Other R tools (not necessarily active, vet them first) useful for
starting new projects.

  - [`usethis`](https://usethis.r-lib.org/) in general,
    [`create_project()` and `create_package()` in
    particular](https://usethis.r-lib.org/reference/create_package.html).
    starters actually depends on usethis.

  - [`skeletor`](https://github.com/nealrichardson/skeletor), An R
    Package Skeleton Generator.

  - [`mkrpkg`](https://github.com/noamross/mkrpkg), Template for making
    R packages.

  - [`mason`](https://github.com/metacran/mason), A friendly craftsman
    that builds you great R packages.

## Contributing

### General info

Wanna report a bug or suggest a feature? Great stuff\! For more
information on how to contribute check out [our contributing
guide](.github/CONTRIBUTING.md).

Please note that this R package is released with a [Contributor Code of
Conduct](CODE_OF_CONDUCT.md). By participating in this package project
you agree to abide by its terms.

### Up for grabs

Make sure to check out the [Issues tab in
GitHub](https://github.com/lockedata/starters/issues)\! We’re making
this project a great place to start contributing to R packages. We will
help you through the process.
