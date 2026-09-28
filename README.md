# Sales Data Exploratory Data Analysis

## 📌 Project Overview

This project performs Exploratory Data Analysis (EDA) on a sales dataset containing 500 orders.

The main goal is to understand sales patterns, product performance, regional performance, salesperson performance, monthly trends, outliers, and the relationship between quantity sold and sales amount.

---

## 📊 Dataset

The dataset contains **500 rows and 7 original columns**:

* `Order_ID` — Unique order identifier
* `Order_Date` — Date of the order
* `Product` — Product purchased
* `Region` — Sales region
* `Salesperson` — Person responsible for the sale
* `Quantity` — Quantity sold
* `Sales_Amount` — Total sales amount

During EDA, additional analytical columns such as `Year`, `Month`, and `Sales_Category` were created.

---

## 🎯 Objectives

The main objectives of this project were:

* Understand the structure of the sales dataset
* Check data quality
* Identify missing and duplicate values
* Perform statistical analysis
* Analyze product performance
* Analyze regional performance
* Analyze salesperson performance
* Identify monthly sales trends
* Detect outliers
* Analyze correlation between quantity and sales
* Generate meaningful business insights

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🔍 EDA Process

### 1. Data Loading

Loaded the CSV dataset using Pandas.

### 2. Dataset Understanding

Analyzed:

* First and last records
* Dataset shape
* Column names
* Data types
* Statistical summary

### 3. Data Quality Analysis

Checked:

* Missing values
* Duplicate rows
* Unique values
* Categorical value distributions
* Invalid/negative values

### 4. Data Cleaning

Performed necessary datatype conversion and date processing.

`Order_Date` was converted to datetime format.

### 5. Univariate Analysis

Analyzed individual variables using:

* Mean
* Median
* Mode
* Minimum
* Maximum
* Range
* Variance
* Standard deviation
* Quartiles
* Percentiles
* IQR

### 6. Data Visualization

Created:

* Bar charts
* Histograms
* Boxplots
* Scatter plots
* Line charts
* Correlation heatmap

### 7. Bivariate Analysis

Analyzed relationships between:

* Product and Sales Amount
* Region and Sales Amount
* Salesperson and Sales Amount
* Quantity and Sales Amount
* Product and Quantity

### 8. Time-Based Analysis

Extracted year and month from `Order_Date` and analyzed monthly sales trends.

### 9. Outlier Analysis

Used the **IQR method** to identify unusual Sales Amount observations.

### 10. Correlation Analysis

Analyzed the relationship between `Quantity` and `Sales_Amount` using Pearson correlation.

### 11. Advanced EDA

Performed:

* GroupBy analysis
* Multiple aggregations
* Pivot tables
* Ranking
* Percentage contribution
* Sales category analysis
* Region-level business summary

---

## 📈 Key Business Insights

| Metric                        |      Result |
| ----------------------------- | ----------: |
| Total Sales                   | ₹63,018,907 |
| Total Orders                  |         500 |
| Total Quantity Sold           |       2,826 |
| Average Order Value           | ₹126,037.81 |
| Top Product                   |      Laptop |
| Top Region                    |        East |
| Top Salesperson               |        Ravi |
| Highest Sales Month           |   September |
| Quantity vs Sales Correlation |       0.447 |
| Sales Amount Outliers         |          23 |
| Quantity Outliers             |           0 |

### Important Findings

* The dataset generated total sales of **₹63,018,907** across 500 orders.
* The average order value was approximately **₹126,037.81**.
* **Laptop** was the highest-performing product based on total sales.
* **East** was the region with the highest total sales.
* **Ravi** generated the highest total sales among the salespersons.
* **September** recorded the highest monthly sales.
* The correlation between Quantity and Sales Amount was approximately **0.447**, indicating a moderate positive linear relationship.
* **23 high-value Sales Amount observations** were identified using the IQR method.
* No quantity outliers were detected.

---

## 📦 Outlier Analysis

The IQR method was used for Sales Amount:

* Q1 = ₹22,222
* Q3 = ₹185,099.75
* IQR = ₹162,877.75
* Lower Limit = -₹222,094.625
* Upper Limit = ₹429,416.375

Values above the upper limit were identified as potential high-value outliers.

A total of **23 Sales Amount observations** were identified.

These observations were not automatically removed because high-value sales can represent genuine business transactions.

---

## 📊 Correlation Analysis

The Pearson correlation between Quantity and Sales Amount was:

**0.4468**

This indicates a **moderate positive linear relationship** between quantity sold and sales amount.

However, correlation does not imply causation.

---

## 🏁 Conclusion

The EDA identified important sales patterns across products, regions, salespersons, and months.

Laptop was the top-performing product, East was the highest-performing region, Ravi generated the highest total sales among salespersons, and September recorded the highest monthly sales.

The analysis also identified 23 high-value Sales Amount observations and found a moderate positive relationship between Quantity and Sales Amount.

This project demonstrates practical skills in **Python, Pandas, data cleaning, statistical analysis, visualization, EDA, outlier detection, correlation analysis, and business insight generation**.

---

## 📁 Project Structure

```text
sales-data-eda/
│
├── sales_data_500_rows.csv
├── Sales_EDA.ipynb
├── README.md
└── requirements.txt
```

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
```

### 2. Install required libraries

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Open Jupyter Notebook

```bash
jupyter notebook
```

### 4. Open

```text
Sales_EDA.ipynb
```

Run the notebook cells sequentially to reproduce the analysis.
