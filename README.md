# online_retail_analyzin

This project is a **data analysis** of the `Online Retail` dataset using **Python**, **Pandas**, **Matplotlib**, and **Seaborn**. The aim is to clean the dataset, perform exploratory data analysis (EDA), and visualize key metrics such as quantity, unit price, and total price.

## 📁 Dataset

The dataset contains ~400,000 records of transactions made by a UK-based online retailer between 2010 and 2011.

Main features:
- `InvoiceNo`: Invoice number (may contain cancellations)
- `StockCode`: Product code
- `Description`: Product description
- `Quantity`: Number of products purchased
- `InvoiceDate`: Date and time of invoice
- `UnitPrice`: Price per product
- `CustomerID`: ID of the customer
- `Country`: Customer's country

---

##  Data Cleaning Steps

✔️ Converted column types (e.g., `InvoiceNo`, `CustomerID`, `InvoiceDate`)  
✔️ Removed rows with:
- Missing or null `CustomerID`
- `Quantity` not in range (0 < Quantity < 1000)
- `UnitPrice` <= 0  
✔️ Filtered `InvoiceDate` to be within a valid date range

---

## 📊 Exploratory Data Analysis (EDA)

We used Pandas, Matplotlib, and Seaborn to analyze key columns:

### ✅ Statistical Metrics

For `Quantity`, `UnitPrice`, and `TotalPrice`, we computed:
- Mean, Median
- Standard Deviation
- Quartiles (Q1, Q2, Q3)
- Interquartile Range (IQR)
- Skewness (to detect asymmetry)

### 📈 Visualizations

We used subplots to compare metrics across multiple columns:

- Histogram + KDE plots
- Box plots and Violin plots
- Outlier detection using IQR
- (Optional) Time series trends by `InvoiceDate`

---

## 🔍 Goals

- Understand data distribution and detect anomalies
- Identify invalid or suspicious transactions
- Prepare the dataset for further machine learning or business analysis

---

## 🛠️ Tools Used

- Python 3.10+
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / VS Code

---

## 📌 How to Run

1. Clone the repository:
```bash
git clone https://github.com/your-username/retail-data-analysis.git
