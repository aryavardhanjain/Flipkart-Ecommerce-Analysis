
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
- Final cleaned dataset: `flipkart_cleaned.csv` (19,917 rows)

---

## 🎯 Business Questions Explored

1. **Which brands offer the most discounted products (by average %)?**
2. **What is the distribution of products across different price ranges?**
3. **What is the distribution of retail prices and discount percentages?**
4. **What are the most common retail price points?**
5. **Which brands have the highest-rated products?**
6. **Which brands have the highest-rated products with at least 10 ratings?**
7. **What’s the distribution of ratings across all products?**
8. **What are the top 10 most expensive products?**
9. **Which categories have the most product listings?**

---

## 📊 Visual Insights

All answers are supported with visualizations in the `/visuals` folder.

---

## 🛠️ Tools & Libraries

- Python (Jupyter Notebook)
- pandas, numpy, matplotlib, seaborn

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

## 🤝 Contact

Made with 💻 by [Aryavardhan Jain](https://www.linkedin.com/in/aryavardhanjain/)  
📫 jainaryan418@gmail.com  
🔗 [GitHub](https://github.com/aryavardhanjain)
