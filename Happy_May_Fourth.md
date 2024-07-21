Happy May Fourth
================
Robert A. Stevens
2024-07-20

``` r
# import libraries
library(rafalib)
```

``` r
par(bg=1, fg="white")
x <- 0.5 -> y
z <- "|-o-|"
s <- cbind(runif(50), runif(50))
m < -c(-1,1)/20
```

    Error in eval(expr, envir, enclos): object 'm' not found

``` r
while(TRUE) {
  rafalib::nullplot(xaxt="n", yaxt="n", bty="n")
  points(s, pch=".")
  text(x, y, z, cex=4)
  x <- pmin(pmax(x + sample(m, 1), 0), 1)
  y <- pmin(pmax(y + sample(m, 1), 0), 1)
}
```

    Error in eval(expr, envir, enclos): object 'm' not found

![](Happy_May_Fourth_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Source:

Rafael Irizarry @rafalab

<https://twitter.com/home> \[2022-05-04\]

Happy `#MayFourth #rstats`
