The Whole Game
================
James Bristow
11/22/23

## 1.1 Load devtools and friends

``` r
library(devtools)
packageVersion("devtools")
```

## 1.4 create_package()

``` r
create_package("/home/rstudio/regexcite")
```

## 1.7 use_r()

``` r
use_r("strsplit1")
```

## 1.8 load_all()

``` r
load_all()
```

``` r
(x <- "alfa,bravo,charlie,delta")
strsplit1(x, split = ",")
```

``` r
exists("strsplit1", where = globalenv(), inherits = FALSE)
```

## 1.9 check()

``` r
check() 
```

## 1.11 use_mit_license()

``` r
use_mit_license()
```

## 1.12 document()

``` r
document() 
```

``` r
?strsplit1 
```

``` r
check() 
```

## 1.14 install()

``` r
install() 
```

``` r
library(regexcite)

x <- "alfa,bravo,charlie,delta"
strsplit1(x, split = ",")
```

## 1.15 use_testthat()

``` r
use_testthat()
```

``` r
use_test("strsplit1")
```

``` r
test()
```

## use_package()

``` r
use_package("stringr")
```

``` r
use_package("stringr")
```

``` r
load_all()
str_split_one("a, b, c", pattern = ", ")
```

## 1.18 use_readme_rmd()

``` r
build_readme()
```

## 1.19 The end: check() and install()

``` r
check()
install()
```
