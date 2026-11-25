# Netflix Data Cleaning and Exploratory Data Analysis

## Project Overview

This project focuses on cleaning, transforming, and exploring the Netflix Titles dataset using Python. The main objective is to identify data quality issues, handle missing and inconsistent values, perform feature engineering, and uncover useful insights through Exploratory Data Analysis (EDA).

The project follows a structured data analytics workflow, starting with raw data inspection and ending with an exported, cleaned dataset.

## Objectives

- Inspect and understand the structure of the dataset.
- Identify missing values and duplicate records.
- Detect and correct inconsistent data entries.
- Standardize data formats and values.
- Perform feature engineering to create meaningful variables.
- Explore content distribution and characteristics.
- Identify patterns and relationships through visualizations.
- Export the final cleaned dataset for further analysis.

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Python | Data analysis and processing |
| Pandas | Data cleaning and manipulation |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive development |

## Dataset Description

The dataset contains information about movies and TV shows available on Netflix.

**Dataset size:**
- Records: 8,807
- Original columns: 12

**Key attributes include:**
- `show_id` – Unique identifier for each title.
- `type` – Movie or TV Show.
- `title` – Title of the content.
- `director` – Director information.
- `cast` – Main cast members.
- `country` – Country of production.
- `date_added` – Date the content was added to Netflix.
- `release_year` – Original release year.
- `rating` – Content rating.
- `duration` – Movie duration or number of seasons.
- `listed_in` – Content genres and categories.
- `description` – Description of the title.

## Project Workflow

### 1. Data Loading and Inspection
- Imported the required Python libraries.
- Loaded the dataset using Pandas.
- Examined dataset dimensions, column names, and data types.
- Generated descriptive statistics.

### 2. Data Quality Assessment
- Checked for missing values.
- Identified duplicate records.
- Inspected inconsistent text formatting.
- Examined invalid and misaligned values.
- Checked date and duration consistency.

### 3. Data Cleaning
- Removed unnecessary whitespace.
- Corrected three records where duration and rating values were misaligned.
- Handled missing categorical values using an `Unknown` label.
- Converted date fields into appropriate datetime formats.
- Retained genuinely missing date values for further analysis.

### 4. Feature Engineering

Created additional features to support deeper analysis:

- `date_added_year` – Year the title was added to Netflix.
- `date_added_month` – Month the title was added.
- `duration_value` – Numerical duration value.
- `duration_unit` – Duration unit (minutes or seasons).
- `primary_genre` – Primary genre extracted from the genre categories.
- `primary_country` – Primary country extracted from the country field.

### 5. Exploratory Data Analysis

Performed univariate and bivariate analysis to investigate:

- Distribution of Movies and TV Shows.
- Content release trends over the years.
- Most common genres.
- Distribution of content ratings.
- Content production by country.
- Movie durations and TV show seasons.
- Relationships between selected numerical variables.

### 6. Inconsistency and Outlier Analysis

- Checked for invalid rating categories.
- Investigated malformed duration values.
- Verified Movie and TV Show duration consistency.
- Checked duplicate show IDs.
- Flagged date inconsistencies for further investigation.
- Applied the Interquartile Range (IQR) method for outlier detection.

### 7. Exporting Cleaned Data

Exported the processed dataset into a CSV file for future analysis and visualization.

## Key Data Quality Findings

| Finding | Result |
|---|---:|
| Original records | 8,807 |
| Exact duplicate records | 0 |
| Rating and duration misalignment | 3 |
| Titles with surrounding whitespace | 1 |
| Date-added values with whitespace | 88 |
| Date-added values earlier than release year | 14 |
| Missing date-added values | 10 |

The 14 date inconsistencies were flagged for review rather than automatically modified.

## Key Outcome

The project demonstrates a complete data cleaning and exploratory analysis workflow using Python. It highlights the importance of data quality assessment, handling inconsistent records, feature engineering, and visual exploration before using datasets for further analytical work.

## Author

Ishaka Dewmini

Data Science | Data Analytics | Python | SQL | Tableau
