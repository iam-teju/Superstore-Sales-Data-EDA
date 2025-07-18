
# 📊 Superstore Sales EDA – Case Study

This project is a comprehensive Exploratory Data Analysis (EDA) of a Superstore sales dataset. The goal was to clean, transform, and analyze retail transaction data to uncover trends, inconsistencies, and actionable insights.

---

## 📁 Dataset

The dataset contains transactional sales data from a retail superstore, including:
- Order information
- Customer details (with PII masking)
- Shipping methods and durations
- Product categories and pricing
- Profitability and discount metrics

---

## ⚙️ Steps Performed

1. **Data Loading & Overview**
   - Inspected data types, missing values, and column summaries

2. **Cleaning**
   - Removed duplicates
   - Standardized date formats
   - Imputed missing values (e.g., `Ship Mode`, `Quantity`)
   - Converted postal codes and numeric fields
   - Masked customer names for privacy

3. **Feature Engineering**
   - Calculated `Original Price`, `Total Sales`, `Total Profit`, `Total Discount`, `Shipping Urgency`
   - Created `Days Since Last Order`
   - Aggregated customer-level metrics

4. **Outlier Detection**
   - Created reusable `remove_outliers()` function using the 3*IQR method
   - Applied on `Sales Price` and `Profit`

5. **Customer Segmentation**
   - Used quintiles for customer-level sales and profit analysis
   - Built a cross-tab to visualize overlap

6. **Data Visualization**
   - Profitable vs. loss-making products
   - Shipping mode analysis
   - Profit trends by region and state
   - Impact of discounts
   - Time series analysis of sales & profit

---

## 📊 Insights

- **Chairs** and **Phones** were among the most profitable products.
- **Same Day shipping** orders had lower profit margins.
- Some states consistently reported losses due to deep discounts.
- The **top 20% of customers (Q5)** contribute to the majority of sales and profits.
- There are seasonal spikes in sales during certain months.

---

## 🚀 How to Run

1. Open the `Superstore_EDA.ipynb` in Jupyter or Google Colab.
2. Upload the `SuperStore_Dataset.csv` file when prompted.
3. Run all cells (`Runtime > Run All` in Colab).
4. Output will include charts, summaries, and cleaned data.

---

## 🧹 Output

- ✅ Cleaned Dataset (as CSV)
- 📓 EDA Notebook (with reusable code)
- 📄 Summary Report (PDF or README insights)

---

## 🧠 Skills Applied

- Data Cleaning & Wrangling (Pandas, NumPy)
- Data Visualization (Matplotlib, Seaborn)
- Feature Engineering
- Outlier Detection
- Customer Segmentation
- Statistical Analysis
