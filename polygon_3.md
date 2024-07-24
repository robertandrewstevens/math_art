polygon 3
================
Robert A. Stevens
2024-07-23

Got a better name?

``` r
# import libraries
library(ggplot2)
```

``` r
df <- data.frame(x = 1, y = 1)

n <- 180

for(i in 2:n) {
  df[i, 1] <- df[i - 1, 1] - sin((i %% 4) * 3 * pi / 2 - ceiling((i - 1) / 4) * pi / 90) * 0.977^i
  df[i, 2] <- df[i - 1, 2] + cos((i %% 4) * 3 * pi / 2 - ceiling((i - 1) / 4) * pi / 90) * 0.977^i
}

ggplot(df, aes(x, y)) +
  geom_polygon()+
  coord_fixed()+
  theme_void()
```

![](polygon_3_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Source:

Antonio S. Chinchón @aschinchon

<https://twitter.com/> \[2018-08-19\]
