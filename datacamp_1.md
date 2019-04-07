DataCamp\_Repo
================
Samuel Governor
April 4, 2019

``` r
library(tidyverse)
```

    ## -- Attaching packages ------------------------------------------------------- tidyverse 1.2.1 --

    ## v ggplot2 3.1.0       v purrr   0.3.2  
    ## v tibble  2.1.1       v dplyr   0.8.0.1
    ## v tidyr   0.8.3       v stringr 1.4.0  
    ## v readr   1.3.1       v forcats 0.4.0

    ## -- Conflicts ---------------------------------------------------------- tidyverse_conflicts() --
    ## x dplyr::filter() masks stats::filter()
    ## x dplyr::lag()    masks stats::lag()

``` r
 me<- c(1, 2, 3, 3,4)
 y<- c("today", "tommorow", "yesterday", "last_night", "today_morning")
 vik <- data.frame(y, me)
vik
```

    ##               y me
    ## 1         today  1
    ## 2      tommorow  2
    ## 3     yesterday  3
    ## 4    last_night  3
    ## 5 today_morning  4

``` r
subset (vik, subset= me < 3)
```

    ##          y me
    ## 1    today  1
    ## 2 tommorow  2

``` r
a <- c(100, 2000, 1, 3000)
order(a)
```

    ## [1] 3 1 2 4

``` r
a[order(a)]
```

    ## [1]    1  100 2000 3000
