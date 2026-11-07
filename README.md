📊 Product Dataset – Data Cleaning and Preparation Using Microsoft Excel

📌 Project Overview

This project focuses on cleaning and preparing a Product Dataset using Microsoft Excel. The main objective is to improve data quality by handling missing values, correcting inconsistent text formats, removing duplicate records, splitting and merging columns, applying number formatting, and using conditional formatting.

Data cleaning is an essential step in data analysis because incomplete, inconsistent, and duplicated data can lead to inaccurate analysis and misleading results.

This assignment demonstrates practical Excel data cleaning, preprocessing, and standardization techniques used by Data Analysts.

🎯 Project Objectives
Identify and handle missing values.
Correct inconsistent text formats and spelling errors.
Identify and remove duplicate records.
Split and merge columns for better data organization.
Apply appropriate number and date formatting.
Use conditional formatting to highlight important information.
Improve the overall quality, consistency, and readability of the dataset.
📂 Dataset Description

Dataset Name: Product Dataset

Initial Records: 35 rows

Records After Removing Duplicates: 32 rows

Attributes:

Product ID
Product Name
Brand Name
Quantity
Category
Price

Additional Columns Created During Cleaning:

Manufacturing Date
Country Code
Product Name_clean
Product Brand
Price_clean
price_currency
Category_clean
🛠️ Tools and Technologies
Microsoft Excel
Find and Replace
Text to Columns
Remove Duplicates
IF Function
MEDIAN Function
PROPER Function
CONCAT / CONCATENATE
Number Formatting
Conditional Formatting
🧹 Data Cleaning and Preparation Steps
1. Handling Missing Values

Price Column:

Checked the Price column for missing values.
Chose the Median Imputation method to handle missing price values.
Used the MEDIAN function to calculate the median price of the dataset.
Applied the IF and ISBLANK functions to replace missing price values with the calculated median while keeping existing values unchanged.

Excel Formula:

excel
=IF(ISBLANK([@[Price ($)]]),MEDIAN([Price ($)]),[@[Price ($)]])


Explanation:

ISBLANK() checks whether the Price cell is empty.
MEDIAN() calculates the median of the Price column.
IF() replaces missing values with the median and retains existing values.

The cleaned values were stored in the Price_clean column.


2. Correcting Inconsistent Data

Product Name Column:

Identified inconsistent capitalization in the Product Name column.
Used Excel's PROPER function to standardize the text format.
Converted product names into Proper Case to maintain consistency.

Examples:

Original Product Name	Cleaned Product Name
laptop	Laptop
smartphone	Smartphone
Sneakers	Sneakers
Coffee Maker	Coffee Maker
Backpack	Backpack

Category Column:

Checked the Category column for spelling errors and misspellings.
Used Excel's Find and Replace feature to correct typos.
Standardized category names for consistency.
Stored the corrected values in the Category_clean column.
3. Removing Duplicates

Used Excel's built-in Remove Duplicates feature to identify and eliminate duplicate records.

Steps followed:

Selected the complete dataset.
Navigated to the Data tab.
Selected Remove Duplicates.
Selected all columns to check for complete duplicate rows.
Clicked OK to remove duplicate records.

Result:

Description	Number of Rows
Initial Records	35
Duplicate Records Removed	3
Final Records	32

Outcome: Successfully removed 3 duplicate rows, reducing the dataset from 35 rows to 32 unique records.

4. Splitting and Merging Data

Splitting Product ID:

The original Product ID contained manufacturing date information and country codes.

Example:

28-JAN-US

Separated the Product ID into two different columns:

Manufacturing Date: 28-JAN
Country Code: US

This transformation improved the structure and usability of the dataset.

Merging Brand Name and Product Name:

Combined the Brand Name and Product Name columns into a new column named Product Brand.

Example:

Brand Name	Product Name	Product Brand
Dell	Laptop	Dell Laptop
Nike	Sneakers	Nike Sneakers
Keurig	Coffee Maker	Keurig Coffee Maker
Samsung	Smartphone	Samsung Smartphone
North Face	Backpack	North Face Backpack
5. Number Formatting

Price Column:

Applied currency formatting to the Price column.
Standardized the price display using dollar currency format.
Maintained numeric values in the Price_clean column.
Created a price_currency column to display prices in currency format.

Examples:

Original Price	Currency Format
1000	$1,000.00
80	$80.00
130	$130.00
900	$900.00
70	$70.00

Manufacturing Date Column:

Applied date formatting to the Manufacturing Date column.
Used the required date display format: DD-MM-YYYY.
Ensured consistent date presentation.

Note: The original Product ID provides only day and month information. A valid manufacturing year is required to create complete dates in DD-MM-YYYY format.

6. Conditional Formatting

Applied Excel Conditional Formatting to improve data visualization and highlight important information.

Price Column:

Applied Data Bars or Color Scales.
Highlighted differences in product prices.
Made it easier to identify higher-priced and lower-priced products.

Category Column:

Created a custom conditional formatting rule.
Highlighted cells where the category equals Electronics.
Improved category identification and readability.
📊 Final Dataset Structure
Column Name	Description
Product ID	Original product identifier
Manufacturing Date	Extracted manufacturing date
Country Code	Extracted country identifier
Product Name	Original product name
Product Name_clean	Standardized product name
Brand Name	Product brand
Product Brand	Combined brand and product name
Price ($)	Original product price
Price_clean	Price with missing values handled using median
price_currency	Currency-formatted price
Quantity	Available product quantity
Category	Original product category
Category_clean	Standardized category
📈 Key Findings

After performing data cleaning and preparation:

Initial Records: 35
Final Records: 32
Duplicate Records Removed: 3
Missing Price Values: Handled using Median Imputation.
Product Names: Standardized using the PROPER function.
Category Values: Corrected using Find and Replace.
Product ID: Split into Manufacturing Date and Country Code.
Product Brand: Created by merging Brand Name and Product Name.
Price: Standardized using currency formatting.
Conditional Formatting: Applied to Price and Category columns.
💡 Skills Demonstrated

Through this assignment, I practiced the following data analytics skills:

Data Cleaning and Preprocessing
Missing Value Identification and Handling
Median Imputation
Text Standardization using PROPER Function
Find and Replace
Duplicate Data Removal
Text-to-Columns Transformation
Column Merging
Date and Currency Formatting
Conditional Formatting
Excel Data Management
🏁 Conclusion

This project demonstrates how Microsoft Excel can be used to clean, organize, and transform raw product data into a structured and analysis-ready dataset.

By applying median imputation to handle missing price values, standardizing product names using the PROPER function, correcting category errors through Find and Replace, and removing duplicate records, the overall quality and consistency of the dataset were improved.

Additionally, splitting and merging columns, applying number formatting, and using conditional formatting helped improve the dataset's structure, readability, and usability.

These data cleaning techniques provide a strong foundation for further data analysis, reporting, and visualization.

Project Title: Product Dataset – Data Cleaning and Preparation
Project Type: Data Cleaning and Data Preprocessing
Tool Used: Microsoft Excel
Domain: Data Analytics
Status: Completed ✅

Author: Gomathy Pandurangan
