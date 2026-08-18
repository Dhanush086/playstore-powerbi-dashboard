# Play Store App Performance & Sentiment Dashboard

An interactive **Power BI dashboard** analyzing app performance, pricing strategy, and user sentiment across the Google Play Store.

This project is a follow-up to my [Play Store EDA project](https://github.com/Dhanush086/Playstore-app-review-analysis), where I initially explored the dataset using **Python and Pandas**. The findings from that analysis were translated into a business-ready interactive dashboard using **Power BI**.

---

## Business Objective

**How can app publishers and product teams use category performance, pricing strategy, and user sentiment data to identify the best growth and monetization opportunities?**

The dashboard helps answer questions such as:

* Which app categories have the highest market reach?
* Which categories have the largest number of apps and competition?
* Do highly priced apps receive better ratings?
* Which categories have the strongest user sentiment?
* Are there categories with high ratings but hidden dissatisfaction in reviews?
* Where are the potential opportunities for growth and monetization?

---

## Dataset

**Source:** [Google Play Store Apps Dataset - Kaggle](https://www.kaggle.com/datasets/lava18/google-play-store-apps)

### Apps Table

* 9,637 apps after cleaning
* Category
* Rating
* Installs
* Price
* Size
* Type
* Content Rating

### Reviews Table

* Approximately 64,000 user reviews
* Sentiment labels:

  * Positive
  * Negative
  * Neutral

The same cleaned dataset was used in my [Python EDA project](https://github.com/Dhanush086/Playstore-app-review-analysis).

The data was further validated and cleaned in **Power Query**, including:

* Deduplication
* Data type conversion
* Malformed value handling
* Data merging
* Additional validation

---

## Tools & Technologies

| Tool             | Purpose                                                 |
| ---------------- | ------------------------------------------------------- |
| Power BI Desktop | Data modeling, DAX measures, interactive visualizations |
| Power Query      | Data cleaning, transformation, deduplication, merging   |
| Python / Pandas  | Initial dataset cleaning and exploratory data analysis  |

---

## Dashboard Overview

The dashboard is a **single-page interactive report** containing **7 visualizations and 3 global slicers**.

### Global Filters

* Category
* Type
* Content Rating

### Visualizations

| Visual                                   | Type         | Purpose                                                  |
| ---------------------------------------- | ------------ | -------------------------------------------------------- |
| Total Apps / Total Installs / Avg Rating | KPI Cards    | At-a-glance performance overview                         |
| App Distribution by Category             | Treemap      | Understand market volume and competition                 |
| Total Installs by Category               | Bar Chart    | Identify categories with the highest user reach          |
| Average Rating by Category               | Bar Chart    | Compare quality benchmarks across categories             |
| Price vs Rating                          | Scatter Plot | Analyze the relationship between app pricing and ratings |
| Overall Review Sentiment                 | Donut Chart  | Understand the overall sentiment split                   |
| Sentiment Distribution by Category       | Stacked Bar  | Identify category-level dissatisfaction patterns         |

---

## Key Insights

### Market Reach

* **9,637 apps** were analyzed.
* The overall average app rating is approximately **4.28**.
* The dataset contains **over 3 trillion combined installs**.
* **Games** lead with approximately **616 billion installs**.
* **Communication** follows with approximately **451 billion installs**.
* These categories have substantially higher user reach than most other categories.

### App Quality

* Category-level average ratings generally cluster between **4.0 and 4.5**.
* There are relatively few categories that significantly outperform or underperform the overall market.
* High install volume does not necessarily imply a significantly higher average rating.

### Pricing Strategy

* Among paid apps, **higher prices do not show a clear relationship with higher ratings**.
* This suggests that pricing alone is not a strong indicator of perceived app quality.
* Publishers may need to focus on product quality and user experience rather than relying on premium pricing to drive perceived value.

### User Sentiment

Overall review sentiment:

* **64% Positive**
* **22% Negative**
* **14% Neutral**

However, sentiment varies considerably across categories.

Some categories with strong install numbers and relatively high ratings still contain a meaningful proportion of negative reviews. This highlights the importance of analyzing **review sentiment alongside traditional KPIs such as ratings and installs**.

---

## Dashboard Preview

### Default View

![Dashboard Default View](images/dashboard_default.png)

### Filtered View

![Dashboard Filtered View](images/dashboard_filtered.png)

### Presentation Mode

![Dashboard Presentation Mode](images/dashboard_presentation.png)

> Replace the image paths above with the actual screenshot locations in your repository.

---

## Project Files

| File                   | Description                        |
| ---------------------- | ---------------------------------- |
| `dashboard.pbix`       | Interactive Power BI dashboard     |
| `dashboard_export.pdf` | Static PDF export of the dashboard |
| `documentation.pdf`    | Detailed project documentation     |

---

## How to Explore the Dashboard

### Option 1 - Power BI Desktop

Download `dashboard.pbix` and open it using **Power BI Desktop**.

You can interact with:

* Category filters
* App type filters
* Content rating filters
* Cross-filtering between visuals
* Individual chart selections
* KPI cards and category comparisons

### Option 2 - PDF Export

Open `dashboard_export.pdf` to view a static version of the dashboard without Power BI.

> A live Power BI Service link is not included because publishing requires a work or school email domain.

---

## Documentation

For a detailed explanation of the project, including:

* Dataset preparation
* Data cleaning
* Data modeling
* DAX measures
* Visualization design
* Individual visual insights
* Dashboard screenshots

See [`documentation.pdf`](documentation.pdf).

---

## Related Project

This dashboard builds upon my earlier Python-based exploratory data analysis:

**[Play Store App Review Analysis - Python / Pandas](https://github.com/Dhanush086/Playstore-app-review-analysis)**

The workflow can be summarized as:

```text
Google Play Store Dataset
          |
          v
Python / Pandas EDA
          |
          v
Data Cleaning & Validation
          |
          v
Power Query Transformation
          |
          v
Power BI Data Model
          |
          v
DAX Measures
          |
          v
Interactive Dashboard
          |
          v
Business Insights
```

---

## Business Takeaway

The dashboard demonstrates how app-store data can be transformed from raw records into actionable business insights.

Rather than looking at **installs, ratings, pricing, or sentiment in isolation**, combining these dimensions provides a more complete view of market opportunity:

**Market Reach + App Quality + Pricing + User Sentiment = Better Product & Monetization Decisions**

High-install categories may offer significant growth opportunities, but sentiment analysis can reveal user dissatisfaction that traditional ratings fail to capture. Similarly, pricing does not appear to be a reliable proxy for app quality, reinforcing the importance of product experience and customer satisfaction.

---

## Author

**Dhanush**

Data Analytics | Python | Pandas | Power BI | Data Visualization

[GitHub](https://github.com/Dhanush086)

