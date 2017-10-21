---
layout: post
published: true
title: TRACEview
subtitle: A Shiny app for visualizing HPLC (or other chromatographic) traces
date: '2017-10-19'
---
# TRACEview
### A Shiny app for visualizing HPLC (or other chromatographic) traces. 
This app reads in chromatogram files from any chromatography system (exported as csv or similar) and plots the traces, allowing also shifting of the traces in the y-axis. Zooming, panning and saving the traces as images are also supported (thanks to [rbokeh](http://hafen.github.io/rbokeh/)).
I have tested with chromatograms from Chromeleon (some example files can also be found here as a zip), but any file with time-signal columns should work.

![A view of the chromatographic traces in the app]({{site.baseurl}}/img/trace1.png)

If you have many samples, a nice comparative overview gives the "simulated TLC":

![trace2.png]({{site.baseurl}}/img/trace2.png)




### Usage  
the easiest way is to run this in RStudio  
`shiny::runGitHub("TRACEview", "angelovangel")`  
or alternatively, download the app.R file from [here](https://github.com/angelovangel/TRACEview), open it in RStudio and press the "Run App" button.  

### Prerequisites
The libraries required (have to be installed in `R` first) are:  
`ggplot2` `dplyr` `purrr` `readr` `stringr` `rbokeh` `shiny` and `shinydashboard`

Have fun!  
Angel
