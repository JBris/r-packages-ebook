5 The package within
================
James Bristow
11/22/23

## 5.4 Delta: a failed attempt at making a package

``` r
usethis::create_package("~/delta")
```

``` r
usethis::create_package("~/delta")
```

``` r
devtools::document()
devtools::install()
```

``` r
library(tidyverse)
library(delta)

infile <- "swim.csv"
dat <- read_csv(infile, col_types = cols(name = "c", where = "c", temp = "d"))

dat <- dat %>% 
  localize_beach() %>% 
  celsify_temp()

write_csv(dat, outfile_path(infile))
```

``` r
devtools::check()
```

## 5.5 Echo: a working package

``` r
usethis::create_package("~/echo")
```

``` r
devtools::install()
```

``` r
devtools::check()
```

``` r
library(tidyverse)
library(echo)

infile <- "swim.csv"
dat <- read_csv(infile, col_types = cols(name = "c", where = "c", temp = "d"))

dat <- dat %>% 
  localize_beach() %>% 
  celsify_temp()

write_csv(dat, outfile_path(infile))
```
