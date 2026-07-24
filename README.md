# Text-To-SQL Employee Data Query System

This project is a desktop application designed to let users search employee data using plain English rather than writing SQL code. Users can type questions like "Show attendance of John last week," and the system automatically converts the text into database queries.

## 🎯 Problem Statement & Solution
* Employees and managers need to check attendance, leaves, duties, and employee information daily.
* Manual query writing is slow, error-prone, and most users do not know SQL programming, which creates an unnecessary burden of simple data requests for the IT department.
* Our solution allows users to type questions in natural language.
* The system understands what information is needed and automatically creates correct SQL queries.
* Results are displayed in easy-to-read tables with no technical knowledge required.

## ⚙️ Technology Stack
* **Python**: Main programming language.
* **PyQt5**: Desktop application interface.
* **SQLAlchemy**: Connects to the SQL Server database.
* **Pandas**: Handles and displays data results.
* **SQL Server**: Stores all employee data.
* **Regular Expressions**: Finds patterns in user questions.

## 💻 System Requirements
* Windows 10/11 operating system.
* Python 3.8 or higher installed.
* SQL Server 2019 or higher running.
* `AttDB` database with employee tables.
* Works offline without requiring internet access.

> **Database Connection Note**: The system utilizes a simple connection string via Windows Authentication (`mssql+pyodbc://@./AttDB?driver=SQL+Server`), meaning no username or password is required.

## 🚀 Features
* **Smart Natural Language Search**: Ask questions regarding attendance, absences, leaves, and duties.
* **Flexible Criteria**: Search by full or partial employee name, ID, department, date range, or multiple combined conditions.
* **Intuitive Results**: View clean table formats, sort by clicking column headers, track total record counts, and copy data seamlessly.
* **Robust Error Handling**: Displays friendly error messages, maintains database connections, prevents application crashes, and validates user input.
* **Performance Optimized**: Ensures fast response times and uses threaded execution to keep the user interface responsive during queries.

## 👥 Team & Module Distribution
This project was developed for the Machine Learning course (Term: Fall 2025, Class: BSE-5 B) at Bahria University, Karachi Campus.

* **Muhammad Taha (NLP Logic)**: Handled text understanding, pattern matching, query type detection, and date extraction.
* **Usama Bin Tariq (Database Expert)**: Handled the SQL Server connection, query building, thread management, and error handling.
* **Ali Hassan (Interface Designer)**: Created the application GUI, managed user experience, results display, and testing.

## 🔗 Repository Link
The complete source code is available on the GitHub repository: https://github.com/Tahawebs/Text-To-Sql-agent
