# Job Scraper

This project is a web scraper that collects job postings from superjob.ru and hh.ru using Scrapy.

## Features

The scraper collects the following information for each job posting:

- **Job Title**
- **Salary From**
- **Salary To**
- **Salary Currency**
- **Job URL**
- **Source Website**

## How it Works

The scraper navigates through superjob.ru and hh.ru, extracting relevant details from job postings. The collected data is then stored in a database of your choice.

Install Dependencies:

bash

pip install -r requirements.txt

Run the Scraper:

bash

scrapy crawl job_spider
    This will initiate the scraper to start collecting job postings.

    Configure Database:

    Update the database configuration in settings.py with your preferred database details.

    View the Data:

    Check your database to see the collected job postings.

Database Schema

The database schema includes tables for storing job details:

    jobs
        id (Primary Key)
        title (Job Title)
        salary_from (Salary From)
        salary_to (Salary To)
        currency (Salary Currency)
        url (Job URL)
        source (Source Website)

Feel free to customize the database schema as needed.
