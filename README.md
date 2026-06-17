# 🎬 Netflix User Engagement & Retention Optimization
> **An End-to-End Advanced Analytics & Machine Learning Pipeline for Subscriber Segmentation**

[![Python](https://img.shields.io/badge/Python-3.12-blue.svg)](https://www.python.org/)
[![SQL](https://img.shields.io/badge/SQL-SQLite-orange.svg)](https://www.sqlite.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Latest-green.svg)](https://scikit-learn.org/)

---

## 📌 1. Problem Identification
In the highly competitive streaming industry, customer acquisition costs (CAC) are exponentially rising. Maximizing the **Lifetime Value (LTV)** of active users and minimizing subscription cancellations (**Churn Rate**) has become the primary operational leverage for sustainable corporate growth. 

### **The Business Problem:**
The global subscriber base is currently treated as a single homogeneous group. This creates inefficiency in product delivery and marketing, leading to misaligned content recommendation algorithms, higher subscriber attrition (churn), and sub-optimal resource allocation.

---

## 🎯 2. Project Objectives & Business Possibilities
To address this inefficiency, this project designs and runs a dual-layer technical pipeline to segment users based on their geometric behavioral proximity.

* **Possibility A (Strategic Marketing Acceleration):** By identifying unique platform archetypes (Personas), marketing departments can transition from generic blasts to hyper-personalized, trigger-based retention campaigns.
* **Possibility B (Product Recommendation Optimization):** UI/UX engineering teams can customize the streaming interface layout dynamically based on the active user’s operational profile.
* **Possibility C (Financial Risk Mitigation):** Isolating clusters with statistically high churn coefficients allows financial analysts to implement targeted proactive retention subsidies before revenue drop-off occurs.

---

## 🛠️ 3. System Architecture & Pipeline Design
The development follows a production-grade data science workflow:

[Raw SQL Data Storage] ──> [Feature Transformation & Scaling] ──> [PCA Variance Compression]
│
[Business Segment Deployment] <── [Twin-Axis Metric Optimization] <── [K-Means Mini-Batch Clustering]

1. **Data Engineering via SQL Engine:** Direct raw relational database simulation (`sqlite3`) to aggregate and isolate high-value user metrics.
2. **Feature Engineering:** Scaling variables via `StandardScaler` and converting categorical attributes using One-Hot Encoding.
3. **Dimensionality Reduction (PCA):** Compressing the sparse feature matrix into 6 principal component axes to avoid the *Curse of Dimensionality* while retaining maximum data variance.
4. **Hyperparameter Tuning:** Dual-validation utilizing the **Elbow Method (WCSS)** and **Silhouette Coefficients** to mathematically locate the optimal number of clusters ($K=4$).
5. **Business Profiling:** Mapping cluster outputs back to real-world business KPIs to develop targeted marketing frameworks.

---

## 📊 4. Dataset Profiles & Metadata

To build this multi-layered analytical engine, the pipeline processes data from two distinct logical horizons, capturing holistic behavioral tracking records for **50,000 active global users**.

### 🔹 4.1 Demographic & Core Subscription Metadata (`netflix_user_behavior_dataset.csv`)
This matrix maps the structural, baseline identity, and financial attributes of the subscriber base before evaluating live platform interactions. It comprises the following critical fields:
* **User Identity Attributes (`user_id`, `gender`, `age`):** Evaluates the core demographic distribution and unique index tracking keys across the global user volume.
* **Geographical Distribution (`country`):** Tracks the user's operational territory, which provides critical boundaries for geo-specific content licensing and local pricing strategies.
* **Financial Tiering (`subscription_type`, `payment_method`):** Identifies the current monetary commitment layer (Basic, Standard, or Premium) alongside the billing mechanism used.
* **Hardware Ecosystem (`primary_device`):** Pinpoints the baseline application portal (Smart TV, Mobile, Desktop, or Tablet) where the consumer initiates streaming.

### 🔹 4.2 Live Consumption & Behavioral Engagement Data
This layer represents the raw input fed into our Machine Learning pipeline. It records active platform usage patterns and customer retention metrics over time:
* **Preference Identification (`favorite_genre`):** Isolates the stream volume concentration across entertainment categories (Sci-Fi, Drama, Comedy, Action, etc.) utilized during the initial SQL extraction phase.
* **Volume Metrics (`avg_watch_time_minutes`, `watch_sessions_per_week`):** Captures temporal consumption density, documenting the average single-session watch span and weekly operational frequency.
* **Content Loyalty Index (`completion_rate`):** Evaluates behavioral drop-off rates by measuring the exact percentage of titles or episodes streamed entirely to completion rather than abandoned mid-way.
* **Attrition Validation (`churned`):** The primary commercial target flag recording subscriber termination states ("Yes" vs. "No"). This field provides the ultimate benchmark to determine the financial risk profile of each generated persona.

---

## 📈 5. Key Insights & Final Personas ($K=4$)

The machine learning pipeline automatically converged into 4 highly stable and balanced user archetypes:

### 🟥 Cluster 0: "The High-Risk Casuals" (Highest Churn Rate)
* **Behavior:** Low average watch times, low completion rates, primarily streaming on portable devices.
* **Strategy:** Aggressive push notifications, personalized re-engagement campaigns, and tactical promotional discounts.

### 🟨 Cluster 1: "The Core Binger Streamers"
* **Behavior:** Highly steady weekly viewing sessions, high completion rates, highly receptive to platform recommendations.
* **Strategy:** Lock into longer-term contractual agreements or family-tier upgrades due to proven baseline loyalty.

### 🟩 Cluster 2: "The Traditional TV Enthusiasts"
* **Behavior:** Moderate weekly frequency but high-fidelity consumption patterns, streaming almost exclusively through Smart TVs.
* **Strategy:** Prioritize premium 4K HDR content licensing and ensure total application stability on television operating systems.

### 🟦 Cluster 3: "The Marathon Content Consumers" (Top Value Segment)
* **Behavior:** Highest average watch time (minutes) and daily platform interactions.
* **Strategy:** Ideal cohort for beta-testing new UI/UX features, early-access content releases, and word-of-mouth referral program rewards.

---

## 🚀 6. How to Run the Project
1. Clone this repository to your local environment or open the notebook directly in Google Colab.
2. Ensure your dataset file (`netflix_user_behavior_dataset.csv`) is placed in your cloud directory or local path.
3. Configure the file paths in the initial cells to point directly to your data source.
4. Select **Runtime -> Run all** to execute the complete end-to-end extraction and clustering pipeline.

---
*Developed as a high-performance portfolio case study showing cross-functional expertise in Data Engineering (SQL), Mathematical Modeling (PCA), and Unsupervised Machine Learning (K-Means).*
