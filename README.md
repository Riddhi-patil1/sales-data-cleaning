Sales Data Cleaning and Preprocessing using Python

## 📌 Project Overview
This project focuses on **cleaning and preprocessing a real-world sales dataset** using **Python** and **Pandas**.  
The dataset intentionally contains common data quality issues such as missing values, inconsistent formats, duplicates, and invalid entries.

The goal of this project is to transform **raw, messy data into clean, reliable data** that is ready for analysis and visualization.

---

## 📂 Project Structure
sales-data-cleaning/ │

                     ├── sales_dirty_data.csv      # Raw (uncleaned) dataset
                    
                     ├── sales_cleaned_data.csv    # Cleaned dataset after preprocessing 
                     
                     ├── sale.ipynb                # Jupyter Notebook with cleaning steps 
                     
                     ├── panda.py                  # (Optional) Python script version
                     
                     └── README.md                 # Project documentation


---

## 📊 Dataset Description

The dataset contains sales transaction records with the following columns:

| Column Name     | Description |
|-----------------|-------------|
| Order_ID        | Unique order identifier |
| Order_Date      | Date of order |
| Customer_Name   | Name of the customer |
| Product         | Product purchased |
| Category        | Product category |
| Quantity        | Number of items purchased |
| Price           | Price per unit |
| Total_Amount    | Total transaction value |
| Payment_Mode    | Payment method used |
| City            | City of the customer |

The raw dataset includes **inconsistent formats and missing values** to simulate real-world data.

---

## 🚩 Data Quality Issues Identified

The following issues were found in the raw dataset:

- Missing values in multiple columns
- Mixed date formats causing parsing errors (`NaT`)
- Duplicate records
- Inconsistent text values (e.g., `Card`, `card`, `CASH`)
- Invalid numeric values (negative quantity and amount)
- Inconsistent product naming
- Incorrect or missing total amounts

---

## 🛠️ Data Cleaning Steps Performed

The following preprocessing steps were applied:

1. Loaded data using Pandas
2. Inspected structure using `df.info()` and `df.describe()`
3. Identified missing values
4. Standardized and parsed date formats safely
5. Handled missing values using logical defaults
6. Fixed inconsistent categorical values
7. Removed invalid rows (negative quantities)
8. Recalculated `Total_Amount` using `Quantity × Price`
9. Removed duplicate records
10. Verified cleaned data integrity

---

## ✅ Final Output

- All critical columns have valid values
- Dates are correctly parsed as `datetime`
- Numeric columns contain valid numbers
- Categorical values are standardized
- Dataset is ready for **EDA and visualization**

The cleaned dataset is saved as:
sales_cleaned_data.csv
Copy code

---

## 🛠️ Tools & Technologies Used

- Python
- Pandas
- Jupyter Notebook / VS Code

---

## 🎯 Learning Outcomes

Through this project, I learned:

- How to identify real-world data quality issues
- Proper handling of missing and invalid data
- Safe date parsing and validation
- Best practices to avoid `SettingWithCopyWarning`
- Structuring a professional data cleaning workflow

---

## 👤 Author

**Riddhi**  

---
## 📌 Note
This project is created for learning and practice purposes and demonstrates real-world data cleaning techniques.