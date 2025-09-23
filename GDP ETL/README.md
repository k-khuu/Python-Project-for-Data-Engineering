# 🌍 Countries by GDP ETL Project

## Overview

An international firm expanding its global footprint has tasked you, a Junior Data Engineer, with building an automated ETL pipeline to extract and process GDP data for all countries. The source is the International Monetary Fund (IMF), which publishes nominal GDP evaluations twice a year.

This project automates the retrieval, transformation, and storage of GDP data—making it accessible for strategic decision-making and future updates.

---

## 📊 Data Source

The GDP data is sourced from the [IMF's nominal GDP list](https://web.archive.org/web/20230902185326/https://en.wikipedia.org/wiki/List_of_countries_by_GDP_%28nominal%29), archived for consistency.

---

## 🛠️ What the Script Does

The Python script `etl_project_gdp.py` performs the following tasks:

1. **Extract**  
   - Scrapes the GDP table from the IMF webpage using BeautifulSoup.

2. **Transform**  
   - Cleans and converts GDP values from USD millions to USD billions.  
   - Rounds GDP figures to 2 decimal places.

3. **Load**  
   - Saves the data to:
     - A JSON file: `Countries_by_GDP.json`  
     - A SQLite database: `World_Economies.db`  
       - Table name: `Countries_by_GDP`  
       - Columns: `Country`, `GDP_USD_billion`

4. **Query**  
   - Runs a SQL query to display countries with GDP > 100 billion USD.

5. **Logging**  
   - Logs each step of the ETL process to `etl_project_log.txt`.

---

## 📁 Output Files

- `Countries_by_GDP.json`  
- `World_Economies.db`  
- `etl_project_log.txt`

---

## 🧪 Success Criteria

To validate the ETL pipeline:
- Run the script and confirm that the database table contains only countries with GDP > 100 billion USD.
- Check the log file for a complete trace of execution.

---

## 🐍 Requirements

- Python 3.x  
- Libraries:
  - `requests`
  - `beautifulsoup4`
  - `pandas`
  - `numpy`
  - `sqlite3`

Install dependencies using:

```bash
pip install requests beautifulsoup4 pandas numpy
```

---

## 🚀 Run the Project

```bash
python etl_project_gdp.py
```

---

## 📌 Notes

- The script is designed to be rerun biannually as IMF updates its GDP evaluations.
- You can modify the source URL or database query logic to adapt to future data formats.
