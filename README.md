# Ontario-Library-Financial-Analysis



# 📘 Ontario Library Financial Report (2006–2010)

## 📌 Overview

This project analyzes financial and operational data for Ontario public libraries from 2006 to 2010. It focuses on understanding library funding efficiency, user engagement, and key performance metrics over time.

---

## 📁 Files & Data Sources

* **CSV Inputs:** Annual library datasets (`2006.csv` through `2010.csv`)
* **Combined Output:** `library_data.csv` (merged dataset)
* **Final Output:** `library_data_with_metrics.csv` (includes derived metrics)

---

## 🔧 Tools & Libraries

* **Data Manipulation:** `dplyr`, `reshape2`, `tidyverse`
* **Reporting:** `knitr`, `tinytex`
* **Visualization:** `ggplot2`, `base::heatmap()`

---

## 📊 Key Steps & Insights

### ✅ Data Preparation

* Combined yearly datasets using `rbind()`
* Cleaned column names to remove special characters
* Converted relevant columns to numeric (e.g., revenue, population)
* Filtered unrealistic revenue-per-cardholder values (> \$2,500)

### 📈 Insight 1: Correlation Analysis

* **Metric:** Revenue per Cardholder vs. Local Operating Grant
* **Result:** Weak positive correlation (\~0.012), suggesting minimal direct influence.

### 📊 Insight 2: Population-Based Analysis

* Grouped libraries into **Small, Medium, Large** based on population.
* Summarized average revenue per cardholder by **Year** and **Population Group**.
* **Visualization:** Boxplots showed small libraries had more variance in revenue efficiency.

### 🔥 Insight 3: Heatmap of Top 10 Libraries

* Identified top libraries by average revenue per cardholder.
* Created a **year-by-library heatmap** highlighting trends in high-performing institutions.

---

## 📉 Sample Visualizations

* **Bubble Plot:** Revenue per Cardholder vs. Local Grant (size = population)
* **Box Plot:** Revenue distribution by population and year
* **Heatmap:** Top 10 Libraries – Year-wise revenue efficiency

---

## 📤 Output

Final CSV: `library_data_with_metrics.csv`
Includes:

* Cleaned data
* `RevPerCardholder` metric
* Filtered rows for analysis integrity

---

## 🧠 Usage & Applications

This analysis can support:

* Budget planning and funding allocation
* Performance benchmarking across library systems
* Policy recommendations for underserved areas

