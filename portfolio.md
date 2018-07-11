---
title: "Shiny apps"
subtitle: "from Angel Angelov"
published: true
---


***

This is just a collection of links to Shiny apps I have written. Most apps are running on a `R` server on the [Amazon cloud](https://aws.amazon.com/), so all you need to use them is a decent web browser. The programs listed here are (hopefully) useful helpers in the daily work in a biology lab, but there are also apps from completely different fields (like visualization of your Google location or of the [openflights](https://openflights.org/) data). Of course, all is open source and the code can be found on [GitHub](https://github.com/angelovangel).

***

#### [FitGrowth](http://35.176.52.165/shiny/rstudio/FitGrowth/v02-drc/)

Upload a text file with growth data (optical density, CFU, etc. *vs* time) and obtain the parameters of a logistic regression model.
(Old version available [here](http://35.176.52.165/shiny/rstudio/FitGrowth/v01/)).

***

#### [TRACEview](http://35.176.52.165/shiny/rstudio/TRACEview/) 

Visualize a set of HPLC trace files (must be first exported to text files). For many samples, the traces can be stacked and a virtual thin layer chromatography (TLC) plate can be simulated.

***

#### [facsR](http://35.176.52.165/shiny/rstudio/facsR/)

Fast plotting of FACS data. You will need the FCS files exported from your machine. The total amount of data you can upload is currently limited to 100 Mb.

***

#### [Heatmap of (your) Google location data](https://github.com/angelovangel/google-location-heatmap)

Make a customizable and interactive heatmap of your location data from Google. First go to [Google takeout](https://takeout.google.com/settings/takeout) to download your Google location history. This app is not running on Amazon, because it generates too much traffic and would cost me too much. If you want to try it you'll have to follow the instructions in the link above. 

***

#### [Interactive map of the openflights data (airports, airlines, routes)](http://35.176.52.165/shiny/rstudio/openflights/)

The name says it all.

#### [aRt]()

Nothing useful here, just nice to look at. [Here are links to youtube videos](https://youtu.be/c0gjVgNmK1o) of some gif animations I made of aircraft flight paths, recorded by the [Automatic Dependent Surveillance-Broadcast (ADS-B) and Mode S systems](https://en.wikipedia.org/wiki/Automatic_dependent_surveillance_%E2%80%93_broadcast) (data obtained from the [opensky network](https://opensky-network.org/)).


***






