# Saptial Temporal Analysis of Bushfire - Metrological Data

![alt text]( bushfire.gif "Logo Title Text 1")

## Introduction:
_______
2020 has been highly unpredictable interms the even that has been happening recently. One such unfortunate event was the bushfire that happened around the world this year. Especially the one that has happened in Australia which almost enveloped most part of Australia leaving a lot of damage behind interms of livelyhood, vegetation loss and lives lost. Though there were a lot of firefighter that were tasked at bringing the fire under controls they could at best mitigate the damages of the fires than to completely stop it which was due to the vastness of the problem. The fire in Australia was majorly caused due climatic changes and in general the earth becoming hotter. We can say that there would be more such bushfire to be expected around the world and in Austrlia.

What this project aims at achieving is to effectively predict bushfire in the future in terms of its __location (Spatial)__ also __time (temporal)__ and the area of affect. This project is based on another research paper which was conducted for the Eurpean bushfires

## Technicalites:
------
### R 4.0.0

### Libraries:
    * grid
    * lattice
    * gridExtra
    * GGaly
    * tidyverse
    * psych
    * reshape
    * corrplot
    * caret
    * ranger
    * e1071
### Pre-settings
The options was get to -1 so as to not show the warning that can come due to discrepancy between libraries or warnings generated due to depreceation of some functions in libraries that we might not be using this is completely _optional_.
```r
options(warn=-1)
set.seed(137) #137 is the golden quantum number (a lil nerd)
```


## Preliminary :
-----------
### This project tasks us with the responsiblity of completeing an Exploratory Data Analysis and consequently building a Model from the selected features to accurately predict the area of the forest fires using some predictors variables like (FFMC, ISI, rain, DMC, DC, temp, wind, month, day)
There for what we are trying to do is create a model that minizes the rss or maximizes r2 values for model where:
* X dependent = FFMC, ISI, rain, DMC, DC, RH, temp, wind, month, day
* Y indipendent = Area (continous variable)
