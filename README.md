 ### Sales dataset and analysis
 This project focuses on cleaning and preparing a messy sales dataset for analysis. The dataset contains inconsistencies such as missing values, incorrect data types, and inconsistent text formatting.
 ### Table of Contents
- [Project Overview](#project-overview)
- [Data Sources](#Data-Sources)
- [Data Description](#Data-Description)  
### Data Sources
Sales Data: The primary dataset is the "sales data.csv" file, containing detailed information about each sales made by the company.
### Dataset Description
- Rows: 150
- Columns include:
- Order ID
- Product Name
- Price
- Quantity
- Payment Method
- Store Location
  ### Issues identified
-	Missing values in Order ID and Quantity columns
-	Price column contains mixed formats (numbers, text with "$", and blanks)
-	Inconsistent payment method entries (e.g., "cash", "Cash", "pos")
-	Inconsistent store locations (e.g., "Lagos", "lagos", "PH", "Abj")
-Incorrect data types across multiple columns
### Data cleaning steps
1. Handling Missing Values: Removed rows with missing Order IDs as values could not be uniquely identified.
- Replaced missing Quantity values with 1 (assumption: minimum purchase)
2. Cleaning Price Column
-	Removed "$" symbols from price values
-	Converted the column to numeric format
-Handled blank values by removing affected rows
3. Standardizing Text Fields
-	Converted all text to proper case
-	Standardized payment methods (e.g., "cash" → "Cash", "pos" → "POS")
-	Standardized store locations (e.g., "lagos" → "Lagos", "PH" → "Port Harcourt")
4. Data Type Corrections
-	Converted Price and Quantity columns to numeric data types
-	Ensured all columns have appropriate formats
5. Feature Creation
-	Created a new column: Total Sales = Price × Quantity
### Tool Used: Excel (for data cleaning and analysis)


