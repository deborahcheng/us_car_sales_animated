# Top 10 US Car Sales by Brand

One of the most viewed types of videos on YouTube are the Top 10 type videos. While there are a lot of different type of Top 10 videos, including Top 10 things you don't know about a celebrity or the Top 10 fastest trains, there are also videos that simply gathers data and visualize it as an animation. This is an attempt to produce a similar animated visualization of the cummulated US car sales by brand over the years by using Python and scrapping the required data on the web by using Beautifulsoup.

## Data

The data was obtained from the website, [Car Sales Base](https://carsalesbase.com/), where it gathers and displays the information of unit car sales for each brand on separate webpages. Therefore, in order to obtain the data for all the brands, I first determined all the links to the different brands, then scrapped each of the links separately using a for loop. The scraped data is then concated into a single dataframe.

### Data Cleaning

Since the data is very simple, there wasn't much data cleaning to do other than filling NAs.

## Graph

Like the animate graph for fertility vs birth rate, placing the data on a graph was relatively simple. However, I was surprised to see that the rank() method does not rank the most sales as #1, but instead, the higher the amount, the higher the rank. This was a bit of a surprise, as we usually regard #1 ranking as best. Regardless, once I understood the rank() method, the rest of making the graph more esthetically pleasing.

Here's the final product:

<img src="https://github.com/deborahcheng/us_car_sales_animated/raw/main/us_car_sales.gif">

## References
https://towardsdatascience.com/introduction-to-web-scraping-with-beautifulsoup-e87a06c2b857
https://medium.com/dunder-data/create-a-bar-chart-race-animation-in-python-with-matplotlib-477ed1590096
