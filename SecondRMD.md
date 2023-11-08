SecondRMD
================
Jethro Banda
2023-11-08

``` r
plot(pressure)
head(pressure)
```

    ##   temperature pressure
    ## 1           0   0.0002
    ## 2          20   0.0012
    ## 3          40   0.0060
    ## 4          60   0.0300
    ## 5          80   0.0900
    ## 6         100   0.2700

``` r
library(tidyverse)
```

    ## ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ## ✔ dplyr     1.1.3     ✔ readr     2.1.4
    ## ✔ forcats   1.0.0     ✔ stringr   1.5.0
    ## ✔ ggplot2   3.4.4     ✔ tibble    3.2.1
    ## ✔ lubridate 1.9.3     ✔ tidyr     1.3.0
    ## ✔ purrr     1.0.2     
    ## ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ## ✖ dplyr::filter() masks stats::filter()
    ## ✖ dplyr::lag()    masks stats::lag()
    ## ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors

``` r
pressure %>% 
  mutate(temperature  = temperature + 2)
```

    ##    temperature pressure
    ## 1            2   0.0002
    ## 2           22   0.0012
    ## 3           42   0.0060
    ## 4           62   0.0300
    ## 5           82   0.0900
    ## 6          102   0.2700
    ## 7          122   0.7500
    ## 8          142   1.8500
    ## 9          162   4.2000
    ## 10         182   8.8000
    ## 11         202  17.3000
    ## 12         222  32.1000
    ## 13         242  57.0000
    ## 14         262  96.0000
    ## 15         282 157.0000
    ## 16         302 247.0000
    ## 17         322 376.0000
    ## 18         342 558.0000
    ## 19         362 806.0000

``` r
plot(pressure)
```

![](SecondRMD_files/figure-gfm/unnamed-chunk-1-1.png)<!-- -->
