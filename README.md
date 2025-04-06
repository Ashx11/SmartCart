# 🛒 SmartCart – Recommender System & Pattern Mining

This project simulates an e-commerce platform using Collaborative Filtering and Association Rule Mining to provide product recommendations and discover frequent purchase patterns.

---

## 📁 Project Structure

```
SmartCart/
├── data/
│   ├── ecommerce_user_data.csv
│   └── product_details.csv
│
├── SmartCart.ipynb            # Main Jupyter notebook
├── smartcart_script.py        # Python script (optional)
├── report.pdf                 # Final project report
├── README.md                  # Project instructions
└── outputs/
    ├── recommendations.csv    # Recommended products
    ├── heatmap.png            # User similarity heatmap
    └── frequent_items.png     # Frequent itemsets visualization
```

---

## 🚀 How to Run the Project

### 1. Install Required Libraries

Make sure you have Python installed. Then run the following to install dependencies:

```bash
pip install pandas numpy scikit-learn mlxtend matplotlib seaborn
```

---

### 2. Run the Notebook

Launch Jupyter Notebook and open the main notebook file:

```bash
jupyter notebook SmartCart.ipynb
```

Run each cell in order to reproduce the results.

---

### 3. Run the Python Script (Optional)

If a script version is provided:

```bash
python smartcart_script.py
```

---

## 📊 Output Files

All generated outputs will be saved in the `outputs/` folder:

- `recommendations.csv` – Top-5 recommended products for each user
- `heatmap.png` – Cosine similarity heatmap of users
- `frequent_items.png` – Visualization of frequent product bundles

---

## 🧪 Evaluation Notes

This project evaluates the recommender system using:

- **Mean Average Precision (MAP@K)** – A measure of ranking quality over the top K recommendations.
- **@K** refers to evaluating the top K recommended items (e.g., @5 means top 5 items).
- Due to data sparsity, traditional Precision@K was replaced with MAP for better evaluation insight.

> The dataset contains 50 users, 100 products, and 724 total ratings, resulting in a sparse matrix. As such, evaluation was done using a manually constructed test set by removing high-rated items and checking if they were successfully recommended back.

---

## 📄 Report

Read `report.pdf` for:

- Description of methods used
- Visualizations and insights
- Answers to conceptual questions
- Discussion on challenges and improvements

---

## 📌 Notes

- Place both `ecommerce_user_data.csv` and `product_details.csv` inside the `data/` folder.
- Ensure all paths are correct when running scripts or notebooks.
- You can adjust the number of top recommendations (K) and rule mining thresholds inside the notebook.
