# Module 11: web-scraping-challenge

Background
-----------------------
You’re now ready to take on a full web-scraping and data analysis project. You’ve learned to identify HTML elements on a page, identify their id and class attributes, and use this knowledge to extract information via both automated browsing with Splinter and HTML parsing with Beautiful Soup. You’ve also learned to scrape various types of information. These include HTML tables and recurring elements, like multiple news articles on a webpage.
As you work on this Challenge, remember that you’re strengthening the same core skills that you’ve been developing until now: collecting data, organizing and storing data, analyzing data, and then visually communicating your insights.

Part 1: Scrape Titles and Preview Text from Mars News
-----------------------
Open the Jupyter Notebook in the starter code folder named part_1_mars_news.ipynb. You will work in this code as you follow the steps below to scrape the Mars News website.
1/ Use automated browsing to visit the Mars news site. Inspect the page to identify which elements to scrape.
2. Create a Beautiful Soup object and use it to extract text elements from the website.
3. Extract the titles and preview text of the news articles that you scraped. Store the scraping results in Python data structures as follows:
a. Store each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview.
b. Store all the dictionaries in a Python list.
c. Print the list in your notebook.

Part 2: Scrape and Analyze Mars Weather Data
-----------------------
Open the Jupyter Notebook in the starter code folder named part_2_mars_weather.ipynb. You will work in this code as you follow the steps below to scrape and analyze Mars weather data.
1. Use automated browsing to visit the Mars Temperature Data Site. Inspect the page to identify which elements to scrape. Note that the URL is https://static.bc-edx.com/data/web/mars_facts/temperature.html.
2. Create a Beautiful Soup object and use it to scrape the data in the HTML table. Note that this can also be achieved by using the Pandas read_html function. However, use Beautiful Soup here to continue sharpening your web scraping skills.
3. Assemble the scraped data into a Pandas DataFrame. The columns should have the same headings as the table on the website.
4. Examine the data types that are currently associated with each column. If necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.
5. Analyze your dataset by using Pandas functions to answer the following questions:
a. How many months exist on Mars?
b. How many Martian (and not Earth) days worth of data exist in the scraped dataset?
c. What are the coldest and the warmest months on Mars (at the location of Curiosity)?

![avg_temp_by_month](https://github.com/alanisrperez/web-scraping-challenge/blob/main/Outputs/avg_temp_by_month.png)

![avg_temp_by_month_sorted](https://github.com/alanisrperez/web-scraping-challenge/blob/main/Outputs/avg_temp_by_month_sorted.png)

d. Which months have the lowest and the highest atmospheric pressure on Mars?

![pressure_by_month](https://github.com/alanisrperez/web-scraping-challenge/blob/main/Outputs/pressure_by_month.png)

e. About how many terrestrial (Earth) days exist in a Martian year?

![terrestrial_days](https://github.com/alanisrperez/web-scraping-challenge/blob/main/Outputs/terrestrial_days.png)

6. Export the DataFrame to a CSV file.

References
-----------------------
The Mars News website (https://static.bc-edx.com/data/web/mars_news/index.html) is operated by edX Boot Camps LLC for educational purposes only.
The news article titles, summaries, dates, and images were scraped from NASA's Mars News website (https://science.nasa.gov/mars/) in November 2022.
Images are used according to the JPL Image Use Policy (https://www.jpl.nasa.gov/jpl-image-use-policy), courtesy NASA/JPL-Caltech.