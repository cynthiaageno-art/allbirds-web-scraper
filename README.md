# Allbirds Web Scraping Project

A Python-based web scraping project designed to extract product data from the Allbirds website, including product names, prices, descriptions, and other relevant details for data collection and analysis. Built to explore web scraping techniques and structured data extraction using Python.

## 1. Project Description

This project uses Python to collect publicly accessible product information from the Allbirds Shopify JSON feed (`https://www.allbirds.com/products.json`) for learning and data analysis. The main workflow is in `Group9_Allbirds_Scraper.ipynb`.

## 2. Objectives

- Learn and practise web scraping using Python.
- Collect publicly accessible Allbirds product information.
- Organise and analyse the collected data.
- Understand how web scraping works in real-world applications.

## 3. Technologies Used

- Python — programming language and standard-library support for JSON, SQLite, and `robots.txt` checks.
- Requests — sends HTTP requests to the public product feed.
- Pandas — processes and organises product data.
- Jupyter Notebook and Visual Studio Code — run and edit the scraping workflow.
- Git and GitHub — version control and project hosting.

The scraper consumes structured JSON directly, so it does not use BeautifulSoup to parse HTML.

## 4. Project Features

- Checks `robots.txt` before accessing the product feed.
- Retrieves paginated product data with retries and polite delays.
- Saves raw JSON and flattened CSV snapshots.
- Stores product, variant, and observation data in SQLite.
- Supports further analysis of the collected product information.

## 5. Installation and Setup

### Prerequisites

- Python 3 installed on your computer.
- Git installed if you plan to clone the repository.
- Jupyter support in Visual Studio Code, or another Jupyter environment.

### Install Dependencies

Open a terminal and run:

```bash
pip install requests pandas
```

## 6. How to Run the Project

1. Clone or download this repository.
2. Open the `Assignment` project folder in Visual Studio Code.
3. Install the required dependencies.
4. Open `Group9_Allbirds_Scraper.ipynb` and run its cells in order.
5. Review the generated dated JSON and CSV files in `raw/` and the SQLite database.

The scraper checks the site's `robots.txt` rules and stops if the feed is disallowed. The public feed and its availability can change; document blocked requests or errors instead of bypassing access controls.

## 7. Project Structure

```text
Assignment/
├── README.md
├── Group9_Allbirds_Scraper.ipynb
├── Warm-up.ipynb
├── books_toscrape.csv
├── allbirds.db
├── RECONNAISSANCE NOTE.docx
└── raw/
	├── allbirds.db
	├── allbirds_flat_2026-10-13.csv through allbirds_flat_2026-10-19.csv
	├── allbirds_raw_2026-10-13.json through allbirds_raw_2026-10-19.json
	└── books_toscrape.csv
```

The October 13 files are a documented backfill based on the October 14 snapshot, not an independent scrape from October 13. They must not be counted as a verified additional collection day. A new scrape records the site at the time it runs and cannot reconstruct past site data.

## 8. Responsible Web Scraping

This project is intended for educational purposes. Scraping should respect the website's terms of service, `robots.txt` rules, applicable rate limits, and privacy requirements. Do not bypass access controls.

## 9. Author

Group 9
