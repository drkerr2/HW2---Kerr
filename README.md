---
title: "HW2"
author: "drkerr2"
date: "9/7/2020"
output: html_document
---
```{r}
###setting up HW2####
#HW2(2) 2x +5y = 33 
#       x + 3y = 19
#       matrix a is:
#       2 5
#       1 3
#       matrix b is:
#       33
#       19
```


```{r}
a <- matrix(c(2,1,5,3), nrow = 2, ncol = 2)
a
> a
     [,1] [,2]
[1,]    2    5
[2,]    1    3
```


```{r}
b <- matrix(c(8,2), nrow = 2, ncol = 1)
b
> b
     [,1]
[1,]    8
[2,]    2
```


```{r}
solve(a,b)

> solve(a,b)
     [,1]
[1,]   14
[2,]   -4
```


```{r}
dyl <- c(1:100)
sum(dyl)/100
[1] 50.5
```


```{r}
> install.packages("dplyr")
WARNING: Rtools is required to build R packages but is not currently installed. Please download and install the appropriate version of Rtools before proceeding:

https://cran.rstudio.com/bin/windows/Rtools/
Installing package into ‘C:/Users/dkerr/Documents/R/win-library/4.0’
(as ‘lib’ is unspecified)
trying URL 'https://cran.rstudio.com/bin/windows/contrib/4.0/dplyr_1.0.2.zip'
Content type 'application/zip' length 1308048 bytes (1.2 MB)
downloaded 1.2 MB

package ‘dplyr’ successfully unpacked and MD5 sums checked

The downloaded binary packages are in
	C:\Users\dkerr\AppData\Local\Temp\RtmpGW63Mv\downloaded_packages
> library(dplyr)

Attaching package: ‘dplyr’

The following objects are masked from ‘package:stats’:

    filter, lag

The following objects are masked from ‘package:base’:

    intersect, setdiff, setequal, union

HW2.df <- data.frame(row1 = c("A","D"), row2 = c("B","E"), row3 = c("C", "F"), row4 = c("D", "G"))
print(HW2.df)
```
 
```{r setup, include=FALSE}
knitr::opts_chunk$set(echo = TRUE)
```

## R Markdown

This is an R Markdown document. Markdown is a simple formatting syntax for authoring HTML, PDF, and MS Word documents. For more details on using R Markdown see <http://rmarkdown.rstudio.com>.

When you click the **Knit** button a document will be generated that includes both content as well as the output of any embedded R code chunks within the document. You can embed an R code chunk like this:

```{r cars}
summary(cars)
```

## Including Plots

You can also embed plots, for example:

```{r pressure, echo=FALSE}
plot(pressure)
```

Note that the `echo = FALSE` parameter was added to the code chunk to prevent printing of the R code that generated the plot.
