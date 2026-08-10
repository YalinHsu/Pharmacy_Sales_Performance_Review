# Power BI Portfolio Project | Pharmacy Sales Performance Analysis

## Business Context

This is a self-directed Power BI project using 5 years of pharmacy sales data from 2014 to 2018 across 8 drug categories.

Instead of building a dashboard that only shows sales performance, I wanted to understand the story behind the numbers:

* Which categories contribute most to overall sales?
* What caused the sales decline from 2016 to 2017?
* When does demand usually happen?
* Are there any seasonal patterns behind the sales trend?

The report contains four pages, moving from an overall performance review to category-level and time-based analysis, followed by a drillthrough page for a closer look at individual categories.

**Dataset:** [Pharmaceutical Drug Sales Dataset (Kaggle)](https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data) — a publicly available dataset.

📄 **Full report:** [Pharmacy Sales Performance Review](Pharmacy_Sales_Performance_Review.pdf)

---

## Report Pages

### 1. Executive Summary — Overall Performance

From 2014 to 2018, total sales reached **$110.5K**.

**N02BE/B (Other analgesics and antipyretics, Pyrazolones and Anilides)** was the largest category, contributing **49.8% of total sales**.

At the overall sales level, **January 2017 was the highest-performing month, with $2.7K in total sales**. The annual trend shows that sales peaked in 2016, declined in 2017, and started to recover in 2018.

These findings led me to look more closely at two questions: why does N02BE/B contribute so much to total sales, and what was behind the decline in 2017?

*Figure: Annual sales trend and category share, 2014–2018.*

---

### 2. Category Insights — What Drove the Decline?

The Pareto analysis shows that sales are highly concentrated: the top 4 categories account for **81% of total sales**, with N02BE/B alone contributing almost half.

I then used a waterfall chart to understand the decline from 2016 to 2017. The analysis shows that **N02BE/B accounted for around 70% of the total decline**.

This means the overall drop was not equally spread across all categories. Most of the change came from one major category.

*Figure: Pareto analysis and waterfall breakdown of the 2016–2017 sales decline.*

---

### 3. Time Analysis — When Does Demand Happen?

This page looks at sales from an operational perspective: **when are sales happening?**

The weekday × hour heatmap shows stronger activity on **Saturdays**, with noticeable peaks around **7–8 PM and 11 AM–12 PM**.

The hourly sales chart provides a closer look at how demand changes across the day and highlights the busiest hours.

*Figure: Weekday × hour demand heatmap and hourly sales distribution.*

---

### 4. Category Details — Drillthrough & Seasonality

The final page is a drillthrough page that allows users to select a category and explore its monthly trend and seasonality in more detail.

Looking more closely at **N02BE/B (Other analgesics and antipyretics, Pyrazolones and Anilides)** revealed a clear seasonal pattern, with higher sales from **October to January**. **R03 (Drugs for obstructive airway diseases)** shows a similar winter pattern, while most other categories remain relatively stable throughout the year.

From a pharmaceutical perspective, the similar winter patterns in N02BE/B and R03 may be related to higher demand for pain, fever, and respiratory treatments during the cold and flu season.

This also provides useful context for the January 2017 sales peak identified on the Executive Summary page.

*Figure: Category-level monthly trend and seasonality comparison via drillthrough.*

---

## What I Worked On

* **Data Modeling** — Built the Power BI data model from transaction-level pharmacy sales data.
* **DAX** — Created measures for total sales, moving averages, category contribution, and other performance metrics.
* **Category Analysis** — Used Pareto and waterfall charts to understand both sales concentration and the 2016–2017 decline.
* **Time Analysis** — Analyzed sales patterns by weekday and hour using a heatmap and hourly ranking.
* **Drillthrough Analysis** — Built a category-level drillthrough page to explore trends and seasonality.
* **Business Interpretation** — Connected the N02BE/B and R03 winter sales patterns with pharmaceutical knowledge of cold and flu season.

---

## Tech Stack

* Power BI
* DAX
* Data Modeling
* Data Visualization

---

## What I Learned

This project helped me practice moving beyond simply showing KPIs and charts and instead using Power BI to answer business questions step by step.

One of the most interesting findings was the 2016–2017 sales decline. At first, the overall trend only showed that sales had fallen. After breaking the change down by category, I found that **N02BE/B alone contributed around 70% of the decline**.

The drillthrough analysis also showed why domain knowledge can be useful when interpreting data. The winter sales pattern in N02BE/B and R03 is consistent with the expected increase in demand for pain, fever, and respiratory treatments during the cold and flu season.

At the same time, I was careful about what the dataset cannot explain. The data can show **which category contributed to the decline**, but it does not contain market, competitor, pricing, or supply chain information, so it cannot tell us **why N02BE/B sales declined in 2017**.

---

## Project Structure

```text
Pharmacy_Sales_Performance_Review
│
├── README.md
├── Pharmacy_Sales_Performance_Review.pdf
│
└── screenshots/
    ├── 01_executive_summary.png
    ├── 02_category_insights.png
    ├── 03_time_analysis.png
    └── 04_category_details.png
```

---

## Data Source

This project uses the publicly available [Pharmaceutical Drug Sales Dataset](https://www.kaggle.com/datasets/milanzdravkovic/pharma-sales-data) from Kaggle, covering pharmacy sales from 2014 to 2018 across 8 drug categories.

The dataset contains sales transaction data but does not include market, competitor, pricing, inventory, or supply chain information. Therefore, the analysis focuses on identifying sales patterns and category contributions rather than explaining the business reasons behind the changes.

---

**Ya-Lin Hsu** · [LinkedIn](https://www.linkedin.com/in/yalin-hsu) · [yalinhsu.work@gmail.com](mailto:yalinhsu.work@gmail.com)
