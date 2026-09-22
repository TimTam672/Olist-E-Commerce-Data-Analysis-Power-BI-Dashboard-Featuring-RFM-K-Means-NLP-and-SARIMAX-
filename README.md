### 📂 Project Directory Structure

```text
Olist-E-Commerce-Data-Analysis/
├── Diagnostic & Predictive Analysis (RFM K-means + NLP Topic Model + SARIMAX)/
│   ├── NLP Topic Model/
│   ├── RFM K-means/
│   ├── SARIMAX/
│   └── Diagnostic & Predictive Analysis PowerPoint.pptx
├── PowerBI/
├── Data Collection Methodology.pdf
├── Project_Outline.pdf
└── README.md
```

#### 📁 Repository Component Breakdown
* **` NLP Topic Model/`** – Contains Jupyter Notebook scripts, datasets, and output charts/tables.
* **` RFM K-means/`** – Contains Jupyter Notebook scripts, datasets, and output charts/tables.
* **` SARIMAX/`** – Contains Jupyter Notebook scripts, datasets, and output charts/tables.
* **` Diagnostic & Predictive Analysis PowerPoint.pptx`** – Comprehensive slide deck summarizing key project findings and executive presentation deliverables.
* **` PowerBI/`** – Houses compiled interactive dashboard application files (`.pbix`) alongside high-resolution interface screenshots.
* **` Project_Outline.pdf`** – Comprehensive project blueprint documenting precise data cleaning pipelines and the baseline Entity-Relationship Diagram (ERD).
* **` Data Collection Methodology.pdf`** – Comprehensive documentation outlining the data collection methodology, ethical considerations, and core limitations of the dataset.

## 📊 Interactive Power BI Dashboards
A 3-page interactive Power BI Dashboard to evaluate Sales,
Logistics, Product Performance, and Customer Loyalty across a 15.49M BRL revenue
ecosystem (100k+ records).

<!-- PowerBI Dashboard -->
![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/8dd34751100f766e6f00c5f98d4859001575e2b5/PowerBI/Sales%20%26%20Logistics.png)

![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/268303a75f7228182adf85e409647b71c98a92f6/PowerBI/Product%20Performance%20%26%20Customer%20Sentinment%20Analysis.png)

![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/8eba5989621e8c1bb8fd03057ec9d5ed5ae99e63/PowerBI/Customer%20Loyalty%20%26%20Seller%20Ecosystem.png)

## 🔍 Key Business Insights & Analytical Findings (PowerBI-based)
A rigorous diagnostic audit of the Olist e-commerce database revealed several critical operational trends and strategic growth challenges across consumer segments, merchant behaviors, and category lifecycles:

### 💳 Consumer Purchasing Behaviors & Experience
* **Payment & Timing Preferences**: Transaction data indicates that customers heavily prefer shopping on **weekdays** and overwhelmingly complete purchases utilizing **credit cards** as their primary payment mechanism.
* **The High-Value Experience Friction**: A critical paradox was identified where **high-spending customer cohorts report significantly lower satisfaction scores (worse user experiences)** compared to baseline spenders. This highlights a pressing need to optimize the premium delivery and customer service funnel.

### 📦 Category Revenue Hierarchy
Aggregate business revenues follow a distinct category structural distribution, led by home goods and trailing into media supplies:
`Home & Living` > `Lifestyle` > `Tech & Gadgets` > `Media & Essentials`

### 🗺️ Geographic Retention & Supply Dynamics
* **The Retention Divide**: **Coastal regions exhibit noticeably lower customer retention rates** compared to interior markets. Spatial analysis indicates this churn is primarily driven by intense localized market competition.
* **Growth Engine Imbalance**: The platform currently faces an over-reliance on **continuous new customer acquisition** to sustain transaction volumes, rather than relying on robust organic user retention.

### 🏪 Merchant Performance & Scaling Friction
* **Mature Seller Expansion**: The volume of **stable, long-tenure merchant accounts ($3+$ months)** operating on the Olist marketplace is steadily expanding, establishing a reliable ecosystem backbone.
* **The Scale vs. Quality Dilemma**: A strong inverse relationship exists between transaction volumes and service metrics. Merchants managing **high sales volumes face severe structural difficulties in maintaining peak service quality and high ratings**, pointing to a need for better seller logistics infrastructure.

<!-- Diagnostic & Predictive Data Analytics -->

## Customer Segmentation Analysis using RFM + K-Means Clustering

This repository contains the data preprocessing, model selection, and strategic growth framework for our customer segmentation engine, utilizing an **RFM (Recency, Frequency, Monetary) model** combined with **K-Means Clustering**.

---

### 🛠️ Data Preprocessing & Methodology

1. **RFM Transformation**: Raw transaction data was tidied into Recency, Frequency, and Monetary metrics and standardized into a **1–4 scale** using statistical quartiles.
2. **Recency Scoring**: Scored inversely—rewarding recent activity—to surface the most engaged, highest-value customers.
3. **Feature Engineering**: 
   * **Log Transformation**: Applied to mitigate heavy monetary skewness.
   * **Standardization**: Harmonized disparate RFM scales to ensure unbiased distance calculations for the K-Means algorithm.
