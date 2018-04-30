---
layout: post
published: false
title: google-location-heatmap
date: '2018-04-30'
---

### Interactive heatmap of your google location history 
[google-location-heatmap](https://github.com/angelovangel/google-location-heatmap) is my take on the problem of visualising your location history data from google.
I wrote this Shiny app a while ago, and now I polished it a bit to put it on GitHub. It takes your google location history, which you can download from your [google account](https://takeout.google.com/settings/takeout), and plots it as a heat trace on a map. You can interactively change some of the settings (map opacity, radius and blur of the heatmap) and select the time range you want to see.

![This is me going around Europe:)](img/screenshot1.png)


### How to use
- First, go to [google takeout](https://takeout.google.com/settings/takeout), select "Location history" (and de-select all the rest), download and unzip the file. What you are going to need is the `LocationHistory.json` file. 
- In [RStudio](https://www.rstudio.com/), run

`runGitHub("google-location-heatmap", "angelovangel")`

If you don't have `shiny` installed, do it with `install.packages("shiny")` before doing the above. The app should open in a browser window on your computer. Note that the processing of your `json` file may take a while, depending on its size and the power of your machine.
- Of course, you can also manually download this repository, open the `app.R` file and press `Run App` in RStudio.

Cheers!   
Angel
