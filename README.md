## Web-Design-Challenge
# Weather Data Revisited through the Power of HTML, CSS and Bootstrap

## Overview

In order to put newly acquired HTML, CSS and Bootstrap skills to good use, a website was created taking advantage of weather data and scatter plots created in a previous challenge. This website needed a landing page, 4 visualization pages, a data page to show the underlying data, and a comparison page so all 4 scatter plots could be viewed at once. Navigation was also included by way of a top navigation bar with links and a dropdown list and a sidebar of visualization thumbnails. All of this needed to work on various size screens from a smartphone up to a desktop monitor. 


### Files and Folders

* [Landing Page](index.html) - this *index.html* file is the landing page for the website 
* **Jupyter Notebook** (city_weather_date.jpynb) - the Jupyter Notebook file that contains the script to convert the weather data output from a CSV file to an HTML file
* [Data](WebVisualizations/data.html) - this is the HTML file created from the Jupyter Notebook and is used for the *Data* page
* [Comparisons](WebVisualizations/comparison.html) - this file is used for the Comparisons page and contains all 4 visualizations
* [WebVisualizations](WebVisualizations/) - this folder contains all the files used in the project except for the index.html file
    * [Resources](WebVisualizations/Resources/) - this folder contains the date source file (*City_Data.csv*)
    * [Assets](WebVisualizations/assets/) - this folder contains the *CSS* and *images* subfolders and files
        * [CSS](WebVisualizations/assets/css/) - this folder contains the *styles.css* file used to format most of the website
        * [Images](WebVisualizations/assets/images/) - this folder contains the 4 scatter plot image files
    * [Visualizations](WebVisualizations/visualizations/) - this folder contains the 4 HTML visualiation files


## Web Development

In order to create this website, I started with the main page, or landing page,



## Notes

I used weather data for this project but I decided to use the data I had gathered from the earlier project instead of using the files provided. I had already done the analysis on the dataset I had created so it just made more sense to use that again. I had also put a lot of work into creating those files originally so to get the oppunity to put that to good use was appealing.

In the *Plots* dropdown, I disabled the plot if it was the current page being viewed. Seemed like you shouldn't have a link to choose it if you're already on that page.

The navigation bar was quite the challenge. Learned a lot about those various attributes, though, so it was more satisying when I actually got everything to work. The different screen sizes and the navbar background color change dependency what one of the more challenging part of it.

The sidebar with the thumbnails gave me a run for my money. But the bootstrap column grid settings finally started to make more sense along the way.

I had such grand ideas for this website but time was not my friend so I didn't get a chance to build it out more. Between the navigation bar and the sidebar, where a good portion of my time was spent, it's amazing my hair hasn't all turned gray!

