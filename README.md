# Nashville Housing Data Cleaning
## Overview
This SQL script is designed to clean and preprocess the Nashville Housing data stored in the PortfolioProject database. The cleaning process involves standardizing date formats, populating missing property addresses, breaking down addresses into individual components, changing values in certain fields, removing duplicates, and deleting unused columns.

## Instructions
To use this script, follow these steps:

1. Review the Code: Carefully examine the SQL queries provided in the script.
2. Connect to Database: Ensure you are connected to the appropriate database where the Nashville Housing data is stored.
3. Execute Queries: Execute each query in sequence to clean and preprocess the data.
4. Verify Results: After executing each query, verify the results to ensure the data is cleaned as expected.
5. Adjust as Needed: Depending on your specific requirements and the structure of the data, you may need to adjust certain queries or add additional cleaning steps.
## Script Details
### Standardize Date Format
* Converts the SaleDate column to a standardized date format.
### Populate Property Address Data
* Populates missing property addresses by matching ParcelIDs with non-null addresses.
### Break Out Address into Individual Columns
* Splits the PropertyAddress column into Address and City columns.
### Split Owner Address
* Splits the OwnerAddress column into Address, City, and State columns.
### Change "Sold as Vacant" Field Values
* Changes values in the SoldAsVacant column from 'Y' and 'N' to 'Yes' and 'No' respectively.
### Remove Duplicates
* Identifies and removes duplicate records based on certain columns while keeping one instance of each unique record.
### Delete Unused Columns
* Drops columns that are no longer needed for analysis or reporting.
## Notes
* This script assumes a certain structure and format of the Nashville Housing data. Make sure to adjust the queries accordingly if the data schema differs.
* Always back up your data before performing any data cleaning operations, especially when removing duplicates or dropping columns.
