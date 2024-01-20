# Amazon Web Scraping Script

This Python script is designed to perform web scraping on Amazon to extract product details such as title, price, and rating. It uses the BeautifulSoup library for parsing HTML and requests for making HTTP requests.

## Prerequisites

Make sure you have the following Python libraries installed:

- requests
- BeautifulSoup
- pandas
- numpy

You can install them using the following:

```bash
pip install requests beautifulsoup4 pandas numpy

Usage
Open the script in your preferred Python environment or text editor.

Add your user agent in the HEADERS variable. This helps mimic a web browser to avoid detection.

python
Copy code
HEADERS = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36', 'Accept-Language': 'en-US, en;q=0.5'}
Modify the URL variable with the desired Amazon search results page URL.

python
Copy code
URL = "https://www.amazon.ca/s?k=mouse+pad&crid=3UDNLUNA6F8CC&sprefix=mouse%2Caps%2C88&ref=nb_sb_ss_ts-doa-p_1_5"
Run the script. It will scrape the product details from the provided Amazon search results page.

The extracted information will be stored in a CSV file named amazon_data.csv. The CSV file will contain columns for title, price, and rating.

Functions
1. get_title_website(webScraping)
Extracts the product title from the given BeautifulSoup object.
2. get_price_website(webScraping)
Extracts the product price from the given BeautifulSoup object.
3. get_rate_product(webScraping)
Extracts the product rating from the given BeautifulSoup object.

