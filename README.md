# 📦 Amazon Product Reviews Analytics: Unveiling Data Reliability

## 🎯 Project Philosophy
> **"The first insight isn't always the right one. Real analysis begins when you question the initial results, rather than just celebrating them."**

In this project, I tackled a massive Amazon product dataset. While the initial premise seemed straightforward—analyzing user ratings and their impact on sales—diving into the raw rows revealed a deeper business challenge: **Data Reliability**. This project showcases how critical data skepticism is to avoiding misleading business conclusions.

---

## 📊 Dataset Scale at a Glance
* **Total Rows:** `1.5 Million` Record Staged
* **Total Products:** Over `1 Million` unique items
* **Total Monthly Revenue Analyzed:** `~$161M`

---

## 🚀 The Analytics Journey & Critical Discoveries

### 1️⃣ The Surface-Level Insight (The Trap)
After conducting initial data cleansing in Power BI, I utilized **DAX** to construct a calculated column named `Rating Category`. 
* **The Initial Result:** The vast majority of sales were heavily concentrated in the "Excellent" (4–5 stars) category. 
* **The Catch:** While this seemed logical on the surface, it felt incomplete. I questioned whether every 4 or 5-star rating was genuinely trustworthy or simply biased by low-engagement products.

### 2️⃣ Deep Diving into Reliability (The Breakthrough)
To uncover the hidden truth, I engineered a brand-new conditional metric using DAX to segment products based on engagement verification:
* **Verified/Reliable:** Products that possess active text **Reviews**.
* **Unreliable:** Products with high ratings but **Zero Reviews** written.

By deploying this logic as a dynamic **Slicer**, the true patterns emerged:
* High-sales volumes were exclusively driven by *Verified* Excellent ratings (4-5 stars).
* Products with high star ratings but zero actual reviews had a negligible impact on overall financial performance.

### 3️⃣ Sector Dominance Focus
* **Top Performing Category:** **Girl’s Clothing** emerged as the ultimate dashboard driver, dominating across all three major axes: **Highest Ratings**, **Highest Sales Volume**, and the **Most Significant Statistical Impact** on the overall dashboard.

---

## 📊 Dashboard Visual View

### 🖼️ Amazon Product Review & Sales Analysis
![Amazon Product Reviews Dashboard](https://raw.githubusercontent.com/abdelrahmanabdulaty010644-sys/proudect-review-analysis/main/Screenshot%202026-05-13%20124108.png)

---

## 💡 Key Business Takeaways
* **Data Quality > Data Quantity:** Processing 1.5 million rows is meaningless if you can't filter out the noise.
* **Analytical Mindset:** A great analyst doesn't just build pretty charts; they challenge the data to extract trustworthy, risk-free insights for stakeholders.

---

## 🛠️ Tools & Techniques Used
* **Microsoft Power BI** - End-to-end processing, visual layout distribution, and interactive filtering.
* **Power Query** - Heavy lifting for initial data cleansing and structural data transformations on 1.5M rows.
* **DAX Formulas** - Crafted calculated columns for logical text segmentation (`Rating Category` and `Reliability Status`).

---
📩 **Let's Connect! Feel free to reach out to discuss data engineering, analytics, or feedback:**
* [LinkedIn](https://www.linkedin.com/in/abdelrahman-mohamed-1034b7387/)
* [Email](mailto:abdelrahman.abdulaty@gmail.com)
