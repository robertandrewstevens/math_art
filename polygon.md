polygon
================
Robert A. Stevens
2024-07-20

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
df <- data.frame(x = 0, y = 0)

n <- 500

for (i in 2:n) {
  df[i, 1] <- df[i - 1, 1] + ((0.98)^i) * cos(i)
  df[i, 2] <- df[i - 1, 2] + ((0.98)^i) * sin(i)
}

ggplot2::ggplot(df, aes(x, y)) +
  geom_polygon()+
  theme_void()
```

![](polygon_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Source:

Antonio S. Chinchón @aschinchon

<https://twitter.com/> \[2018-08-16\]