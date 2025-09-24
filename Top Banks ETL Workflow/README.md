# 🏦 Largest Banks ETL Project

This project automates the extraction, transformation, and loading (ETL) of market capitalization data for the world’s top banks. Built as part of a data engineering exercise, it demonstrates real-world ETL workflows using Python and SQLite.

## 📌 Project Scenario

You’ve been hired by a financial research organization to compile and process a quarterly report on the **top 10 largest banks in the world**, ranked by **market capitalization in USD**. The data is extracted from an archived Wikipedia page, converted into **GBP, EUR, and INR** using exchange rates from a CSV file, and stored both as a **CSV file** and a **SQLite database table**.

## 🧠 Skills Demonstrated

- Web scraping with BeautifulSoup  
- Data transformation with pandas and NumPy  
- Currency conversion using external CSV data  
- Structured logging  
- SQL-based data storage and querying  
- Modular Python scripting for automation

## 📂 Project Structure

| Parameter                  | Value                                                                 |
|---------------------------|-----------------------------------------------------------------------|
| Code name                 | `banks_project.py`                                                    |
| Data source               | [Wikipedia Archive](https://web.archive.org/web/20230908091635/https://en.wikipedia.org/wiki/List_of_largest_banks) |
| Exchange rate CSV         | [`exchange_rate.csv`](https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBMSkillsNetwork-PY0221EN-Coursera/labs/v2/exchange_rate.csv) |
| Output CSV path           | `./Largest_banks_data.csv`                                            |
| Database name             | `Banks.db`                                                            |
| Table name                | `Largest_banks`                                                       |
| Log file                  | `code_log.txt`                                                        |

## ⚙️ ETL Workflow

### Task 1: Logging
- `log_progress()` logs each stage of the ETL process to `code_log.txt`.

### Task 2: Extraction
- `extract()` scrapes bank names and market caps from the Wikipedia table.

### Task 3: Transformation
- `transform()` adds market cap columns in GBP, EUR, and INR using exchange rates.

### Task 4: Load to CSV
- `load_to_csv()` saves the transformed data to a local CSV file.

### Task 5: Load to Database
- `load_to_db()` writes the data to a SQLite table.

### Task 6: Querying
- `run_query()` executes SQL queries to analyze the stored data.

### Task 7: Log Verification
- Confirm all stages are logged in `code_log.txt`.

## 🚀 How to Run

```bash
pip install requests pandas beautifulsoup4 numpy
python banks_project.py
```

Ensure `exchange_rate.csv` is in the same directory or update the path accordingly.

