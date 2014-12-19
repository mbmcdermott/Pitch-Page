---
title       : Crime by State,
subtitle    : and why you should care!
author      : Michael McDermott
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [bootstrap,quiz]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
--- bg:lightyellow

## Do you really know where you live?

- You may think that the state where you live is great.
- Perhaps it's beautiful, perhaps it has great food, but wouldn't you want to know what the crime rate was?
- If your state has really great ice cream but you have a high chance of getting it stolen, you might not want to live there.
- Well you're probably thinking you know what the crime rate is in your state.  You're probably thinking it's low compared to other states.  Well let's just see, you might be surprised!

--- &radio
## A question you might think you know the answer to

Which state had the highest murder rate per resident in 1973?

1. California
2. _Georgia_

*** .hint 
It might be the opposite of what you think.

*** .explanation 
You might have thought the answer was California.  We're always hearing about their broken prison system, but it turns out Georgia has a much higher murder arrest rate.


--- bg:url(assets/images/bg.png)

## What does the murder arrest rate look like?

- Here is a plot showing the various states and their murder arrest rates, there's alot of information on there!


```r
data(USArrests); par(mfrow=c(1,1),mar=c(15,5,2,1))
plot(factor(row.names(USArrests)),USArrests$Murder,xlab="State",ylab="Arrested Murders 
per 100,000 residents")
```

![plot of chunk unnamed-chunk-1](assets/fig/unnamed-chunk-1-1.png) 



--- bg:lightblue
## So want to compare States easily?


- There's a lot of information on that graph!
- Wouldn't it be nice to explore it interactively?


- Use the application to compare states interactively and much more easily!



- Simply pick as many states as you want to compare, and the application will tell you which has the highest and lowest crime rate! It will even tell you the average crime rate if you are comparing a group of states to another to move to!

 



