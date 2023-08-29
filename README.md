# Web-Scraping-Challenge

This challenge involves using what was learned in the current module, identifying HTML elements on a page, 
their ids and class attributes, and then using that knowledge to extract information via both automated browsing 
with Splinter and HTML parsing with Beautiful Soup. To fully complete this task I had to collect, organize, analyze the data, 
and then visually communicate my insights.

-- Project Deliverables --

- Deliverable 1: Scrape titles and preview text from Mars news articles.

- Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

-- Part 1: Scrape Titles and Preview Text from Mars News --

I Used an automated browser to visit the Mars news siteLinks to an external site, then inspected the page to identify which elements to scrape. Afterwards I 
extracted the titles and preview text of the news articles that I scraped. Then I stored the scraping results in Python data structures as follows:

- Stored each title-and-preview pair in a Python dictionary and, give each dictionary two keys: title and preview. I then exported the scraped data to a JSON file.

-- Part 2: Scrape and Analyze Mars Weather Data --

For this part I again used an automated browsing to visit the Mars Temperature Data SiteLinks to an external site. Inspected the page to identify which elements to scrape. 
Created a Beautiful Soup object and used it to scrape the data in the HTML table. Assembled the scraped data into a Pandas DataFrame, making sure the columns had the same headings as the 
table on the website. Here’s an explanation of the column headings:

- id: the identification number of a single transmission from the Curiosity rover
  
- terrestrial_date: the date on Earth

- sol: the number of elapsed sols (Martian days) since Curiosity landed on Mars

- ls: the solar longitude

- month: the Martian month

- min_temp: the minimum temperature, in Celsius, of a single Martian day (sol)

- pressure: The atmospheric pressure at Curiosity's location

I also had to examine the data types that were associated with each column and if necessary, cast (or convert) the data to the appropriate datetime, int, or float data types.

After analyzing my dataset using Pandas functions, I had to answer the following questions:

- How many months exist on Mars?

- How many Martian (and not Earth) days worth of data exist in the scraped dataset?

- What were the coldest and the warmest months on Mars (at the location of Curiosity)? To answer this question:

I had to find the average minimum daily temperature for all of the months. The plot the results as a bar chart.

- Which months had the lowest and the highest atmospheric pressure on Mars? To answer this question:

I had to find the average daily atmospheric pressure of all the months. Once that was done I plotted the results as a bar chart.

- How many terrestrial (Earth) days exist in a Martian year? To answer this question:

I had to consider how many days elapse on Earth in the time that Mars circles the Sun once. Also Visually creating an estimate of the
results by plotting the daily minimum temperature. The last thing left to do was export the DataFrame to a CSV file.

*Technologies used: Microsoft Visual Studio Code
