# ETL-Pipeline-for-E-Commerce-Data
**Shopify Data Extraction & Storage Project**
Project Overview

This project extracts publicly available product data from the Allbirds Shopify store, processes it, and stores it in Google Sheets for further analysis. The goal is to automate data retrieval and create a structured dataset for future visualization and analytics.
Tech Stack

    Python (requests, pandas, gspread, oauth2client)
    Google Sheets API (for storing extracted data)

Project Workflow
1. Data Extraction from Shopify

    Connected to Shopify API using a public endpoint.
    Fetched product details such as title, vendor, type, published date, price, and image URL.
    Handled API authentication errors (401 - Invalid API key).

2. Data Storage in Google Sheets

    Used gspread and Google Sheets API to store extracted data.
    Cleared old data and inserted updated product details dynamically.

Challenges & Solutions

    401 Error in API Calls → Used correct Shopify API authentication.
    Data Formatting Issues → Cleaned data using Pandas before pushing to Google Sheets.

Future Enhancements

    Automate data updates using a scheduler (cron job/Airflow).
    Use Grafana for real-time visualization.
    Implement ETL pipeline to store data in a SQL database.
