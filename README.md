
<!-- README.md is generated from README.Rmd. Please edit that file -->

# pathroutr

<!-- badges: start -->

[![Lifecycle:
experimental](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)
[![R build
status](https://github.com/jmlondon/pathroutr/workflows/R-CMD-check/badge.svg)](https://github.com/jmlondon/pathroutr/actions)
<!-- badges: end -->

The goal of `{pathroutr}` is to provide functions for re-routing paths
that cross land around barrier polygons. The use case in mind is
movement paths derived from location estimates of marine animals. Due to
error associated with these locations it is not uncommon for these
tracks to cross land. The `{pathroutr}` package aims to provide a
pragmatic and fast solution for re-routing these paths around land and
along an efficient path. It is important to note any re-routed paths are
not statistical models and may have unintended consequences and biases
associated with them that depends on the study animal, study area, and
error nature of the original data. Re-routed paths may also exceed the
speed or physiological capabilities of the study species.

## Credit Where Credit is Due

We believe this is the first implementation of visibility graphs within
R for spatial routing. However, three sources were of key importance to
developing the approach

1.  Seaway distances with PostgreSQL by Angus Cameron (24 Apr, 2016)
2.  Pyvisgraph Python package by Christian Reksten-Monsen
3.  Jan, Gene Eu, et al. “An $ $ Shortest Path Algorithm Based on
    Delaunay Triangulation.” IEEE/ASME Transactions On Mechatronics 19.2
    (2013): 660-666. DOI: 10.1109/TMECH.2013.2252076

In addition, both the `{sf}` and `{stplanr}` R packages are of key
importance to the functionality within `{pathroutr}`

1.  Lovelace, R. and Ellison, R., 2017. stplanr: A Package for Transport
    Planning. The R Journal. <https://doi.org/10.32614/RJ-2018-053>
2.  Pebesma, E., 2018. Simple Features for R: Standardized Support for
    Spatial Vector Data. The R Journal 10 (1), 439-446,
    <https://doi.org/10.32614/RJ-2018-009>

## Installation

\`{pathroutr}’ is currently not available on CRAN

The development version is available from
[GitHub](https://github.com/jmlondon/pathroutr) with:

``` r
# install.packages("remotes")
remotes::install_github("jmlondon/pathroutr")
```
