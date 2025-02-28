# E-Commerce Data Analysis and EDA

## Project Overview
This project performs exploratory data analysis (EDA) and data cleaning on an e-commerce dataset. The dataset includes online transactions and customer information, and the analysis focuses on customer behavior, order trends, and revenue insights.

## Dataset
Here's a concise update:  

The dataset is sourced from [Kaggle](https://www.kaggle.com/datasets/carrie1/ecommerce-data/data), 
downloaded, and uploaded to Google Drive. The data file is also included in the repository for easy access.
- The dataset is loaded from Google Drive (`data.csv`).
- It includes transaction details such as `CustomerID`, `InvoiceNo`, `InvoiceDate`, `Quantity`, `UnitPrice`, and `Country`.

## Data Cleaning & Transformation
- Handled missing values:
  - Dropped rows with missing `CustomerID`.
  - Replaced missing `Description` values with "no description".
- Converted `CustomerID` to integer format.
- Transformed `InvoiceDate` to DateTime format.
- Created new features:
  - `year_month`: Extracted year and month from `InvoiceDate`.
  - `month`, `day`, and `hour` from `InvoiceDate`.
  - `amount_spent`: Computed as `Quantity * UnitPrice`.
- Saved the cleaned dataset as `clean_data.csv`.

## Exploratory Data Analysis (EDA)
- **General Statistics:**
  - Displayed dataset shape and column details.
  - Analyzed missing values and their percentages.
- **Customer Behavior Analysis:**
  - Plotted the number of orders per `CustomerID`.
  - Identified the top 10 customers by order volume.
- **Geographical Analysis:**
  - Visualized the number of orders from different countries.
- **Time-Based Analysis:**
  - Examined order distribution across months.

## Visualizations
- Line plot: Number of orders per customer.
- Bar plot: Top 10 customers with order count.
- Horizontal bar plot: Number of orders per country.
- Bar chart: Monthly order trends.

## Tools & Libraries
- `pandas`: Data manipulation and analysis
- `matplotlib.pyplot`: Data visualization
- `seaborn`: Advanced data visualization
- `warnings`: Suppressing warnings for cleaner output

## Future Improvements
- Implement advanced customer segmentation (RFM Analysis).
- Analyze revenue trends over time.
- Create a dashboard for interactive data visualization.

