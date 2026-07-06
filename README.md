# books-webscraping-project
Multi-level web scraping project (list + detail pages) built with Python, BeautifulSoup &amp; Pandas — includes EDA and visualizations on book pricing and ratings.
# 📚 Books Web Scraping & EDA Project

A Python-based web scraping project that extracts and analyzes data for **1000 books** from [books.toscrape.com](http://books.toscrape.com) — a site built specifically for scraping practice. The project covers everything from multi-page scraping and nested detail-page extraction to data cleaning and exploratory data analysis (EDA).

---

## 🔍 Overview

This project demonstrates an end-to-end data collection pipeline:

1. **Scrape** book listings across 50 paginated pages
2. **Extract** detailed info (description, UPC) by visiting each book's individual page
3. **Clean** and structure the data using Pandas
4. **Analyze** pricing, ratings, and stock trends through visualizations

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| `requests` | Fetching HTML pages |
| `BeautifulSoup4` | Parsing HTML and extracting data |
| `pandas` | Data structuring and analysis |
| `matplotlib` / `seaborn` | Data visualization |
| `time` | Rate limiting for ethical scraping |

---

## ✨ Features

- ✅ Scrapes **1000 books** across 50 paginated listing pages
- ✅ **Multi-level scraping** — follows each book's link to a detail page for extra data (description, UPC)
- ✅ Handles **UTF-8 encoding issues** for special characters (currency symbol £)
- ✅ Implements **rate limiting** (`time.sleep`) to scrape responsibly
- ✅ Includes **error handling** for failed requests and missing data
- ✅ Clean, reusable functions for scraping and parsing

---

## 📊 Dataset

**File:** `books_dataset_full.csv`
**Rows:** 1000 | **Columns:** 7

| Column | Description |
|--------|-------------|
| `title` | Book title |
| `price_gbp` | Price in GBP (£) |
| `availability` | In stock / Out of stock |
| `rating` | Star rating (1–5) |
| `book_url` | Link to book's detail page |
| `description` | Book summary/description |
| `upc` | Unique product code |

---

## 📈 Analysis & Visualizations

- Distribution of book prices
- Number of books by star rating
- Average price by rating
- In-stock vs out-of-stock breakdown
- Description length distribution

---

## 📂 Project Structure

```
books-webscraping-project/
│
├── books_scraping.ipynb      # Full scraping + analysis notebook
├── books_dataset_full.csv    # Final cleaned dataset
└── README.md                 # Project documentation
```

---

## ⚙️ How to Run

```bash
pip install requests beautifulsoup4 pandas matplotlib seaborn
```

Open `books_scraping.ipynb` in Jupyter Lab/Notebook and run all cells.

> ⏱️ **Note:** Full run takes ~8–10 minutes due to 1000 detail-page requests with built-in rate limiting.

---

## 🎯 Key Learnings

- Handling pagination in web scraping
- Nested/multi-level scraping (list page → detail page)
- Encoding-related bug fixing (UTF-8 decode issues)
- Structuring scraped data into a clean, analysis-ready format
- Ethical scraping practices (rate limiting, error handling)

---

## 👩‍💻 Author

**Aditi Bharti**
[GitHub](https://github.com/aditib145) • [Kaggle](https://www.kaggle.com/aditib145)

---

⭐ If you found this project useful, consider giving it a star!
