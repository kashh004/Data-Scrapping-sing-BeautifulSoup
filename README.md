# Data-Scrapping-using-BeautifulSoup
This project demonstrates how to scrape quotes from the website [Quotes to Scrape](http://quotes.toscrape.com/) using the BeautifulSoup library in Python. The script collects quotes, authors, and associated tags, and saves the data into a CSV file for easy analysis and storage.

## Features
- Scrapes multiple pages of quotes.
- Extracts quote text, author names, and tags.
- Saves the collected data into a CSV file.

## Prerequisites

1. **Python**: Ensure you have Python 3.x installed on your machine.
2. **Install Required Libraries**: 
   - Install the necessary packages by running:
     ```bash
     pip install requests beautifulsoup4 pandas
     ```

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/quote-scraper.git
   ```

2. **Navigate to the Project Directory**:
   ```bash
   cd quote-scraper
   ```

3. **Install Dependencies**: 
   Make sure to install the required Python libraries as mentioned above.

## Usage

1. **Run the Script**:
   To execute the quote scraping tool, run the following command:
   ```bash
   python quotes_scraper.py
   ```

2. **Output**:
   The script will create a file named `quotes.csv` in the project directory containing the scraped quotes, authors, and tags.

## Example Output
The `quotes.csv` file will contain data structured like this:

| Quote                                             | Author              | Tags                     |
|---------------------------------------------------|---------------------|--------------------------|
| "The world as we have created it is a process of our thinking." | Albert Einstein      | change, deep-thought, thinking, world |
| "It is our choices, Harry, that show what we truly are, far more than our abilities." | J.K. Rowling         | abilities, choices, harry, truth |

## Challenges Faced

- **Changing Website Structure**: The website's HTML structure may change, affecting the scraping logic. Always inspect the webpage and update the selectors accordingly.
  
- **Rate Limiting**: Making too many requests in a short period can lead to being blocked. Implement delays between requests to mimic human browsing behavior.
  
- **Handling Pagination**: Correctly managing pagination is crucial to scrape all quotes from the website.
