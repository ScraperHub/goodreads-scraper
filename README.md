<a href="https://crawlbase.com/signup?utm_source=github&utm_medium=readme&utm_campaign=crawling_api_banner" target="_blank">
  <img src="https://github.com/user-attachments/assets/afa4f6e7-25fb-442c-af2f-b4ddcfd62ab2" 
       alt="crawling-api-cta" 
       style="max-width: 100%; border: 0;">
</a>

# Goodreads Ratings & Reviews Scraper

## Description

This repository contains a Python-based scraper for extracting book ratings and reviews from Goodreads. The scraper leverages the [Crawlbase Crawling API](https://crawlbase.com/crawling-api-avoid-captchas-blocks) to bypass bot protections, handle JavaScript rendering, and navigate button-based pagination automatically.

➡ Read the full blog [here](https://crawlbase.com/blog/scrape-goodreads-ratings-and-comments/) to learn more.

## Scraper Overview

### Goodreads Ratings & Reviews Scraper

The `goodreads_scraper.py` extracts the following details for each book:

- **Book Title**
- **Rating**
- **Reviews**

The scraper efficiently handles button-based pagination using the Crawlbase Crawling API, ensuring comprehensive extraction of reviews across multiple pages.

## Environment Setup

Ensure Python is installed on your system. Check the version using:

```bash
python --version
```

Install the required dependencies:

```bash
pip install requests
```

- **requests** – Used for making API calls to Crawlbase.

## Running the Scraper

### 1. Get Your Crawlbase Access Token

- Sign up on [Crawlbase](https://crawlbase.com/signup) to get an API token.
- This token is required to access the Crawling API for bypassing bot protection.

### 2. Update the Scraper with Your Token

Replace "`CRAWLBASE_JS_TOKEN`" in the script with your Crawlbase Crawling API Token.

### 3. Run the Scraper

```bash
python goodreads_scraper.py
```

The extracted book ratings and reviews will be saved in a JSON file.

## To-Do List

- Extract additional book details like author, genres, and publication year.
- Implement support for filtering reviews based on rating (e.g., only 5-star reviews).
- Add export options for CSV and database storage.
- Optimize request handling for large-scale scraping.
