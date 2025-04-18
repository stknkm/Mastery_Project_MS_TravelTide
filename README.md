# Mastery_Project_MS_TravelTide

# ✈ TravelTide User Clustering & Loyalty Perk Recommendation

This project focuses on analyzing user behavior from a travel booking platform to segment users into meaningful groups using unsupervised learning (PCA + KMeans). Based on these clusters, we recommend personalized loyalty perks to improve user engagement and retention.

---

##  Project Goal

- Segment users based on their behavior, demographics, and spending patterns
- Understand each cluster’s travel preferences and value to the business
- Recommend one optimal loyalty perk per segment to boost engagement and revenue

---

##  Dataset

The dataset includes detailed user session data, bookings, cancellations, hotel stays, flight preferences, demographic data, and more.

**Key features used:**
- Demographics: age, marital status, children
- Behavior: session duration, page clicks, trip frequency
- Travel: average nights, return flight ratio, baggage usage
- Value: total spend, value per day, dollars saved
- Engagement metrics: booking conversion, engagement score

---

##  Process Overview

1. **Data Preprocessing**
   - Date parsing and corrections
   - Cleaning inconsistent values (e.g., negative nights)
   - Feature engineering (e.g., trip frequency, combo trip ratio, cancellation rate)

2. **Outlier Analysis**
   - Visualization of skewed distributions and boxplots
   - Applied log-transformation to reduce skewness and keep valuable outliers

3. **Dimensionality Reduction**
   - Applied PCA to reduce noise and keep principal behavioral dimensions

4. **Clustering**
   - Used KMeans with 6 clusters
   - Evaluated quality using Silhouette Score (0.53)

5. **Cluster Profiling**
   - Assigned user-friendly names and characteristics to each cluster
   - Mapped tailored perks based on user needs and business value

---

##  Cluster Summaries & Perks

| Cluster | Name               | Description Highlights                                               | Suggested Loyalty Perk            |
|--------:|--------------------|----------------------------------------------------------------------|------------------------------------|
| 0       | Seniors            | Oldest, married, low usage and low spend                             |  Free Baggage                    |
| 1       | Young Singles      | Active, young, frequent trips, high conversion                       |  Exclusive Discounts             |
| 2       | Family Travelers   | Married with kids, hotel-focused, moderate travel & value            |  Free Hotel Meals                |
| 3       | Business Travelers | High activity & engagement, very efficient users                     |  No Cancellation Fees            |
| 4       | Dreamers           | High interest, browsing but not booking                              |  Free Hotel Night (with flight)  |
| 5       | Normal Travelers   | Young, low activity, low value                                       |  Exclusive Discounts             |

---

##  Key Metrics Visualized

- Feature distributions and outliers
- PCA explained variance
- Cluster size and separation
- Cluster centers and comparison tables

---

##  Tech Stack

- SQL,Python (Pandas, NumPy, Scikit-learn)
- Visualization: Matplotlib, Seaborn, Plotly
- Google Colab for development and annotation



---


Developed as part of a data science project.
