**Data Cleaning Procedures - README**
**Introduction**
This document provides a comprehensive overview of the data cleaning methodologies applied to the customer, product, region, and transaction datasets. The cleaning process was carried out using Power BI's Power Query Editor to ensure data integrity and uniformity across all datasets.

Datasets Included:
Customer Data
Product Data
Region Data
Transaction Data
**1. Customer Data Cleaning Steps**
Key Columns: CustomerID, Email, Phone, City, State, Country, Gender, Age, Join Date, Last Purchase, Total Spent, Loyalty Points, Purchase Frequency, Customer Segment, Preferred Payment, Marital Status, Account Creation, Account Status, Last Modified, Referrer ID, Feedback Score, Email Domain, Country Code.

Cleaning Steps:
Data Import: Imported the dataset into Power BI using the Text/CSV option under Get Data.
Invalid Email Filtering: Eliminated entries with incorrect email domains.
Phone Number Formatting: Standardized phone numbers to a consistent format (e.g., +1-123-456-7890).
Missing Value Treatment: Addressed missing data through logical filling or imputation.
Data Type Verification: Confirmed and adjusted data types for all columns (e.g., Date, Number, Text).
Email Domain Extraction: Created a new column to capture the domain of email addresses.
Derived Columns Creation: Developed classifications based on metrics like Total Spent and Loyalty Points.
Date Formatting Consistency: Ensured all dates were formatted uniformly.
Country Code Standardization: Ensured all country codes followed a consistent format.
**2. Product Data Cleaning Steps**
Key Columns: ProductID, Product Name, Category, Price, Stock Status, Supplier, Updated Price, Stock Status Update, Last Modified, Discontinued Status.

Cleaning Steps:
Duplicate Removal: Checked for and removed duplicate entries based on ProductID.
Missing Value Imputation: Addressed gaps in Price and Stock Status with appropriate values.
Price Format Standardization: Ensured all prices were uniformly formatted (e.g., $100.00).
Data Type Adjustment: Confirmed that Price is treated as a number and Product Name as text.
Discontinued Products Update: Marked products that are no longer available.
**3. Region Data Cleaning Steps**
Key Columns: RegionID, Region Name, Country, State, Updated Region Name, Last Modified, Country Code.

Cleaning Steps:
Invalid Region Removal: Filtered out any entries with incomplete or invalid region names.
Country Code Standardization: Ensured consistent formatting of country codes (e.g., +1 for the USA).
Missing Data Handling: Used fill-down techniques to address missing region or country information.
Data Type Correction: Made sure Region Name is text and Country Code is numerical.
**4. Transaction Data Cleaning Steps**
Key Columns: TransactionID, CustomerID, ProductID, Transaction Date, Quantity, Total Amount, Payment Method, Discount Applied, Last Modified.

Cleaning Steps:
Duplicate Transaction Removal: Ensured each TransactionID is unique, eliminating any duplicates.
Missing Data Handling: Addressed gaps in Quantity and Total Amount with appropriate values.
Data Type Adjustment: Applied correct data types, ensuring Transaction Date is in date format and Total Amount is numerical.
Payment Method Standardization: Ensured uniformity in the Payment Method field (e.g., Credit Card, PayPal).
Discount Verification: Checked for consistent values in the Discount Applied column.
**Conclusion**
The cleaning and standardization of the datasets have been successfully completed. Each dataset is now accurate, well-structured, and ready for analysis and reporting within Power BI.

