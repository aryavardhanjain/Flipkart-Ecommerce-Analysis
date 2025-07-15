# 📦 Flipkart E-Commerce Product Analysis

This project involves exploratory data analysis (EDA) on a dataset of ~20,000 Flipkart product listings. The goal is to uncover insights related to product pricing, discounts, brand trends, and ratings using Python and pandas.

---

## 📂 Dataset Summary

- **Rows:** 20,000 (cleaned to 19,917)
- **Columns:** 15
- **Source:** Flipkart product scraping (public dataset)
- **Key Columns:** `product_name`, `brand`, `retail_price`, `discounted_price`, `product_rating`, `product_category_tree`

---

## 🧹 Data Cleaning Steps

- Dropped rows with missing `retail_price`, `discounted_price`, `image`, or `description`
- Converted ratings from `"No rating available"` to `NaN` and cast to `float`
- Dropped duplicates
- Filled missing brands with `"Unknown"`
- Resulting clean dataset: `flipkart_cleaned.csv` (19,917 rows)

---

## 🎯 Business Questions Explored

### ✅ 1. Which brands offer the most discounted products (by average %)?
We computed average discount percentage for each brand and identified the **Top 10 brands** with the highest discounts — most of them offer over 85% average discount.

### ✅ 2. What is the distribution of products across different price ranges?
We categorized products into price ranges (`<500`, `500-999`, `1000+`) and calculated the **average discount %** within each range. Surprisingly, **lower-priced products had higher average discounts**.

### ✅ 3. What is the distribution of retail prices and discount percentages?
- **Retail prices** are highly right-skewed with most products priced under ₹2000.
- **Discount percentages** peaked around 0% and 60%, with many products offering flat discounts.

---

## 📊 Visual Insights

We used a range of charts to uncover key trends in pricing and discounts:

### 🛒 Top Retail Price Points
![Top Retail Prices](visuals/top_retail_prices.png)

### 📉 Retail Price Distribution (Log Scale)
![Retail Price Log Distribution](visuals/log_scaled_retail_prices.png)

### 💸 Discount Distribution
![Discount Percent Distribution](visuals/discount_distribution.png)

### 🏷️ Top Brands by Average Discount
![Top Discount Brands](visuals/top_discount_brands.png)

### 🔢 Product Count by Discounted Price Range
![Product Count by Range](visuals/product_count_by_range.png)

### 📉 Average Discount by Price Range
![Average Discount by Range](visuals/avg_discount_by_price_range.png)

---

## 🛠️ Tools & Libraries

- **Language:** Python (Jupyter Notebook)
- **Libraries:** pandas, numpy, matplotlib, seaborn
- **IDE:** JupyterLab / VS Code

---

## 📁 Project Structure

```
Flipkart-Ecommerce-Analysis/
├── data/
│   └── flipkart_cleaned.csv
├── notebooks/
│   ├── 01_data_cleaning.ipynb
│   └── 02_eda_analysis.ipynb
├── visuals/
│   └── *.png (charts shown above)
└── README.md
```

---

## 📌 Next Steps

- Continue answering remaining business questions
- Identify patterns or pricing anomalies that could inform business decisions

---

## 🤝 Contact

Made with 💻 by [Aryavardhan Jain](https://www.linkedin.com/in/aryavardhanjain/)  
📫 jainaryan418@gmail.com  
🔗 [GitHub](https://github.com/aryavardhanjain)