4. **Model Optimization**: The **Elbow Method** identified **K=4** as the optimal cluster count, achieving the best trade-off between model complexity and Within-Cluster Sum of Squares (WCSS) reduction.

---

### 📈 Key Insights & Strategic Diagnostics

* **New-Customer Dependence**: Our current growth relies heavily on continuous acquisition rather than repeat purchases. This is a structurally unsustainable model.
* **The Loyalty Paradox**: High-value spenders (**Cluster 1**) are not being retained. This creates a severe revenue leak that actively offsets our acquisition gains.
* **Strategic Priority**: Fixing the post-purchase experience for **Cluster 1** high-spenders is the fastest path to transforming transactional cycles into a sustainable loyalty ecosystem.

---

### 🎯 Targeted Retention & Growth Programs

#### 📦 New User Program (Clusters 0 & 2)
* **Tactics**: Introductory incentives and welcome bonuses.
* **Goal**: Convert one-time new customers into repeat buyers.

#### 🛡️ Stable Core Program (Cluster 3)
* **Tactics**: Exclusive retention programs and tier-based loyalty benefits.
* **Goal**: Maintain and protect high-value customer engagement.

#### 💎 Platinum Tier Program (Top 0.8% | RFM Score 11–12)
* **Tactics**: Premium benefits including free shipping and priority customer support.
* **Goal**: Stabilize our most profitable segment and maximize Customer Lifetime Value (CLV).

![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/RFM%20K-means/Elbow.png)

![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/RFM%20K-means/Olist_KMeans_Diagnostic_Table_Final.png)

## 🛠️ Pipeline Methodology & Technical Stack

### 1. Neural Translation
* **Model**: Facebook's **NLLB-200**
* **Application**: Normalized international customer feedback by converting non-English text (e.g., Portuguese) to English while preserving semantic nuances.

### 2. Rigorous Text Preprocessing
* **Noise Reductions**: Stripped URLs, punctuation, digits, and nonsensical strings.
* **Feature Pruning**: Eliminated standard stop words, high-frequency baseline terms, and ultra-rare outliers.
* **Normalization**: Handled emoticon-to-text conversion followed by strict stemming and lemmatization.

### 3. Quality Audit & Validation
* **Semantic Evaluation**: Utilized **LaBSE (Language-Agnostic BERT Sentence Embedding)**.
* **Benchmark**: Achieved a semantic similarity score of **0.657**, validating that core contextual meaning remained intact post-translation and preprocessing.

### 4. Advanced Refinement & Topic Discovery
* **Vectorization**: Integrated `CountVectorizer` to capture critical multi-word phrases and n-grams.
* **Topic Modeling**: Executed a **BERTopic** pipeline optimized with `KeyBERTInspired` embeddings to distill **9,869 raw reviews** down to **4 Critical Themes** (accounting for 5,619 high-impact reviews).

---

## 📊 Structural Matrix: Themes by Category

| Core Theme | Home & Living | Tech & Gadgets | Media & Essentials | Lifestyle |
| :--- | :---: | :---: | :---: | :---: |
| **Product Specification** | 🔴 Discrepancies | | | |
| **Installation Issues** | | 🔴 Poor Manuals | | |
| **Customer Anxiety** | | | 🔴 Poor Tracking | 🔴 Poor Tracking |
| **Fulfillment & Returns** | ⚠️ High Impact | ⚠️ High Impact | ⚠️ High Impact | ⚠️ High Impact |

---

## 🎯 NLP Solutions & Operational Interventions

### 📋 1. Proactive Logistics & Dispute Management
* **Target Objective**: Eliminate systemic **Customer Anxiety** by addressing both tactical ("Action") and emotional ("Psychological") bottlenecks.
* **Interventions**:
  * Deploy **Live Customer Service** frameworks to mediate and de-escalate transaction disputes in real-time.
  * Construct automated monitoring triggers for orders with extreme lead times, backed by **strict penalties** for underperforming third-party sellers.
* **Expected Result**: Minimal operational friction and a measurable drop in anxiety-driven customer support tickets.

### 🛡️ 2. Product Integrity & Information Standards
* **Target Objective**: Systematically eliminate **Specification Discrepancies** and **Installation Failures**.
* **Interventions**:
  * Execute a platform-wide **specification audit** to purge fraudulent or inaccurate product sheets.
  * Enforce a **Mandatory Digital Documentation** standard, requiring merchants to supply localized video tutorials or interactive, enhanced digital manuals.
* **Expected Result**: Drastic reduction in avoidable post-purchase returns and an elevated initial unboxing experience.



![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/NLP%20Topic%20Model/WordCloud.png)

![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/NLP%20Topic%20Model/Customer%20Pain%20Point%20Diagnosis%20Matrix.png)




![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/SARIMAX/Olist_SARIMAX_Forecast_Charts.png)

![image alt](https://github.com/TimTam672/Olist-E-Commerce-Data-Analysis-Power-BI-Dashboard-Featuring-RFM-K-Means-NLP-and-SARIMAX-/blob/3540e95101ae8eb3fb4d74e0a722d65d6970aff3/Diagnostic%20%26%20Predictive%20Analysis%20(RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX)/SARIMAX/Olist_Strategic_Analysis_Table.png)
