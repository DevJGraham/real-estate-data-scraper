# Real Estate Data Extractor

## Overview

The Real Estate Data Extractor efficiently gathers data from the Allegheny County Real Estate Portal. Designed to extract key property details such as property address, owner's mailing address, sale date, and sale price, this tool allows users to input the street name and municipality (optional) to quickly collect comprehensive data across multiple entries. The collected data is then compiled into a CSV file, facilitating easy analysis and insight generation.

## Features

- **Data Extraction**: Automates the extraction of whatever data points are most valuable to the client, for example, Owner Mailing Address, Sale Date and Price, etc. 
- **Concurrency**: Employs Asyncio and Aiohttp to enhance data gathering efficiency through parallel processing.
- **Data Export**: Organizes and outputs the collected data into a structured CSV file for further use.

## What I Learned

The development of the Real Estate Data Extractor provided valuable insights and skills enhancement in key areas:

- **Advanced Web Scraping**: Mastered techniques for extracting data not directly embedded in HTML, utilizing tools such as Selenium and XPath to handle elements without clear HTML labels.
- **Data Exporting**: Employed Pandas to efficiently organize scraped data into dataframes and export it into CSV format, optimizing data storage and accessibility.
- **Optimization of Data Collection**: Refined the web scraping process by minimizing the use of Selenium. Instead, data used to extrapolate URLs were utilized to fetch data asynchronously without a browser, thereby enhancing the efficiency of data collection.
- **Concurrency with Asyncio**: Implemented Asyncio and Aiohttp for effective management of asynchronous tasks, enabling the parallel execution of data retrieval operations which significantly improved performance.
- **Problem-Solving and Debugging**: Developed sophisticated problem-solving abilities by troubleshooting issues related to extracting data from dynamically generated content and handling data without clear HTML structures.

These advancements not only enhanced technical capabilities but also honed analytical and problem-solving skills, preparing for complex data processing challenges in future roles.
