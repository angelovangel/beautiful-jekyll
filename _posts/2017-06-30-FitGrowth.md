---
layout: post
title: FitGrowth app
tags:
  - R
  - Shiny
published: true
date: '2017-06-30'
---

FitGrowth is a Shiny app for (bacterial) growth curve analysis I wrote recently.
You can get it on [GitHub](https://github.com/angelovangel/FitGrowth), where you will find also example files for testing.
With FitGrowth you can:
  - Upload your own growth data
  - Visualize it and fit a model on it
  - Select interactively the time interval for fitting
  - Select number of facets of the plot and which samples to analyze 
  - Obtain the model parameters as a table
  - Analyse many samples
  - Download all plots and tables

### How it works
This app fits growth data to the continuous [logistic equation](https://en.wikipedia.org/wiki/Generalised_logistic_function). The best parameters `n0`, `k` and `r` are found using the nonlinear least-squares method `nls` in `R`. The app handles one or many samples (tested with 96), as well as `NA` values. You can get an example file [here](https://www.dropbox.com/sh/zzf7y3ijwkat55e/AABUvp7BAARIdYBqZWgk1E37a?dl=0). The easiest way to run FitGrowth is if you have [RStudio](http://rstudio.org), you just have to paste this in your console:
```r
shiny::runGitHub('FitGrowth', 'angelovangel')
```
You will need these packages, so install them if you haven't done so: `shiny`, `shinydashboard`, `modelr`, `tidyverse`, `broom` and `DT`.
### Instructions for use
Load the data as a text file, the first column *must* be named `time`, all other columns are treated as samples and the columns names are used as sample names. Adjust the file input settings until the data is read into the app. After that, take a look at the other tabs. 
Note that the parameters of the logistic model are re-calculated when the time interval is changed with the slider.

Cheers!
Angel
