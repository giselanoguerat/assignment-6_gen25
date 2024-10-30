assignment-6
================
Gisela Noguera Toffoletti

# Assignment 6: Data import and tidy data

``` r
library(tidyverse)
library(knitr)
library(janitor)
library(ggplot2)
```

<br>

## Exercise 1. Tibble and Data Import

Import the data frames listed below into R and
[parse](https://r4ds.had.co.nz/data-import.html#parsing-a-vector) the
columns appropriately when needed. Watch out for the formatting oddities
of each dataset. Print the results directly, **without** using
`kable()`.

**You only need to finish any three out of the five questions in this
exercise in order to get credit.**

<br>

#### 1.1 Create the following tibble manually, first using `tribble()` and then using `tibble()`. Print both results. $$We didn’t have time to cover this in class, but look up how these functions work [here](https://r4ds.had.co.nz/tibbles.html#creating-tibbles)$$

``` r
tribble(
  ~a, ~b, ~c,
  1,2.1, "apple",
  2, 3.2, "orange"
)
```

    ## # A tibble: 2 × 3
    ##       a     b c     
    ##   <dbl> <dbl> <chr> 
    ## 1     1   2.1 apple 
    ## 2     2   3.2 orange

``` r
tibble(a = c(1,2),
       b = c(2.1,3.2),
       c = c("apple","orange"))
```

    ## # A tibble: 2 × 3
    ##       a     b c     
    ##   <dbl> <dbl> <chr> 
    ## 1     1   2.1 apple 
    ## 2     2   3.2 orange

<br>
