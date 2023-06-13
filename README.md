# ScrapeNews.py Documentation

ScrapeNews.py is a Python script that scrapes top news stories from the Associated Press (AP) website and stores them in a CSV file. 
This script uses the Scrapy library to extract data from HTML pages.

## Usage

To use this script, simply run it in a Python environment. The `scrape_top_news()` function will perform the scraping and store the 
results in a CSV file called `stored_articles.csv`.

```python
if __name__ == "__main__":
  scrape_top_news()
```

Note that running this script may take a while to execute as there are built-in timers to slow down the scraping process. 
Additionally, there is a risk of being blacklisted by the site being scraped due to excessive requests.

## Functionality

The `scrape_top_news()` function executes three main steps:

1. Extracts links to top news stories from the AP website.
2. Follows each link and extracts the article title and body.
3. Stores the link, title, and body for each article in a CSV file.

These steps are performed by two parsing methods within a Scrapy spider:

1. `parse1()`: Extracts links to top news stories.
2. `parse2()`: Follows each link and extracts article title and body.

The spider has built-in timers between requests as an attempt to avoid being labeled as a bot by the AP website.

## Output

The output of this script is stored in a CSV file called `stored_articles.csv`. This file contains three columns: 
Link, Title, and Body. The Link column contains URLs to each news story, while the Title column contains the article's title. 
The Body column contains the article's content.

## Conclusion

This program was created purely for informational purposes and should not be used in violation of any policies or regulations. 
The user is fully responsible for any effects or implications that using this software may result in. 
ScrapeNews.py is an effective tool for scraping top news stories from the AP website. It uses Scrapy to extract data from HTML 
pages and stores it in an easy-to-use CSV file. However, caution should be exercised when running this script as there is a 
risk of being blacklisted by the site being scraped.
