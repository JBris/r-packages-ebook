7 Data
================
James Bristow
11/22/23

## 7.1 Exported data

``` r
usethis::create_package("~/pkg")
```

``` r
my_pkg_data <- sample(1000)
usethis::use_data(my_pkg_data)
```

### 7.1.1 Preserve the origin story of package data

``` r
usethis::use_data_raw()

usethis::use_data_raw("my_pkg_data")
```

## 7.2 Internal data

``` r
internal_this <- 1
internal_that <-  2 
usethis::use_data(internal_this, internal_that, internal = TRUE)
```

``` r
usethis::use_data_raw("internal_this")
usethis::use_data_raw("internal_that")
```

## 7.3 Raw data file

``` r
usethis::use_data_raw("internal_this")
usethis::use_data_raw("internal_that")
```
