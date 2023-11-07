# WebScraping_challenge
 ## Part 1 : Scrape Titles and Preview Text from Mars News
 Following tasks are performed in the notebook part_1_mars_news.ipynb:
 1. Used automated browsing to visit the [Mars news](https://static.bc-edx.com/data/web/mars_news/index.html) and inspected the page to identify which elements to scrape
 2. Created a Beautiful Soup object and used it to extract text elements(articles) from the website
 3. Extracted the titles and preview text of the news articles that were scraped. Stored the scraping results in Python data structures as follows:
    1. Stored each title-and-preview pair in a Python dictionary(article_dict) and gave each dictionary two keys: title and preview
    2. Stored all the dictionaries in a Python list(artilces_list)
    3. Printed the list in your notebook

 ## Part 2 : Scrape and Analyze Mars Weather Data
 Following tasks are performed in the notebook part_2_mars_weather.ipynb:
 1. Used automated browsing to visit the [Mars Temperature Data](https://static.bc-edx.com/data/web/mars_facts/temperature.html) and inspected the page to identify which elements to scrape
 2. Created a Beautiful Soup object and used it to scrape the data in the HTML table
 3. Assembled the scraped data into a Pandas DataFrame(mars_df). The columns have the same headings as the table on the website
 4. Converted the data to datetime, int, or float data types as follows:
    id                          object
    terrestrial_date    datetime64[ns]
    sol                          int64
    ls                           int64
    month                        int64
    min_temp                   float64
    pressure                   float64
 5. Analyzed the dataset by using Pandas functions to answer the following questions:
    1. How many months exist on Mars?
    2. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
    3. What are the coldest and the warmest months on Mars (at the location of Curiosity)?
        Find the average minimum daily temperature for all of the months
        Plot the results as a bar chart
    4. Which months have the lowest and the highest atmospheric pressure on Mars?
        Find the average daily atmospheric pressure of all the months.
        Plot the results as a bar chart.
    5. About how many terrestrial (Earth) days exist in a Martian year?
        Consider how many days elapse on Earth in the time that Mars circles the Sun once.
        Visually estimate the result by plotting the daily minimum temperature.
 6. Exported the DataFrame to a CSV files(MarsWeather.csv, MarsTemperature.csv and MarsPressure.csv)
