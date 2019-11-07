Markdown Example
================
Erik Eiler
2019-10-17

  - [Introduction](#introduction)
  - [HTML Content](#html-content)
  - [Embed Code](#embed-code)
      - [Set Directory](#set-directory)
      - [Load data](#load-data)
          - [Plot Data](#plot-data)
          - [Plot with format options](#plot-with-format-options)

-----

# Introduction

This is an *R Markdown document*. Markdown is a simple formatting syntax
for authoring HTML, PDF, and MS Word documents. For more details on
using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that
includes both content as well as the output of any embedded R code
chunks within the document.

# HTML Content

<p>

This is a new paragraph written with the HTML tag

<table border=1>

<th>

Pros

</th>

<th>

Cons

</td>

<tr>

<td>

Easy to use

</td>

<td>

Need to Plan ahead

</td>

<tr>

</table>

<hr/>

# Embed Code

## Set Directory

You can embed any R code chunk within 3 ticks. If you add echo=FALSE the
code chunk is not displayed in the document. We can set knitr options
either globally or within a code segment. The options set globally are
used throughout the document.

We set the root.dir before loading any files. By enabling cache=TRUE, a
code chunk is executed only when there is a change from the prior
execution. This enhances knitr performance.

## Load data

<test_link>

### Plot Data

``` r
plot(auto$mpg~auto$weight)
```

![](knitr_files/figure-gfm/plotData-1.png)<!-- -->

### Plot with format options

![](knitr_files/figure-gfm/plotFormatData-1.png)<!-- -->

    ## 'data.frame':    398 obs. of  9 variables:
    ##  $ No          : int  1 2 3 4 5 6 7 8 9 10 ...
    ##  $ mpg         : num  28 19 36 28 21 23 15.5 32.9 16 13 ...
    ##  $ cylinders   : int  4 3 4 4 6 4 8 4 6 8 ...
    ##  $ displacement: num  140 70 107 97 199 115 304 119 250 318 ...
    ##  $ horsepower  : int  90 97 75 92 90 95 120 100 105 150 ...
    ##  $ weight      : int  2264 2330 2205 2288 2648 2694 3962 2615 3897 3755 ...
    ##  $ acceleration: num  15.5 13.5 14.5 17 15 15 13.9 14.8 18.5 14 ...
    ##  $ model_year  : int  71 72 82 72 70 75 76 81 75 76 ...
    ##  $ car_name    : Factor w/ 305 levels "amc ambassador brougham",..: 66 184 165 86 8 18 11 79 42 112 ...

There are 398 cars in the auto data set.
