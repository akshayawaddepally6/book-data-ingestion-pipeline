# Book Data Ingestion Pipeline

This project is a complete data engineering pipeline built to extract, transform, and load (ETL) book data from Goodreads. It automates the process of ingesting book metadata and user reviews, cleaning and transforming the data, and loading it into a PostgreSQL database for further analysis or downstream applications.

## 🔍 Overview

The pipeline focuses on building a scalable and modular ETL process using Python. It is ideal for anyone looking to understand the basics of working with real-world web data, handling messy datasets, and setting up a structured data flow into a database.

## 📌 Key Features

* **Data Extraction**: Scrapes book and review data from the Goodreads website.
* **Data Transformation**: Cleans and normalizes scraped data using pandas.
* **Data Loading**: Stores the processed data in a PostgreSQL database using SQLAlchemy.
* **Modular Codebase**: Each ETL stage is separated into its own module for better maintainability and scalability.
* **Logging & Error Handling**: Integrated logging to track the pipeline’s execution and handle errors gracefully.

## ⚙️ Technologies Used

* Python 3
* BeautifulSoup (for web scraping)
* pandas (for data transformation)
* SQLAlchemy (for ORM and DB communication)
* PostgreSQL (as the data warehouse)
* dotenv (for environment management)
* Logging module (for pipeline monitoring)

## 📁 Project Structure

```
goodreads_etl_pipeline/
│
├── extract/
│   └── extract_books.py
│
├── transform/
│   └── transform_books.py
│
├── load/
│   └── load_books.py
│
├── config/
│   └── db_config.py
│
├── utils/
│   └── helpers.py
│
├── .env
├── main.py
└── requirements.txt
```

## 📊 Example Use Case

The extracted and processed Goodreads data can be used to:

* Perform sentiment analysis on reviews
* Identify highly-rated books by genre or author
* Power recommendation systems
* Conduct trend analysis in book popularity

---

