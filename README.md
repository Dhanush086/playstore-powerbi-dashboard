#  Play Store App Performance & Sentiment Dashboard

An interactive Power BI dashboard analyzing app performance, pricing strategy, and user sentiment across the Google Play Store — built as a follow-up to my [Play Store EDA project](https://github.com/Dhanush086/Playstore-app-review-analysis) (Python/Pandas), translating those findings into a business-ready visual tool.

---

##  Business Objective

**How can app publishers and product teams use category performance, pricing strategy, and user sentiment data to identify which app categories offer the best growth and monetization opportunities?**

---

##  Dataset

**Source:**
[https://www.kaggle.com/datasets/yassershrief/goggle-play-data ](https://www.kaggle.com/datasets/yassershrief/goggle-play-data?utm_source=chatgpt.com)

[Google Play Store User Reviews - Kaggle](https://www.kaggle.com/datasets/rowemorehouse/googleplaystoreuserreviews)
            
* **Apps table:** 9,638 apps (post-cleaning) — category, rating, installs, price, size, type, content rating
* **Reviews table:** ~64,000 user reviews with sentiment labels (Positive / Negative / Neutral)

Same cleaned dataset used in my [Python EDA project](https://github.com/Dhanush086/Playstore-app-review-analysis) — re-validated and further cleaned in Power Query for this dashboard (deduplication, type conversion, malformed value handling).

---

##  Tools Used

* **Power BI Desktop** — data modeling, DAX measures, visualization
* **Power Query** — data cleaning: type conversion, deduplication, merge
* **Python / Pandas** — initial dataset cleaning, upstream of this dashboard

---

##  Dashboard Overview

A single-page interactive dashboard with **7 visuals** and **3 global slicers** (Category, Type, Content Rating).

| Visual | Type | Purpose |
|---|---|---|
| Total Apps / Total Installs / Avg Rating | KPI Cards | At-a-glance orientation |
| App Distribution by Category | Treemap | Market volume/competition per category |
| Total Installs by Category | Bar Chart | Which categories dominate user reach |
| Average Rating by Category | Bar Chart | Quality benchmark per category |
| Price vs Rating (Paid Apps) | Scatter Plot | Whether price correlates with rating |
| Overall Review Sentiment | Donut Chart | Positive/Negative/Neutral split |
| Sentiment Distribution by Category | Stacked Bar | Hidden dissatisfaction despite decent ratings |

---

##  Key Insights

* 9,637 apps analyzed, averaging a **4.28** rating, with over **3 trillion** combined installs
* **Games (616bn)** and **Communication (451bn)** apps dominate total installs, far ahead of every other category
* Category average ratings cluster tightly between **4.0–4.5** — few categories significantly under- or out-perform the pack
* Among paid apps, higher price does **not** clearly correlate with higher rating — quality is fairly independent of price point
* **64% Positive / 22% Negative / 14% Neutral** — sentiment breakdown varies notably by category, revealing categories with strong install/rating numbers that still carry a meaningful share of negative reviews

---

## Dashboard Preview

### Default View

![Dashboard Default View](screenshots/dashboard_default.png)

### Filtered View

![Dashboard Filtered View](screenshots/dashboard_filtered.png)

### Presentation Mode

![Dashboard Presentation Mode](screenshots/dashboard_presentation_mode.png)

---

##  Links

* **Interactive file:** [playstore_dashbord.pbix ](https://github.com/Dhanush086/playstore-powerbi-dashboard/blob/main/playstore_dashbord.pbix)— download and open in Power BI Desktop (free) to explore all filters and interactions
* **Static PDF export:** [Download the Dashboard PDF](https://github.com/Dhanush086/playstore-powerbi-dashboard/blob/main/playstore_dashbord.pdf)

> A live Power BI Service shareable link isn't included, as publishing requires a work/school email domain. The `.pbix` file and PDF export provide full access to the dashboard and its design.

---

##  Documentation

Full documentation — including dataset details, per-visual insight explanations, and screenshots — is available in [`documentation.pdf`](documentation.pdf).

---

## Author

**Dhanush**
Data Analytics | Python | Pandas | Power BI | Data Visualization

[GitHub](https://github.com/Dhanush086)

