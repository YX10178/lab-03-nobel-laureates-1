Lab 03 - Nobel laureates
================
Yuxin Xie
1/29/2025

### Load packages and data

``` r
library(tidyverse) 
```

``` r
nobel <- read_csv("data/nobel.csv")
```

## Exercises

### Exercise 1

``` r
dim(nobel)
```

    ## [1] 935  26

``` r
cat("Number of observations:", nrow(nobel), "\n")
```

    ## Number of observations: 935

``` r
cat("Number of variables:", ncol(nobel), "\n")
```

    ## Number of variables: 26

``` r
##there are 935 observations of 26 variables in the dataset.
##each row represents a Nobel Prize laureate 
```

### Exercise 2

``` r
nobel_living <- nobel %>%
  filter(!is.na(country) & gender != "org" & is.na(died_date))
cat("Number of observations in nobel_living:", nrow(nobel_living))
```

    ## Number of observations in nobel_living: 228

### Exercise 3

Remove this text, and add your answer for Exercise 1 here. Add code
chunks as needed. Don’t forget to label your code chunk. Do not use
spaces in code chunk labels.

### Exercise 4

…

### Exercise 5

…

### Exercise 6

…
