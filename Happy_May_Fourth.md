Happy May Fourth
================
Robert A. Stevens
2024-07-21

``` r
# import libraries
library(rafalib)
```

``` r
par(bg=1, fg="white")

n <- 50  # originally 50

x <- 0.5
y <- 0.5
z <- "|-o-|"
s <- cbind(runif(n), runif(n))
m <- c(-1, 1) / 20

# while(TRUE) {
for(i in 1:10) {
  rafalib::nullplot(xaxt="n", yaxt="n", bty="n")
  points(s, pch=".")
  text(x, y, z, cex=4)
  x <- pmin(pmax(x + sample(m, 1), 0), 1)
  y <- pmin(pmax(y + sample(m, 1), 0), 1)
}
```

![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-2.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-3.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-4.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-5.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-6.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-7.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-8.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-9.png)<!-- -->![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-10.png)<!-- -->

Source:

Rafael Irizarry @rafalab

<https://twitter.com/home> \[2022-05-04\]

Happy `#MayFourth #rstats`
