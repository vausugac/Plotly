Data Product
========================================================
author: Victor Usuga
date: 6/11/2020
autosize: true

Following instructions have been given for the assignment
========================================================


1. Create a web page presentation using R Markdown that features a plot created with Plotly.  
2. Host your webpage on either RPubs, GitHub Pages, or NeoCities.   
3. Your webpage must contain the date that you created the document, and it must contain a plot created with Plotly.

The Interactive Plot presented in this Assignment are as follows
========================================================

 A Time-Series chart of the Population of the United States (in millions) for the period 1790-1970.

Slide With Code
========================================================



library(datasets)

library(plotly)

data(uspop)

 Load the data set that gives the population of the United States in millions for the period 1790-1970

Plotly Command

plot_ly(x=~time(uspop),y=~uspop,type="scatter",mode="lines") %>% layout(title = "U.S. Population in millions for the period 1790-1970", xaxis = list(title = "Year"),yaxis = list(title = "U.S. Population (millions)"))

```


Slide With Plot
========================================================

![plot of chunk unnamed-chunk-1](Data Product-figure/unnamed-chunk-1-1.png)
