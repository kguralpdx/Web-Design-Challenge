## Web-Design-Challenge
# Weather Data Revisited through the Power of HTML, CSS and Bootstrap

## Overview

In order to put newly acquired HTML, CSS and Bootstrap skills to good use, a website was created taking advantage of weather data and scatter plots created in a previous challenge. This website needed a landing page, 4 visualization pages, a data page to show the underlying data, and a comparison page so all 4 scatter plots could be viewed at once. Navigation was also included by way of a top navigation bar with links and a dropdown list and a sidebar of visualization thumbnails. All of this needed to work on various size screens from a smartphone up to a desktop monitor. 


### Files and Folders

* [Landing Page](index.html) - this *index.html* file is the landing page for the website 
* **Jupyter Notebook** (city_weather_date.jpynb) - the Jupyter Notebook file that contains the script to convert the weather data output from a CSV file to HTML
* [Data](WebVisualizations/data.html) - this is the HTML file created from the Jupyter Notebook HTML and is used for the *Data* page
* [Comparisons](WebVisualizations/comparison.html) - this file is used for the Comparisons page and contains all 4 visualizations
* [WebVisualizations](WebVisualizations/) - this folder contains all the files used in the project except for the index.html file
    * [Resources](WebVisualizations/Resources/) - this folder contains the date source file (*City_Data.csv*)
    * [Assets](WebVisualizations/assets/) - this folder contains the *CSS* and *images* subfolders and files
        * [CSS](WebVisualizations/assets/css/) - this folder contains the *styles.css* file used to format most of the website
        * [Images](WebVisualizations/assets/images/) - this folder contains the 4 scatter plot image files
    * [Visualizations](WebVisualizations/visualizations/) - this folder contains the 4 HTML visualization files


## Web Development

In order to create this website, I started with the home page, or landing page. Just added the image and text. Started looking into navigation and sidebar but that was becoming time consuming so moved on.

Next I created the *Data* page. I knew that was going to require something outside the HTML/CSS whelm so wanted to get that taken care of. I used *Pandas* to generate an HTML table from a dataframe. That worked pretty well. I then created the page with some help from the [Layoutit!](https://layoutit.com/build) website to get the table structure. It took a little bit of tweaking but was pretty helpful.

After the *Data* page was created, I did the *Comparisons* page. Once again, I turned to the [Layoutit!](https://layoutit.com/build) website for structure assistance for the grid.

The *Visualization* pages came next and were pretty straightforward. 

Now I had all the pages created, time to tackle navigation and the sidebar. I decided to go with navigation first. This posed several challenges for me. Trying to get the layout correct and then the background colors to work depending on the screen size. Used media queries to help with the background color change. Ran into an issue when using the `navbar-light` with `bg-light`class attributes of the `nav` element. When the navigation bar background color was supposed to switch because the screen size got smaller, the *hamburger* icon would disappear. I tried setting the background color in the *styles.css* file using a media query and just trying to set it directly, but neither would work. Finally found that removing the `bg-light` attribute was all that was needed. Used the `navbar-brand` class of the `nav` element since that was always in the left side of the navigation bar and I could make it a link. Once I got the navigation bar working correctly, I added the code for that to each of the HTML pages.

The sidebar was the last challenge to overcome. Had issues getting it positioned correctly. Then I had trouble with the images, or thumbnails, and not having the correct layout based on the size of the screen; they kept stacking on top of each other instead of one row of 4 images for small screens. Finally got that working through media queries, column classes and sizing of the images. Have a better understanding of the meaning behind the 12-column structure in *Bootstrap*. Once all those issues were resolved, added the sidebar code to the 4 *Visualization* pages and the *Home* page.


## Notes

I used weather data for this project but I decided to use the data I had gathered from the earlier project instead of using the files provided. I had already done the analysis on the dataset I had created so it just made more sense to use that again. I had also put a lot of work into creating those files originally so to get the opportunity to put that to good use was appealing.

In the *Plots* dropdown, I disabled the plot if it was the current page being viewed. Seemed like you shouldn't have a link to choose it if you're already on that page. Same for the *Comparisons* and *Data* links.

The navigation bar was quite the challenge. Learned a lot about those various attributes, though, so it was more satisying when I actually got everything to work. The different screen sizes and the navbar background color change dependency what one of the more challenging parts of it.

The sidebar with the thumbnails gave me a run for my money. But the Bootstrap column grid settings finally started to make more sense along the way.

I had such grand ideas for this website but time was not my friend so I didn't get a chance to build it out more. Between the navigation bar and the sidebar, where a good portion of my time was spent, it's amazing my hair hasn't all turned gray!

