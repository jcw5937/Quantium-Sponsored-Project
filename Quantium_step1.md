Quantium Step 1
================

## Front Matter

``` r
library(dplyr)
```

    ## 
    ## Attaching package: 'dplyr'

    ## The following objects are masked from 'package:stats':
    ## 
    ##     filter, lag

    ## The following objects are masked from 'package:base':
    ## 
    ##     intersect, setdiff, setequal, union

## Loading the data

``` r
purchase_data <- read.csv("QVI_purchase_behaviour.csv")
transaction_data <- read.csv("QVI_transaction_data.xlsx")
```

    ## Warning in read.table(file = file, header = header, sep = sep, quote = quote, :
    ## line 1 appears to contain embedded nulls

    ## Warning in read.table(file = file, header = header, sep = sep, quote = quote, :
    ## line 3 appears to contain embedded nulls

    ## Warning in read.table(file = file, header = header, sep = sep, quote = quote, :
    ## line 4 appears to contain embedded nulls

    ## Warning in scan(file = file, what = what, sep = sep, quote = quote, dec = dec,
    ## : EOF within quoted string

    ## Warning in scan(file = file, what = what, sep = sep, quote = quote, dec = dec,
    ## : embedded nul(s) found in input

## Basic Data Exploration

``` r
head(purchase_data)
```

    ##   LYLTY_CARD_NBR              LIFESTAGE PREMIUM_CUSTOMER
    ## 1           1000  YOUNG SINGLES/COUPLES          Premium
    ## 2           1002  YOUNG SINGLES/COUPLES       Mainstream
    ## 3           1003         YOUNG FAMILIES           Budget
    ## 4           1004  OLDER SINGLES/COUPLES       Mainstream
    ## 5           1005 MIDAGE SINGLES/COUPLES       Mainstream
    ## 6           1007  YOUNG SINGLES/COUPLES           Budget
