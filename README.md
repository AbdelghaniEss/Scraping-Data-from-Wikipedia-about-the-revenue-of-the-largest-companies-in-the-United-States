# Scraping Largest U.S. Companies by Revenue from Wikipedia

This project focuses on scraping data from Wikipedia to collect information about the revenue of the largest companies in the United States. We stored the scraped data into a pandas DataFrame and performed various data manipulations and explorations.

## Dataset Source

The data was scraped from the Wikipedia page: [List of largest companies in the United States by revenue](https://en.wikipedia.org/wiki/List_of_largest_companies_in_the_United_States_by_revenue).

## Project Overview

### Steps Involved:

1. **Data Scraping**:
   - We used BeautifulSoup and requests to scrape the table containing information about the top companies in the U.S. based on revenue.
   - The data collected includes details such as:
     - Rank
     - Company name
     - Industry
     - Revenue (in USD millions)
     - Revenue growth percentage
     - Number of employees
     - Headquarters location

2. **Data Storage and Manipulation**:
   - After scraping the data, we used pandas to store the data into a DataFrame.
   - Each row in the DataFrame represents a company, and each column contains details about the company such as revenue, employees, and headquarters.

3. **DataFrame Construction**:
   - A pandas DataFrame was created with the following columns:
     - `Rank`: The company's rank based on revenue.
     - `Company`: The company's name.
     - `Industry`: The industry in which the company operates.
     - `Revenue (USD millions)`: The company's revenue in millions of dollars.
     - `Revenue Growth`: The percentage growth or decline in revenue.
     - `Employees`: The number of employees working at the company.
     - `Headquarters`: The location of the company's headquarters.

4. **Data Display**:
   - We explored and printed parts of the DataFrame, such as the first few rows, to ensure the scraping was successful and the data was cleanly stored.

5. **Data Handling**:
   - The DataFrame was displayed using pandas' default settings, which show a few rows from the start and end of the dataset to ensure proper visualization of large datasets.

### Libraries Used:
- **requests**: To send HTTP requests to the Wikipedia page and retrieve the HTML content.
- **BeautifulSoup (bs4)**: To parse the HTML and extract relevant data from the Wikipedia table.
- **pandas**: To store, manipulate, and analyze the scraped data in a DataFrame.


