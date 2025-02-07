# Jumba Stores - AliExpress Data Scraping and Database Integration
This project scrapes portable generator product data from AliExpress and loads it into a PostgreSQL database. The script extracts product details such as names, prices, discounts, original prices, ratings, and quantity sold, processes the data, and stores it in structured database tables.

## Overview
The script performs the following tasks:

1. Web Scraping:

    + Uses Selenium and BeautifulSoup to scrape product data from AliExpress.
    + Extracts product names, stores, prices, discounts, original prices, ratings, and quantity sold.
    + Handles pagination to scrape multiple pages.

2. Data Processing:

    + Cleans and transforms the scraped data (e.g., removing currency symbols, extracting discount percentages).
    + Splits the data into three tables: products, sales, and discount.

3. Database Integration:

    + Connects to a PostgreSQL database using credentials from an environment file.
    + Loads the processed data into the respective tables in the EDW schema.

### Key Features
1. Web Scraping: Extracts product data from AliExpress using Selenium and BeautifulSoup.
2. Data Cleaning: Processes and transforms raw scraped data into a clean format.
3. Database Integration: Automates data loading into a PostgreSQL database.

### Repository Contents
  + Script: The main Python script for scraping and database integration.
  + Output: Processed data saved as CSV files (product_table.csv, sales_table.csv, discount_table.csv) and loaded into PostgreSQL.

### Prerequisites
  + Python 3.x
  + Libraries: selenium, beautifulsoup4, requests, pandas, sqlalchemy, python-dotenv
  + PostgreSQL database.
  + Microsoft Edge WebDriver

**For any questions or issues, please open an issue in the repository. Contributions are welcome! Thank You!!!**
