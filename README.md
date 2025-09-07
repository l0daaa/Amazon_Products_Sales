# 📒 Amazon Products Sales Dataset – Exploratory Data Analysis (EDA)

## 📌 Project Overview
This repository contains the Jupyter Notebook **`EDA.ipynb`**, which performs an in-depth **Exploratory Data Analysis (EDA)** on the [Amazon Products Sales Dataset (2025)](https://www.kaggle.com/datasets/ikramshah512/amazon-products-sales-dataset-42k-items-2025).  

The notebook focuses on cleaning, transforming, and analyzing product-level data to uncover insights into **pricing, discounts, customer ratings, reviews, and sales performance**.

---

## 🛠️ Tools & Libraries
The notebook is implemented in **Python 3** using the following libraries:
- **pandas** – data manipulation and cleaning  
- **numpy** – numerical operations  
- **matplotlib & seaborn** – data visualization  
- **missingno** – missing data visualization  

---

## 📂 File Description
- **EDA.ipynb** → Jupyter Notebook containing the entire analysis process.

---

## 🔍 Notebook Workflow
The notebook is structured into the following steps:

1. **Import Libraries & Load Data**  
   - Load dataset into a Pandas DataFrame  
   - Initial exploration (shape, info, sample view)  

2. **Data Cleaning**  
   - Handle missing values  
   - Convert text columns (`rating`, `number_of_reviews`, `bought_in_last_month`) into numeric  
   - Drop irrelevant columns (URLs, images, badges, etc.)  

3. **Feature Engineering**  
   - `discount_percentage` (relative discount)  
   - `price_difference` (absolute price gap)  
   - `is_high_rating` (flag for rating > 4)  
   - `is_discounted` (boolean for discounts)  
   - `price_category` (low / medium / high price bins)  
   - `product_category` (derived from product names using keyword mapping)  

4. **Exploratory Data Analysis (EDA)**  
   - **Univariate Analysis**: product categories, ratings, prices, discount percentages  
   - **Bivariate Analysis**:  
     - Ratings vs. Reviews  
     - Price Category vs. Sales  
     - Discount Percentage vs. Sales  
   - **Correlation Heatmap**: overview of numeric relationships  

5. **Key Insights** (documented inline within the notebook)

---

## ▶️ How to Run
1. Clone this repository:  
   ```bash
   git clone https://github.com/your-username/amazon-sales-eda.git
Navigate into the repo and open the notebook:

bash
Copy code
jupyter notebook notebooks/EDA.ipynb
Download the dataset from Kaggle and place it inside a Data/ folder.

Run all cells sequentially.

📎 Notes
The dataset is not included in the repo due to size.

All plots are generated dynamically in the notebook.

Insights and interpretations are provided inline for clarity.

 Author
Khaled Youssef
Data Analysis & Machine Learning Enthusiast

 If you find this useful, don’t forget to star the repo!
