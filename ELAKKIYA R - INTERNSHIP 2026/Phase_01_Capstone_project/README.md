# Netflix Data Engineering Capstone Project

## Project Overview

This project was completed as part of the **CodeBoosters Tech – Phase 1 Capstone Project (Data Engineering Phase)**.

The objective of this project is to perform an end-to-end Data Engineering workflow using the Netflix Movies and TV Shows dataset. The project covers data ingestion, data cleaning, SQL analysis, ETL pipeline implementation, PySpark Medallion Architecture, data visualization, and machine learning.

---

## Dataset

**Dataset Name:** Netflix Movies and TV Shows

**Source:** Kaggle

The dataset contains information about Netflix content, including:

* Show ID
* Type (Movie / TV Show)
* Title
* Director
* Cast
* Country
* Date Added
* Release Year
* Rating
* Duration
* Listed Categories
* Description

---

## Technologies Used

* Python
* Pandas
* NumPy
* SQLite
* SQL
* PySpark
* Matplotlib
* Scikit-Learn
* Jupyter Notebook

---

## Project Workflow

### 1. Data Ingestion

* Loaded CSV dataset using Pandas.
* Explored dataset structure.
* Analyzed columns, shape, data types, and statistics.

### 2. Data Cleaning and Preprocessing

* Handled missing values.
* Removed duplicate records.
* Converted data types.
* Renamed columns for consistency.
* Saved cleaned dataset.

### 3. SQLite Database Integration

* Created SQLite database.
* Loaded cleaned dataset into database.
* Verified successful insertion of records.

### 4. SQL Analysis

Performed SQL operations including:

* Filtering
* Sorting
* Aggregation
* Group By
* Conditional Queries

### 5. SQL-Based Transformation

Created derived business columns such as:

* Content Category
* Release Category

Exported transformed data to CSV.

### 6. ETL Pipeline

Implemented a complete ETL workflow:

#### Extract

Read data from source CSV.

#### Transform

Cleaned and standardized data.

#### Load

Stored processed data into output files.

### 7. PySpark Medallion Architecture

#### Bronze Layer

* Raw Netflix dataset stored as Parquet.

#### Silver Layer

* Cleaned and standardized data.
* Missing values handled.
* Duplicate records removed.

#### Gold Layer

Created business-ready datasets:

* Content Type Analysis
* Rating Analysis
* Country Analysis
* Release Year Analysis

All layers were stored in Parquet format.

### 8. CSV vs Parquet Comparison

Compared both formats based on:

* File Size
* Storage Efficiency
* Read Performance
* Write Performance
* Advantages and Limitations

### 9. Parquet to Pandas Conversion

* Read Parquet files using PySpark.
* Converted data back into Pandas DataFrame.
* Validated successful conversion.

### 10. Data Visualization

Created visualizations including:

* Movies vs TV Shows
* Top Content Ratings
* Release Year Trend
* Rating Distribution

### 11. Machine Learning

Built a classification model using Scikit-Learn.

Steps performed:

* Feature Selection
* Data Encoding
* Train-Test Split
* Model Training
* Prediction
* Performance Evaluation

---

## Project Structure

```text
Codeboosters-Phase1-Capstone-Project/

│
├── Phase1_Capstone_Project.ipynb
├── netflix_titles.csv
├── netflix_cleaned.csv
├── netflix_transformed.csv
├── etl_output.csv
├── netflix.db
│
├── bronze_layer/
├── silver_layer/
├── gold_layer/
│
└── README.md
```

---

## Key Outcomes

* Successfully implemented an end-to-end Data Engineering pipeline.
* Demonstrated SQL analysis and transformation techniques.
* Built a Medallion Architecture using PySpark.
* Compared CSV and Parquet storage formats.
* Generated business insights through visualization.
* Developed and evaluated a machine learning model.

