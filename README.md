## README: Jumia Product Performance Dashboard

### Project Overview
This project involves designing an interactive Excel dashboard to analyze Jumia product data. The goal is to uncover how pricing strategies, discounts, and customer feedback (ratings/reviews) drive product performance and engagement in the Kenyan e-commerce market.

---

### 🛠 Data Cleaning & Preparation
Before analysis, the raw dataset must be processed using the following steps:
* **De-duplication:** Remove duplicate product entries.
* **Standardization:** Use **Find & Replace (Ctrl+H)** or **Text-to-Columns** to remove "KSh" and commas from price columns.
* **Numeric Conversion:** * Convert **Ratings** (e.g., "4.5 out of 5") to a simple numeric scale.
    * Ensure **Discounts** are formatted as percentages.
    * Handle missing values in the Reviews and Ratings columns.
* **Validation:** Correct any negative review counts to positive values.

### 📊 Data Enrichment (Calculated Columns)
To enhance the analysis, the following fields are created:
1.  **Discount Amount:** `Old Price - Current Price`
2.  **Rating Category:** * *Poor*: < 3
    * *Average*: 3 – 4.4
    * *Excellent*: ≥ 4.5
3.  **Discount Category:**
    * *Low*: < 20%
    * *Medium*: 20% – 40%
    * *High*: > 40%

---

### 📈 Key Analysis Objectives
The dashboard aims to answer:
* **Descriptive Stats:** Average prices, discounts, and ratings across the catalog.
* **Performance Leaders:** Top 10 products by discount and review volume; top/bottom 5 by rating.
* **Correlation Analysis:** * Does a higher discount lead to more reviews (engagement)?
    * Do highly-rated products attract a higher volume of reviews?
* **Segment Comparison:** Comparing "High Discount" vs. "Low Discount" products regarding customer satisfaction.

---

### 🖥 Dashboard Features
The final Excel output is a single-page interactive interface featuring:
* **KPI Summary:** Total products, average rating, average discount, and total reviews.
* **Visualizations:** * **Bar/Column Charts:** Product rankings.
    * **Pie/Donut Charts:** Distribution of Rating and Discount categories.
    * **Scatter Plots:** Relationships between discounts, ratings, and reviews.
* **Interactivity:** **Slicers** for Rating Category, Discount Category, and Price Range to allow for dynamic filtering.
* **Conditional Formatting:** Visual cues to highlight underperforming ratings or exceptional discounts.

---
