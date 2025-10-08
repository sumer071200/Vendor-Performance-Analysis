# 📊 Vendor Performance Data Analysis

## 📝 Overview
This project analyzes **vendor performance metrics** to identify key profitability drivers, cost inefficiencies, and sales patterns.  
The analysis uses descriptive statistics, outlier detection, and correlation insights to guide **pricing strategies**, **inventory optimization**, and **vendor negotiations**.

---

## ✨ Key Insights

### 📉 Summary Statistics
- **Negative and Zero Values**:
  - *Gross Profit*: Minimum value of **-52,002.78**, indicating losses on some transactions.
  - *Profit Margin*: Minimum of `-∞`, suggesting zero or negative revenue in some cases.
  - *Sales Quantity & Dollars*: Minimum values at **0**, highlighting obsolete or slow-moving stock.

- **High Standard Deviations / Outliers**:
  - *Purchase Price*: Range from `0.09` to `257,032.07` indicates pricing inconsistencies and premium products.
  - *Freight Cost*: Extreme variation reflects logistics inefficiencies.
  - *Stock Turnover*: Ranges from `0` to `274.5`. Values above 1 suggest fulfilling orders from older inventory.

---

### 📈 Correlation Insights
- **Purchase Price** has **weak correlation** with Total Sales Dollars (-0.012) and Gross Profit (-0.016).  
- **Strong positive correlation** (0.999) between **Total Purchase Quantity** and **Total Sales Quantity** indicates efficient inventory turnover.  
- **Negative correlation** between Profit Margin and Total Sales Price (-0.179) implies margin compression as sales price increases.  
- **Stock Turnover** has weak negative correlation with Gross Profit (-0.038) and Profit Margin (-0.055).

---

### 💡 Pricing Strategy Insight
- Vendors buying in bulk (large order size) receive the **lowest unit price** (`$10.78 per unit`), yielding higher margins when inventory is efficiently managed.
- Bulk pricing creates a **-72% cost reduction** compared to small orders.
- Bulk pricing strategy effectively **encourages higher order volumes**, leading to increased overall sales.

---

## 🧰 Tech Stack
- **Language**: Python  
- **Libraries**:
  - `pandas` — data manipulation & aggregation  
  - `numpy` — numerical operations  
  - `matplotlib` / `seaborn` — visualization  
  - `openpyxl` — Excel file handling

---

## ⚙️ How to Run the Notebook

1. 📥 Clone or download this repository:
   ```bash
   git clone https://github.com/your-username/vendor-performance-analysis.git
   cd vendor-performance-analysis
