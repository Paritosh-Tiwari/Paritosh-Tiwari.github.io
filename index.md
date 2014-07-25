---
title       : The Idiot Box Trends
subtitle    : Explore TV Shows trends across time and categories- then choose your favorites
author      : Paritosh Tiwari
job         : 
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}
knit        : slidify::knit2slides
logo        : TV_Image_4.jpg
ext_widgets : {rCharts: libraries/nvd3}

---

## What's in it for me ?

<style>
strong {
  font-weight: bold;
}
em {
  font-style: italic;
}
</style>

You might find this app useful, if:

- You want to create the next big series in the history of television but are not sure which genre to step into. Fret not. Have a look at how different categories of TV Shows have fared with time and choose either the hottest one or the one with least competition.
- You are a social thinker, philosopher or just looking to gain an insight in the psyche of society. Explore the top genre's viewed by the public within each decade and ponder over the general state of society's mind.
<div style='text-align: left;'>
<img src="assets/img/image1.jpg">
</div>
- You just enjoy watching TV. You have seen all *(or most)* of the current best and want to know which shows were great before your time. Maybe you are just feeling nostalgic and want to remember the best television of the 80's/90's. Just select a category and a time period and have the list of top shows ready for you to enjoy. You can also directly go to the relevant TV show page by cliking on the hyperlink present in the results.

---

## So, How does it work ?

<style>
strong {
  font-weight: bold;
}
em {
  font-style: italic;
}
</style>

Check the App here: http://patiwari.shinyapps.io/TV_Shiny_App

You select whether to summarize by Category or Time Period. The chart below displays the trend for a sample category *(Action and Adventure)* across time. You can choose other categories in the actual application. *Hover the mouse over the graph to see the actual numbers.*
<iframe src=' assets/fig/nvd3plot.html ' scrolling='no' frameBorder='0' seamless class='rChart nvd3 ' id=iframe- myChart ></iframe> <style>iframe.rChart{ width: 100%; height: 400px;}</style>

---

## Trends can be summarized as per Time Periods also 

<style>
strong {
  font-weight: bold;
}
em {
  font-style: italic;
}
</style>

The chart below displays the top categories for a sample time period *(2001-2010)*. You can choose other time-periods in the actual application.

<iframe src=' assets/fig/nvd3plot_2.html ' scrolling='no' frameBorder='0' seamless class='rChart nvd3 ' id=iframe- myChart_2 ></iframe> <style>iframe.rChart{ width: 100%; height: 400px;}</style>

--- 
## **Forget trends !!! I just want to watch good TV**
<style>
strong {
  font-weight: bold;
}
em {
  font-style: italic;
}
</style>

Choose the **Both** option. Then choose a category and a time-period. You will get the list of Top 20 shows for the selected parameters. Do give some time for the image to load as it is sourced in real time from the show webpage.

#### **Appendix**
- *Data Source*: www.tv.com/shows/
- Code for scraping data from website and further cleanup can be found here: https://github.com/Paritosh-Tiwari/TV_Trends_App_Shiny/tree/master/Data%20Scraping%20and%20Cleanup
- Popular category was decided on the basis of calculated quantity 'Success Quotient'
- *Success Quotient* = (Votes for a show/Votes for all shows across same time period)*User Rating*100. Shows with success quotient in the top 80 percentile were considered Popular

#### **Disclaimers**
- The data is not exhaustive and is collected only from one source
- Any show with missing information was removed to have a clean data set
- Popularity is dependent on the voting and rating by users on the said website. It does not reflect on the actual commercial success of the show.





