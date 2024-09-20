Versatile Amazon Product Scraper
This Python script is a flexible web scraping tool designed to extract product information from any category on Amazon. It uses Selenium WebDriver with Microsoft Edge to automate web browsing and data collection.
Key features and components:

Versatile Scraping: Can scrape any product category on Amazon by changing the input URL.
Driver Initialization: Sets up the Selenium WebDriver for Microsoft Edge.
Data Extraction: The scrape_data() function navigates through multiple pages of Amazon search results, extracting:

Product names
Prices
Categories
Product links


Multi-page Scraping: Currently configured to scrape 7 pages of search results, but this can be adjusted.
Data Processing: Collected data is structured into a pandas DataFrame for easy manipulation and analysis.
Data Storage: Scraped information is saved to a CSV file, with the filename reflecting the scraped category (e.g., 'amazon_Movies_TV_Shows.csv').
Error Handling: Implements basic error catching, particularly for navigation issues and element loading.
Customizable: The URL can be easily changed to scrape different product categories or even different Amazon domains.

Usage:

Set the desired Amazon search URL.
Run the script to initiate the scraping process.
The script will navigate through the specified number of pages, collecting product data.
Data is saved to a CSV file upon completion.

Note: While the current implementation requires manual execution, it provides a solid foundation for further automation, such as scheduled runs or integration into larger data collection systems.
