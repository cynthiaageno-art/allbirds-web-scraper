# Group 9: Allbirds Web Scraping and Data Analysis

## Project Overview
This project applies web scraping, data cleaning, database management, and exploratory data analysis to publicly accessible Allbirds product information. The project is part of the DSC2107 Data Mining and Wrangling course at Uganda Christian University.

## Objectives

- Practise web scraping using Books to Scrape.
- Examine the target website and its crawling rules.
- Collect and preserve product data where access is permitted.
- Clean and transform the collected data using Python and Pandas.
- Store product information and time-stamped observations in SQLite.
- Analyse product prices, categories, and availability.
- Visualise findings using Matplotlib.

## Technologies Used

- Python
- Requests
- BeautifulSoup
- Pandas
- SQLite
- Matplotlib
- NumPy
- Jupyter Notebook

## Project Structure

```
WEB SCRAPING/
├── day1_books_practice.ipynb
├── reconnaissance.ipynb
├── scraper.ipynb
├── clean_load.ipynb
├── analysis.ipynb
├── extra_analysis.ipynb
├── requirements.txt
├── README.md
├── data/
│   ├── raw/
│   ├── clean/
│   └── allbirds.db
└── outputs/
    └── charts/
```

## Database
The SQLite database is stored at `data/allbirds.db`.

It contains two main tables:

- `products`: stores product details.
- `observations`: stores variant-level observations with collection timestamps.

## Installation
Install the required packages by running:

```
python -m pip install -r requirements.txt
```

## Execution
Run the notebooks in the appropriate order:

1. `day1_books_practice.ipynb`
2. `reconnaissance.ipynb`
3. `scraper.ipynb`
4. `clean_load.ipynb`
5. `analysis.ipynb`
6. `extra_analysis.ipynb`

## Responsible Data Collection
Collection must respect the website's access rules and applicable restrictions. The project does not attempt to bypass access controls. Raw data, collection dates, and limitations should be documented.

## Group Members
Agenorwot Cynthia Jillian
Ayoo Alice
Ngobi Jonah
Jjumba 
Keji Flora

## Status
The project is under development. Final findings should be based on successfully collected and validated data.