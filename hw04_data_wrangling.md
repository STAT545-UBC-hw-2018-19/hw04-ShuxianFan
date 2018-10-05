Homework 04: Tidy data and joins
================
**Shuxian Fan**
Oct 4th, 2018

Initial Package Set-up
----------------------

``` r
suppressPackageStartupMessages(library(gapminder))
suppressPackageStartupMessages(library(tidyverse))
suppressPackageStartupMessages(library(geonames))
suppressPackageStartupMessages(library(devtools))
suppressPackageStartupMessages(library(rjson))
require(devtools)
install_github("ropensci/geonames")
```

    ## Skipping install of 'geonames' from a github remote, the SHA1 (e90cd742) has not changed since last install.
    ##   Use `force = TRUE` to force installation

Data Reshaping Prompts
----------------------

Join Prompts - **Activity \#1**
-------------------------------

*(1) Create a second data frame, complementary to Gapminder.*

*(2) Join this with (part of) Gapminder using a `dplyr` join function and make some observations about the process and result. Explore the different types of joins.*

In terms of incorporating more informations of the country, I will be using the data from the package `geonames`. In order to get access to the geonames database, I refered to this [GitHub Repository](https://github.com/ropensci/geonames) providing an R package for accessing the geonames.org API.

One row per country, a country variable and one or more variables with extra info, such as language spoken, NATO membership, national animal, or capitol city. One row per continent, a continent variable and one or more variables with extra info, such as northern versus southern hemisphere.

Reference and Source
--------------------

1.  R package for accessing the geonames.org API

<https://github.com/ropensci/geonames>
