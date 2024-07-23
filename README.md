# Data Cleaning Project: Layoffs Data

This project involves cleaning a dataset containing information about layoffs from companies around the world. The cleaning process includes removing duplicates, standardizing data, handling null or blank values, and removing unnecessary columns.

## Table of Contents

- [Data Description](#data-description)
- [Data Cleaning Steps](#data-cleaning-steps)
  - [Step 1: Remove Duplicates](#step-1-remove-duplicates)
  - [Step 2: Standardize Data](#step-2-standardize-data)
  - [Step 3: Handle NULL or Blank Values](#step-3-handle-null-or-blank-values)
  - [Step 4: Remove Unnecessary Columns](#step-4-remove-unnecessary-columns)

## Data Description

The dataset contains information about layoffs from various companies, including details such as the company name, location, industry, total number of layoffs, percentage of layoffs, date, stage, country, and funds raised in millions.

## Data Cleaning Steps

### Step 1: Remove Duplicates

We identify and remove duplicate records based on multiple columns (company, location, industry, total_laid_off, percentage_laid_off, date, stage, country, funds_raised_millions) by using a `row_number()` window function.

### Step 2: Standardize Data

Standardizing data involves converting date formats to a consistent format and ensuring all text fields are in the same case (e.g., all lowercase or all uppercase).

### Step 3: Handle NULL or Blank Values

Handling NULL or blank values involves filling them with appropriate default values or removing records where necessary.

### Step 4: Remove Unnecessary Columns

Remove columns that are not relevant to the analysis and do not affect other processes. Care should be taken to ensure these columns are not used elsewhere in the project.
