
<!-- README.md is generated from README.Rmd. Please edit that file -->
shed
====

[![lifecycle](https://img.shields.io/badge/lifecycle-experimental-orange.svg)](https://www.tidyverse.org/lifecycle/#experimental)

![shed](inst/img/shed.png)

A minimal, eye-friendly csv editor made with shiny, rhandsontable and readr. Shed is designed to quickly edit small (hundreds of rows) csv files and `data.frames`. It uses `readr::write_excel_csv()` as backend for writing files, and thus produces UTF-8 encoded csv files that are compatbile with MS Excel by default.

Help Wanted
-----------

Shed is still in an early stage of development. If you think shed could be useful to you you can contribute in the following way:

-   File feature requests and bug reports in the issue tracker
-   Make a more modern looking, light css theme for shed (see `inst/css/shed_dark.css`)

Installation
------------

You can install shed from github with:

``` r
# install.packages("devtools")
devtools::install_github("s-fleck/shed")
```

Example
-------

``` r
shed(iris)

# Uppon termination, shed returns the edited data.frame

x <- shed(iris)
```
