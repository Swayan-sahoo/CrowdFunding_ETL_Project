# CrowdFunding_ETL_Project
Crowdfunding ETL/Database Project

# 📌Project Overview

This project focuses on designing and implementing a relational PostgreSQL database for managing crowdfunding campaign data. The goal is to transform raw crowdfunding data into a normalized, query-ready database that supports efficient reporting and analysis.

The project demonstrates key data engineering and analytics skills, including data transformation, schema design, SQL database creation, and data validation.

# 🛠️ Technologies Used

Python (Pandas)

PostgreSQL

SQL

QuickDBD (ERD design)

CSV files

GitHub

# 📂 Project Structure
crowdfunding-database-project/
│
├── Resources/
│   ├── category.csv
│   ├── subcategory.csv
│   ├── campaign.csv
│   └── contacts.csv
│
├── crowdfunding_db_schema.sql
├── data_transformation.ipynb
├── ERD.png
└── README.md

# 🔄 Data Extraction & Transformation

The original crowdfunding dataset was cleaned and transformed using Python and Pandas.

Category & Subcategory Tables

Identified unique categories and subcategories.

Generated sequential IDs:

category_id → cat1, cat2, ...

subcategory_id → subcat1, subcat2, ...

Exported cleaned data to:

category.csv

subcategory.csv

Campaign Table

Extracted relevant campaign attributes including:

Campaign details, financial goals, backer counts, country, currency, and dates.

Renamed columns for readability:

blurb → description

launched_at → launch_date

Converted data types:

Financial fields → FLOAT

Dates → DATETIME

Added foreign keys:

category_id

subcategory_id

Exported final dataset to campaign.csv.

Contacts Table

Transformed contact data by:

Converting rows to dictionaries

Splitting full names into first_name and last_name

Exported cleaned data to contacts.csv.

# 🧱 Database Design

An Entity Relationship Diagram (ERD) was created using QuickDBD to model the database structure.

Tables Included

category

subcategory

campaign

contacts

Design Features

Clearly defined primary keys

Proper foreign key relationships

Data integrity constraints such as:

NOT NULL

UNIQUE

The complete schema is stored in:

crowdfunding_db_schema.sql

# 🗄️ Database Creation & Data Loading

Created a PostgreSQL database named:

crowdfunding_db


Executed the schema file to create tables in the correct order.

Imported CSV files into PostgreSQL:

category.csv

subcategory.csv

campaign.csv

contacts.csv

Validated successful imports using SELECT queries.

# ✅ Key Skills Demonstrated

Data cleaning and transformation (ETL)

Relational database design

SQL schema creation

Foreign key relationships

Data validation and quality checks

Documentation and reproducibility

# 📈 Future Enhancements

Add analytical SQL queries for insights

Create dashboards using Power BI or Tableau

Implement a Flask API for data access

Add automated data validation checks

# 👤 Author

Swayansiddha Sahoo
\Haanah Candido
(Data Analyst)
