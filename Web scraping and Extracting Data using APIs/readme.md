# 🎬 Top 50 Films Web Scraping Project

## Overview

This repository contains a hands-on lab project focused on web scraping and data extraction using Python. The goal is to extract information about the **Top 50 Most Highly-Ranked Films** from a curated list based on five major sources: Rotten Tomatoes, IMDb, AFI, Empire, and Sight & Sound.

The project demonstrates how to:
- Analyze HTML structure
- Extract structured data using `requests` and `BeautifulSoup`
- Save the data to both a CSV file and a SQLite database

---

## 🔗 Data Source

The film rankings are sourced from the archived webpage:  
[100 Most Highly-Ranked Films](https://web.archive.org/web/20230902185655/https://en.everybodywiki.com/100_Most_Highly-Ranked_Films)

This list aggregates rankings from multiple expert and crowd-sourced sources to produce a composite score.

---

## 🧠 Objectives

- Use `requests` and `BeautifulSoup` to extract data from a webpage  
- Parse and analyze HTML to locate relevant movie information  
- Save the extracted data to:
  - A CSV file: `top_50_films.csv`
  - A SQLite database: `Movies.db` (table: `top_50`)

---

## 📄 Extracted Attributes

Each movie record includes:

| Attribute | Description              |
|----------|--------------------------|
| Rank     | Position in the top 50   |
| Film     | Movie title              |
| Year     | Year of release          |
| Average  | Average rank across sources (optional)

---

## 📂 Repository Structure

```
├── webscraping_movies.py       # Main script for scraping and saving data
├── top_50_films.csv            # Output CSV file
├── Movies.db                   # SQLite database
├── README.md                   # Project documentation
```

---

## 🚀 How to Run

1. Clone the repository  
2. Install dependencies:
   ```bash
   pip install requests beautifulsoup4 pandas
   ```
3. Run the script:
   ```bash
   python webscraping_movies.py
   ```

---

## 🧪 Success Criteria

- The CSV and database should contain the top 50 films with correct rank, title, and year.
- The database table `top_50` should be queryable for further analysis.

---

## 📌 Notes

- This project is designed for educational purposes and demonstrates core web scraping techniques.
- You can extend it by adding genre classification, visualizations, or API integration for live updates.

---
