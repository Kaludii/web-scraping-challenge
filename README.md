## Module 12 Challenge

This assignment consists of two technical products.

* Deliverable 1: Scrape titles and preview text from Mars news articles. 

* Deliverable 2: Scrape and analyze Mars weather data, which exists in a table.

### Deliverable 1: Scrape Titles and Preview Text from Mars News (40 points)

1. Created a new Jupyter notebook named `mars_data_challenge_part_1.ipynb`.

2. Scraped the [Mars News](https://redplanetscience.com) website by using Splinter and Beautiful Soup. Specifically, scraped the title and preview text of each article on the landing page.

3. Stored the scraping results in Python data structures as follows:

    * Stored all the dictionaries in a Python list.

    * Printed the list in the notebook.

4. Optionally, stored the scraped data into a json file then converted and downloaded as a csv file to ease sharing the data with others.

### Deliverable 2: Scrape and Analyze Mars Weather Data (60 points)

1. Created a Jupyter notebook named `mars_data_challenge_part_2.ipynb`. Import the relevant dependencies for web scraping, Pandas, and Matplotlib.

2. With the automated browser, visited the [Mars Temperature Data](https://data-class-mars-challenge.s3.amazonaws.com/Mars/index.html) site.

3. Scraped the data in the HTML table using Splinter and Beautiful Soup.

4. Assembled the scraped data into a Pandas DataFrame. The columns have the same headings as the table on the website. Here’s are the column headings:

    - The `id` heading: The identification number of a single transmission from the Curiosity rover.
    - The `terrestrial_date` heading: The date on Earth.
    - The `sol` heading: The number of elapsed sols (Martian days) since Curiosity landed on Mars.
    - The `ls` heading: The solar longitude.
    - The `month` heading: The Martian month.
    - The `min_temp` heading: The minimum temperature, in Celsius, of a single Martian day (sol).
    - The `pressure` heading: The atmospheric pressure at Curiosity's location.

5. Examined the data types of all the DataFrame columns. Converted the data to the appropriate `datetime`, `int`, or `float` data types.

6. Answered the following question: How many months exist on Mars?

7. Answered the following question: How many Martian (and not Earth) days worth of data exist in the scraped dataset?

8. Answered the following question: What are the coldest and the warmest months on Mars (at the location of Curiosity)? Got the answer by averaging the minimum daily temperature of all the months. Plotted the results as a bar chart.

9. Answered the following question: Which months have the lowest and the highest atmospheric pressure on Mars? Got the answer by averaging the daily atmospheric pressure of all the months. Plotted the results as a bar chart.

10. Answered the following question: About how many terrestrial (Earth) days exist in a Martian year? That is, in the time that Mars circles the Sun once, how many days elapse on Earth? Visually estimated the result by plotting the daily minimum temperature.

11. Exported the DataFrame to a CSV file.