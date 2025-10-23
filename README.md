# 🧠 Analysis of Trader Behavior vs. Market Sentiment

## 📄 Project Overview

This project analyzes the relationship between **trader behavior** and **overall market sentiment**, using the **Fear & Greed Index** as a key indicator.
The analysis aims to uncover patterns or signals by comparing trader **profitability (PnL)**, **trade side (Buy/Sell)**, and **trade volume (Size USD)** across different sentiment levels.

---

## 🎯 Objectives

* Identify how market sentiment influences trader profitability.
* Examine whether traders are more likely to **buy** or **sell** during “Fear” vs. “Greed” conditions.
* Analyze how trade volume changes with sentiment intensity.

---

## 🧩 Datasets Used

1. **historical_data.csv** – Contains trader-level information such as trade side, PnL, and trade size.
2. **fear_greed_index.csv** – Contains daily sentiment data classified into categories such as *Extreme Fear*, *Fear*, *Neutral*, *Greed*, and *Extreme Greed*.

---

## ⚙️ Methodology

1. **Data Matching:**
   Identified a **common factor (`date`)** present in both datasets to enable alignment and comparison.

2. **Data Merging:**
   Combined both datasets into one unified DataFrame based on the matching `date` column.

3. **Data Filtering and Visualization:**
   Extracted only relevant columns and rows for the analysis, then visualized findings using **Matplotlib** and **Seaborn**.

---

## 📊 Key Findings

### 1️⃣ Profit & Loss (PnL) vs. Sentiment

* **Finding:** Profitability was **highest during “Extreme Greed”** (avg. ≈ $68).
* **Insight:** Traders following optimistic market trends tended to perform best.
* **Lowest profitability:** During “Extreme Fear” and “Neutral” (avg. ≈ $34).

---

### 2️⃣ Trade Side (Buy/Sell) vs. Sentiment

* **Finding:** The ratio of “Buy” to “Sell” trades remained nearly **50/50** across all sentiment levels.
* **Insight:** Market sentiment had **no significant effect** on trade direction — the market remained balanced regardless of mood.

---

### 3️⃣ Trade Volume vs. Sentiment

* **Finding:** **Highest trade volume** occurred during **“Fear”** periods (avg. ≈ $7,800).
* **Insight:** Traders tend to trade **more aggressively or commit larger amounts** during fearful markets — possibly due to panic selling or “buy-the-dip” activity.

---

## 🧾 Conclusion

* Profitability peaks during **Extreme Greed**.
* The **Buy/Sell ratio** remains constant regardless of sentiment.
* **Trade volume spikes during Fear**, suggesting more emotional or high-capital movements in uncertain markets.

---

## 🗂️ Folder Structure

```
ds_<your_name>/
├── notebook_1.ipynb        # Main Google Colab notebook with analysis and visualizations
├── csv_files/              # Contains raw and processed CSV data
│   └── *.csv
├── outputs/                # Stores all generated plots, charts, and visual outputs
│   └── *.png / *.jpg
├── ds_report.pdf           # Final summarized report (this file)
└──README.md               # Setup instructions and project overview
```

---

## 🧰 Tools & Libraries

* **Python**
* **Pandas** – Data manipulation and merging
* **Matplotlib / Seaborn** – Data visualization
* **Google Colab** – Notebook execution environment

---

## 🚀 How to Run the Project

1. Open `notebook_1.ipynb` in **Google Colab**.
2. Upload the required CSVs from the `csv_files` folder.
3. Run all cells sequentially to reproduce the analysis.
4. Generated visual outputs will be saved in the `outputs` folder.

---

## 🧑‍💻 Author

**Aditya Raj**
Data Science Candidate
