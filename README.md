# slidify

---
title: "GDP Visualization USA"
author: "Aaron nejad"
date: "Sunday, July 26, 2015"
output: slidy_presentation
---


## Slide 2 Purpose of the Shiny Project 

1. Difficult to make economic analysis on just numbers and even charts
2. Need a method to visualize the data in a more simple fashion
3. Need to be able to split the data into different subcomponents



--- .class #id 

## Slide 3 Visualizing using Maps

1. Maps allow us to create a more efficient image of statistics
2. By using heat maps or color plates we are able to use vast amount of data and make quick and true assesments on facts.
3. Using maps and color visualizations allow readers to memorize the data much better.

--- .class #id 

## Slide 4  Splitting GDP into its Different Components

Here is an example of economic data to download from R

```{r}
library(WDI)
dat = WDI(indicator='NY.GDP.PCAP.KD', country=c('US'), start=1960, end=2012)
head(dat)

```

1. We should be able to split our GDP data into various subcategories.
2. Subcategories include GDP Including Investments , GNP (Gross National Product) etc.
3. By keeping the percentage slider constant and changing the tabs into different categories, we can see consistency of subcategories.

--- .class #id 

##  Slide 5  Further Research
1. In future projects we can add more complex data like column bars on the charts to add more statistics. 
2. Future projects should allow us to change data from % quantile for county to absolute average value for county. 
