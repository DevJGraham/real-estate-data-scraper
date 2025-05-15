# 🏠 Allegheny County Real Estate Web Scraper

A Python-based web scraper built to collect detailed property data from the Allegheny County Real Estate portal. Designed to assist real estate professionals, data analysts, and developers, this tool automates the process of gathering property-level information across multiple municipalities.

> This public README showcases the capabilities and technologies used for this tool. 
>
> If you would like to access the code base for this web scraper. Reach out to me on [LinkedIn](https://www.linkedin.com/in/davidgraham-cs/) or send me an [email](mailto:davidgraham7447@gmail.com).

---

## 📌 Technical Overview

This project combines **Selenium** and **aiohttp** to efficiently gather property data from the Allegheny County Real Estate portal. **Selenium** is used to navigate the site and extract parcel information because the search results and pagination are dynamically loaded via JavaScript, using mechanisms like `__doPostBack(...)`. As such, a real browser environment is required to interact with the page and retrieve the data needed for the next step.

Once parcel data is collected, the corresponding URLs for each property are generated. These URLs are then processed asynchronously using **aiohttp** and **asyncio**, allowing the scraper to retrieve HTML content from multiple property pages in parallel. **BeautifulSoup** is used to parse the content and extract structured data, which is then compiled into a clean, downloadable **CSV** file.

Given a list of street names and matching municipalities, the scraper automates the entire process and outputs an analysis-ready dataset containing detailed property information.

---

## 📊 Data Collected

For each property, the scraper extracts:

- `property_address`
- `municipality`
- `owner_name`
- `owner_mailing`
- `sale_date`
- `sale_price`
- `lot_area_sqft`
- `bedroom_count`
- `bathroom_count`
- `use_code`
- `living_area_sqft`
- Tax status for the current year and three prior years

---

## 🛠️ Technologies Used

- Python 3.11
- Selenium
- aiohttp + asyncio
- BeautifulSoup
- Pandas

---

## 📁 Example Output

You can view a sample of the output data here:  
📂 [`Sample Output CSV`](sample_output.csv)

*Note that the owner name and mailing address are not included in the sample output.*

The CSV contains one row per property with each of the fields listed above, ideal for downstream analysis or integration into a real estate workflow.

---

## 💡 Potential Use Cases

- Analyzing local markets and identifying comparable properties for valuation
- Identifying warmer leads by filtering properties based on ownership, sale history, or tax status
- Powering real estate dashboards and data visualizations with structured property data
- Supporting more informed offer negotiations with historical and contextual property insights


---

## 🚧 Future Enhancements

- Add a simple front-end UI for selecting municipalities or zip codes
- Improve HTML scraping speed and fault tolerance
- Docker support for streamlined deployment

---

## 📬 Contact

If you have questions, suggestions, or would like to collaborate:

📧 [davidgraham7447@gmail.com](mailto:davidgraham7447@gmail.com)

🔗 [LinkedIn](https://www.linkedin.com/in/davidgraham-cs/)

---

