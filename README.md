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

1. **Which categories have the highest average retail and discounted prices?**
2. **What are the top 10 most expensive products on Flipkart?**
3. **Which brands offer the most discounted products (absolute and % terms)?**
4. **How does average discount (%) vary across categories?**
5. **What is the distribution of products across different price ranges?**
6. **Which categories have the highest number of listings?**
7. **Which products or brands have the highest ratings (if available)?**
8. **How does the average rating vary by category or brand?**

---

## 📊 Tools & Libraries

- **Language:** Python (Jupyter Notebook)
- **Libraries:** pandas, numpy, matplotlib, seaborn
- **IDE:** JupyterLab / VS Code

---

## 📈 Project Structure

```
Flipkart-Ecommerce-Analysis/
│
├── data/
│   └── flipkart_cleaned.csv
├── notebooks/
│   └── 01_data_cleaning.ipynb
├── visuals/
│   └── (to be added in EDA)
├── README.md
```

---

## 📌 Next Steps

- Perform in-depth EDA and visualizations
- Answer the business questions with plots and summary tables
- Identify patterns or pricing anomalies that could inform business decisions

---

## 🤝 Contact

Made with 💻 by [Aryavardhan Jain](https://www.linkedin.com/in/aryavardhanjain/)  
📫 jainaryan418@gmail.com  
🔗 [GitHub](https://github.com/aryavardhanjain)
