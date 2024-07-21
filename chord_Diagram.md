chord Diagram
================
Robert A. Stevens
2024-07-20

``` r
# import libraries
library(circlize)
```

    ========================================
    circlize version 0.4.16
    CRAN page: https://cran.r-project.org/package=circlize
    Github page: https://github.com/jokergoo/circlize
    Documentation: https://jokergoo.github.io/circlize_book/book/

    If you use it in published research, please cite:
    Gu, Z. circlize implements and enhances circular visualization
      in R. Bioinformatics 2014.

    This message can be suppressed by:
      suppressPackageStartupMessages(library(circlize))
    ========================================

``` r
par(mar=c(1, 1, 1, 1), bg="violetred4")

circlize::chordDiagram(
  matrix(1, 20, 20), 
  col="white", 
  symmetric=TRUE, 
  transparency=0.85, 
  annotationTrack = NULL
)
```

![](chord_Diagram_files/figure-gfm/unnamed-chunk-3-1.png)<!-- -->

Source:

Antonio S. Chinchón @aschinchon

<https://twitter.com/> \[2017-11-22\]
