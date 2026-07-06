# books-webscraping-project
Multi-level web scraping project (list + detail pages) built with Python, BeautifulSoup &amp; Pandas — includes EDA and visualizations on book pricing and ratings.
# Books Web Scraping Project

## Overview
A web scraping project that extracts book data (title, price, rating, availability, description, UPC) from [books.toscrape.com](http://books.toscrape.com) — a practice site designed for scraping exercises.

## Tech Stack
- Python
- Requests
- BeautifulSoup4
- Pandas
- Matplotlib / Seaborn

## Features
- Scrapes 1000 books across 50 paginated pages
- Multi-level scraping: extracts detail-page data (description, UPC) via nested requests
- Handles encoding issues (UTF-8) for currency symbols
- Implements rate limiting (time.sleep) for ethical scraping
- Includes error handling for failed requests

## Dataset
`books_dataset_full.csv` — 1000 rows, 7 columns (title, price_gbp, availability, rating, book_url, description, upc)

## Analysis
- Price distribution across books
- Average price by rating
- Description length analysis
- In-stock vs out-of-stock breakdown

## Note
Runtime ~8-10 mins due to 1000 detail-page requests with rate limiting.

## Author
Aditi Bhardwaj
