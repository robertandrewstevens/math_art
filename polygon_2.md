polygon 2
================
Robert A. Stevens
2024-07-23

Got a better name?

``` r
# import libraries
library(ggplot2)
```

``` r
d <- data.frame(x = 1, y = 1)

n <- 120

for (i in 2:n) {
  d[i, "x"] <- d[i - 1, 1] - sin((i %% 4) * 3 * pi / 2 - ceiling(i / 4) * pi / 40) * 0.99^i
  d[i, "y"] <- d[i - 1, 2] + cos((i %% 4) * 3 * pi / 2 - ceiling(i / 4) * pi / 40) * 0.99^i
}

ggplot(d, aes(x, y)) +
  geom_polygon() +
  coord_fixed() +
  theme_void()
```

![](polygon_2_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Source:

Antonio S. Chinchón @aschinchon

<https://twitter.com/> \[2018-08-17\]
