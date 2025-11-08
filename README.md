# 🛒 Amazon Sales Analysis Dashboard


## 📌 Project Objective
The main objective of this project is to analyze **Amazon sales performance** to gain insights into:

- 📈 Total sales and order trends over time  
- 🏆 Best performing states, categories, and fulfillment methods  
- 📦 Order status distribution (Delivered, Cancelled, Returned)  
- 💰 Overall business KPIs (Total Sales, Total Orders, Average Order Value)

---

## 📂 Data Source
The dataset used in this project was collected from **Amazon Seller Records**, provided for analysis during internship at **Innobyte Services**.  
It includes details such as **Order ID, Fulfilment Method, Category, Quantity, Courier Status, and Amount**.

---

## 🧹 Data Cleaning & Preparation (Python)
Performed in **Jupyter Notebook** using **Pandas** and **NumPy**:

- 🧾 Removed unnecessary columns (`New`, `PendingS`)  
- 🔄 Handled missing values in columns like `Fulfilment`, `fulfilled-by`, `Courier Status`, `Category`, and `Size` using **'Unknown'**  
- 🔢 Filled missing numeric values (`Amount`, `Qty`) with **0**  
- ⏱️ Converted data types (e.g., `Date → datetime`, `Amount → numeric`)  
- 🧑‍💻 Standardized text fields for consistency  
- ✅ Verified data quality after cleaning using `df.isnull().sum()`

📘 **Notebook and cleaned dataset are published on GitHub.**

---

## 📊 Data Modeling (Power BI)
A **simple star schema** model was designed with:

- **Fact Table →** Amazon Sales (contains `Amount`, `Qty`, `Status`, `Date`)  
- **Dimension Tables →** Category, Fulfilment, Location (State, City)  

Relationships were built logically between categorical dimensions and sales data for accurate aggregation and filtering.

---

## 📈 Dashboard Features

### 🧮 KPIs:
- 💰 Total Sales (₹)  
- 🧾 Total Orders  
- 📊 Average Order Value (AOV)  
- ❌ Cancelled Orders  

### 📊 Visuals Used:
- 📆 **Line Chart:** Daily Sales Trend Over Time  
- 🗺️ **Map:** Sales Distribution by State  
- 🛍️ **Bar Chart:** Sales by Category  
- 🚚 **Pie Chart:** Fulfilment Method Distribution (Easy Ship vs Merchant)  
- 📦 **Column Chart:** Top Selling Categories  
- 🔍 **Card Visuals:** Total Orders, Total Sales, Average Order Value  

### 🎚️ Filters / Slicers:
- Date  
- State  
- Category  
- Fulfilment Method  

---

## 🔑 Key Business Insights

- 💰 **Total Sales crossed ₹2.5 lakh** with over **500+ orders**.  
- 📍 **Maharashtra** recorded the highest number of orders.  
- 🚀 **Amazon Easy Ship** performed better than **Merchant Fulfilment**.  
- 👕 **Fashion** and **Electronics** were the top performing categories.  
- ⚠️ A few orders were cancelled — indicating areas to improve stock and delivery time.

---

## 💡 Recommendations

1. 📢 Focus on marketing and offers in top-performing states.  
2. 🚚 Use **Easy Ship** for faster and more reliable delivery.  
3. 🔁 Track and reduce **order cancellations** by optimizing inventory.  
4. 🏬 Maintain **ready stock** for high-demand categories.

---

## 🚀 Tools & Skills Demonstrated

| Tool / Skill | Purpose |
|---------------|----------|
| 🐍 **Python (Pandas, Matplotlib)** | Data Cleaning & Analysis |
| 📊 **Power BI** | Dashboard Design & Visualization |
| 🧮 **DAX Measures** | KPI Calculations |
| 🧱 **Data Modeling** | Relationship Building (Star Schema) |
| 💬 **Business Insights Communication** | Interpreting & Presenting Results |


