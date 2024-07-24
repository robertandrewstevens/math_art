waffle
================
Robert A. Stevens
2024-07-23

Got a better name?

``` r
# import libraries
library(tidyverse)
```

    ── Attaching core tidyverse packages ──────────────────────── tidyverse 2.0.0 ──
    ✔ dplyr     1.1.4     ✔ readr     2.1.5
    ✔ forcats   1.0.0     ✔ stringr   1.5.1
    ✔ ggplot2   3.5.1     ✔ tibble    3.2.1
    ✔ lubridate 1.9.3     ✔ tidyr     1.3.1
    ✔ purrr     1.0.2     
    ── Conflicts ────────────────────────────────────────── tidyverse_conflicts() ──
    ✖ dplyr::filter() masks stats::filter()
    ✖ dplyr::lag()    masks stats::lag()
    ℹ Use the conflicted package (<http://conflicted.r-lib.org/>) to force all conflicts to become errors

``` r
seq(-10, 10, by=0.05) %>%
  expand.grid(x=., y=.) %>%
  ggplot(aes(x=(x + sin(y)), y=(y + cos(x)))) +
    geom_point(alpha=0.1, shape=20, size=0, color="white") +
    theme_void() +
    coord_fixed() +
    theme(panel.background=element_rect(fill="violetred4"))
```

![](waffle_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Source:

Antonio S. Chinchón @aschinchon

<https://twitter.com/> \[2018-08-21\]
