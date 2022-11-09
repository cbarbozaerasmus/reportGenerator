
<!-- README.md is generated from README.Rmd. Please edit that file -->

# reportGenerator

<!-- badges: start -->
<!-- badges: end -->

Automatic report generator of the Darwin EU studies.

## Installation

You can install the development version of reportGenerator like so:

``` r
install.packages("remotes")
remotes::install_github("cbarbozaerasmus/reportGenerator")
```

## Example

The function reportIncidencePrevalence takes a character string for
title and author. Then a tibble for incidence and prevalence from
IncidencePrevalence package.

``` r
library(reportGenerator)
library(IncidencePrevalence)

title <- "..."
author <- "..."
prevalence <- prevalence$prevalence_estimates
incidence <- incidence$incidence_estimates

## RUN

reportIncidencePrevalence(title,
                          author,
                          prevalence,
                          incidence)
```

It generates an HTML document in the reports folder.
