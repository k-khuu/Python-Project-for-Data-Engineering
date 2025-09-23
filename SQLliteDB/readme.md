# 🧪 STAFF Database Lab – CSV to SQL with Python

## Overview

This repository contains a hands-on lab project focused on foundational database operations using Python. The goal is to demonstrate how structured data from a CSV file can be loaded into a relational database and queried efficiently—all within a Python workflow.

---

## 🧠 Objectives

In this lab, you'll learn how to:

1. ✅ Create a SQLite database using Python  
2. ✅ Load data from a CSV file into a database table  
3. ✅ Run basic SQL queries to retrieve meaningful insights

---

## 📘 Scenario

You're working as a Data Engineer supporting an HR team. They’ve provided a CSV file containing employee records, and your task is to:

- Create a database named `STAFF`  
- Load the CSV data into a table called `INSTRUCTORS`  
- Run queries to access and analyze the data

---

## 📄 Dataset Description

The CSV file contains the following columns:

| Column | Description         |
|--------|---------------------|
| ID     | Employee ID         |
| FNAME  | First Name          |
| LNAME  | Last Name           |
| CITY   | City name           |
| CCODE  | Country code (2-letter ISO) |

---

## 🛠️ Technologies Used

- Python 3.x  
- SQLite3  
- Pandas (optional for CSV handling)  
- CSV module

---

## 📂 Repository Structure

```
├── staff_lab.py            # Main script for database creation and querying
├── instructors.csv         # Sample input data
├── README.md               # Project documentation
```

---

## 🚀 How to Run

1. Clone the repository  
2. Ensure Python 3 is installed  
3. Run the script:
   ```bash
   python staff_lab.py
   ```

---

## 📌 Notes

- This lab is ideal for beginners exploring database integration in Python.  
- You can extend the project by adding CRUD operations, joins, or integrating with Flask for a web interface.


