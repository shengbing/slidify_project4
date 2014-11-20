---
title       : Data product project presentation
subtitle    : shiny and slidify
author      : Shengbing Huang
job         : Data science specialization
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [quiz, bootstrap, shiny, interactive]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
ext_widgets: {rCharts: [libraries/nvd3]}


--- .class #id 

## Motivation and functionality of the T-distribution apps

1. T distribution approximates normal distribution when degree of freedom increases
2. This app can visulize change of t-distribution given degree of freedom. 
3. Given a t-statistics and degree of freedom, p-value can be computed and shown on the t-distribution

---

## A normal distribution plot ##


```r
x <- seq(-10, 10, length=100)
hx <- dnorm(x)
plot(x, hx, type="l", lty=2, xlab="x value",
                     ylab="Density", main="normal distribution")
```

<img src="assets/fig/simple-plot.png" title="plot of chunk simple-plot" alt="plot of chunk simple-plot" style="display: block; margin: auto;" />

```r
lines(x, dt(x, 1),lwd=2, col=colors[1])
```

```
## Error: object of type 'closure' is not subsettable
```

![plot of chunk simple-plot](figure/simple-plot.png)

---



<iframe src="https://huangshengb.shinyapps.io/project_shiny/"></iframe>

--- &radio

## Quiz

Which one of these slidify slides do you like the most?

1. I don't like any of these slides 
2. The normal distribution plot
3. T distribution
4. _I can not tell. All is interesting._

*** .hint
This is a hint

*** .explanation
This is an explanation


