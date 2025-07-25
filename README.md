# 📈 Sales Forecasting and Business Insights Using SQL, Prophet & Linear Regression

## 📊 Overview
This project focuses on analyzing retail sales data to extract meaningful business insights and forecast future sales trends. It combines powerful SQL queries for data exploration, **Linear Regression** for baseline trend modeling, and **Facebook Prophet** for advanced time series forecasting.

---

## 🛠️ Tech Stack
- **SQL (MySQL)** – for data exploration and aggregation
- **Python (Pandas, Scikit-learn, Prophet)** – for preprocessing and modeling
- **Facebook Prophet** – for time series forecasting
- **Linear Regression** – for trend-based prediction
- **Jupyter Notebook** – for code and visualization

---

## 📁 Dataset Description
The dataset contains transactional sales records with the following key columns:
- `Order Date`, `Ship Date`
- `Customer ID`, `Customer Name`, `Segment`
- `Region`, `State`, `City`
- `Product ID`, `Product Name`, `Category`, `Sub-Category`
- `Sales`, `Ship Mode`

---

## ⚙️ Features / SQL Insights
A variety of SQL queries were used to analyze the dataset, including:
- 🧮 **Total Sales by Region, State, and Category**
- 👥 **Top Customers and Products by Revenue**
- 📅 **Monthly Sales Trends using `DATE_FORMAT`**
- 🚚 **Average Shipping Delay using `DATEDIFF`**
- 🏷️ **Customer Purchase Patterns (Weekday vs. Weekend Orders)**
- 🏅 **First Order Analysis using `ROW_NUMBER()`**
- 🔢 **Ranking Customers by Sales using `RANK()`**
- 🧾 **Customer-wise Product List using `GROUP_CONCAT()`**

---

## 🔮 Forecasting Models

### 📌 Linear Regression
- Aggregated monthly sales used as input
- Applied **scikit-learn’s LinearRegression** to model the trend
- Used as a baseline model for comparison

### 📌 Facebook Prophet
- Data formatted with `ds` and `y` columns
- Captured **seasonality** and **trends**
- Provided forecasts with **confidence intervals**
- Plotted forecast and component trends (yearly, weekly)

---

## 📉 Results & Visualizations
- 📈 **Linear Regression Forecast:** Straight-line projection of monthly sales trend
- 🔮 **Prophet Forecast:** Advanced prediction with seasonal patterns
- 📊 SQL summaries of top customers, products, regions, and monthly sales
- 🗓️ Visualizations of shipping delays and order timing

---

## 🧠 Key Insights
- **West region** had the highest total sales
- **Phones** and **Tables** were the top-performing sub-categories
- **Brosina Hoffman** was the highest-spending customer
- Most orders were placed on **weekdays**
- Average shipping delay: **4.25 days**
- Prophet detected **December and September** as peak sales months

---

## 🚀 How to Run
1. Clone the repository or download the notebook and SQL file.
2. Load the sales dataset into a MySQL database (`train` table).
3. Run SQL queries using any MySQL client.
4. Open the Jupyter Notebook `SALES FORCASTING-prophet.ipynb`.
5. Install dependencies:
   ```bash
   pip install pandas scikit-learn prophet matplotlib
