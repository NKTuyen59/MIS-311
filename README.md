# MIS-311
# 🛒 Supermarket Sales Analysis
## 📊 1. Data Overview
The dataset used in this analysis is *The Supermarket Sales dataset*, which contains detailed transaction records from different supermarket branches across three major U.S. cities.  Each record represents one sale transaction, capturing information about the branch, customer type, products sold, and total revenue.

**Dataset Information:**
- Dataset Name: Supermartket Sales  
- File name: `supermarket_sales.xlsx`  
- Number of rows: 253  
- Number of columns: 8  

**Dataset Features:**

| Column | Description |
|--------|--------------|
| sale_id | Unique identifier for each sale transaction |
| branch | Brand of the supermarket |
| city | City in which the branch is located |
| customer_type | Member / Normal |
| product_name | Name of the product sold |
| product_category | Product category |
| quantity | Number of items purchased |
| total_price | Total sales value (USD) |

**Context:**  
The purpose of this dataset is to analyze supermarket sales performance across branches, customer types, and product categories. The goal is to identify sales trends and **customer behavior patterns** to support data-driven marketing and inventory decisions.


## 🧹 2. Data Cleaning

**Missing Values and Duplicate Rows**

| Column | Missing Values | Duplicate Rows |
|--------|----------------|----------------|
| customer_type | 3 |  |
| product_category | 6 |  |
| quantity | 3 |  |
| sale_id |  | 3 |

**Action Taken**
- Rows with missing `customer_type` and `product_category` were removed (<5% data loss).  
- Missing `quantity` values were imputed with the **median** (**11**) using Excel’s `=MEDIAN()` function.  
- Duplicate rows (3 total) were removed using Excel’s *Remove Duplicates* tool.  

👉 **Result:** After cleaning, the dataset is now complete, accurate, and ready for analysis. These steps ensure the data’s reliability for both descriptive and inferential analysis.


## 📈 3. Descriptive Statistics
After data cleaning, the key metrics were summarized to describe the dataset’s overall characteristics.

**Key Metrics**

| Statistic | Quantity | Total Price (USD) |
|------------|-----------|-------------------|
| Mean | 10.78 | 126.32 |
| Median | 11 | 103.89 |
| Min | 1 | 2.18 |
| Max | 20 | 427.14 |

**Dataset Summary:**
- Number of rows: 241  
- Number of columns: 8  


### 🔍 Insight 1: Members Spend More per Transaction

**Table 1:**  
<img width="822" height="242" alt="image" src="https://github.com/user-attachments/assets/1aed18f8-c6f1-4d43-b15c-18b872c0824b" />

**Chart 1:** 
<img width="974" height="558" alt="image" src="https://github.com/user-attachments/assets/4c89c0a5-3ecb-4f43-84e4-7ef4c78eff10" />

- Based on descriptive statistics from the dataset, members have a higher average spending per transaction (≈ USD 138) compared to normal customers (≈ USD 113).
- This demonstrates that the membership program encourages customers to spend more, likely due to loyalty benefits or promotional offers.

➡️ **Implication:** The supermarket should continue enhancing its loyalty program to increase customer retention and overall revenue growth.



### 🔍 Insight 2: Members Purchase More Items and Shop More Frequently

**Table 2:**  
<img width="960" height="563" alt="image" src="https://github.com/user-attachments/assets/2d01751b-03c1-4de9-8c0f-4e6bf50d3a56" />

**Chart 2:**  
<img width="974" height="569" alt="image" src="https://github.com/user-attachments/assets/9ef58666-0e1d-47d1-9c3e-18d5d52fa5b8" />

- From the descriptive statistics of customer purchase quantity, it is observed that members made 128 transactions compared to 113 from normal customers.
- In both branches, members tend to purchase higher quantities per transaction, particularly in the 16–20 item range.

➡️ **Implication:** This indicates that the membership program effectively promotes repeat purchases and higher spending per visit, highlighting its importance in driving sales performance.


## 📝 Summary

The analysis reveals that *member customers* not only spend more per transaction but also buy in larger quantities and more frequently.  
This insight highlights the strategic value of maintaining and expanding the **membership program** to sustain sales growth and customer loyalty.
