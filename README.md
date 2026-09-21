# 📊 Olist E-Commerce Data Analysis & Forecasting

An end-to-end data analytics and predictive modeling project utilizing the Olist e-commerce dataset. This repository integrates an interactive PowerBI dashboard with descriptive, diagnostic, and predictive methodologies—specifically **RFM Segmentation, K-Means Clustering, NLP Topic Modeling, and SARIMAX Time-Series Forecasting**.

---

## 📂 Repository Structure

* **`Diagnostic & Predictive Analysis (RFM K-means + NLP Topic Model + SARIMAX)/`** - Contains all Jupyter Notebooks, raw data pipelines, and python visualization outputs.
* **`PowerBI/`** - Contains the compiled `.pbix` dashboard application files.
* **`Project_Outline.pdf`** - High-level functional specification and pipeline overview.
* **`Data Collection Methodology.pdf`** - Details regarding the structured schema extraction mapping process.

---

## 📈 Diagnostic Analysis: RFM K-Means Clustering

To optimize marketing spend and retention strategies, customer purchasing behaviors were segmented using an unsupervised K-Means model scoring three core operational vectors: **Recency**, **Frequency**, and **Monetary Value**. 

Below is the automated summary distribution showcasing the volume share and revenue performance across the identified distinct consumer cohorts:

<!-- Note: If your image file name differs or is saved in a subfolder, adjust the path within the parenthesis accordingly -->
![K-Means Clustering Diagnostic Summary Table](Diagnostic%20%26%20Predictive%20Analysis%20%28RFM%20K-means%20%2B%20NLP%20Topic%20Model%20%2B%20SARIMAX%29/RFM%20K-means/Olist_KMeans_Diagnostic_Table_Final.png)

### 💡 Core Cohort Insights
* **Cluster 1 & 3 (High-Value Patrons)**: Represents the top tier of customer spenders, exhibiting highest average monetary value (~\$316 and ~\$296 respectively). While accounting for less than **3%** of the cumulative customer footprint combined, their transaction weights yield disproportionate revenue momentum.
* **Cluster 0 (Mainstream Active Base)**: Captures **43.20%** of the user volume. This represents recent, stable shoppers providing the bedrock of long-term operational health, contributing a staggering **72.51%** share of aggregate business revenues.
* **Cluster 2 (Dormant / Low-Value Trailing)**: Accounts for the single largest bulk segment at **53.77%** of the database volume, yet brings in only **21.85%** of revenue with the lowest monetary average (\$67.26). Highly susceptible to churn; requires low-cost automated re-engagement funnels.

---

## 🛠️ Getting Started & Dependencies

To execute the python diagnostic pipelines and regenerate the reporting summary matrix assets locally, ensure your virtual environment contains the necessary scientific computing extensions:

### Prerequisites
* Python 3.8+
* Pandas
* Matplotlib
* Scikit-Learn

### Execution
Run the baseline modeling script from your terminal:
```bash
python "Diagnostic & Predictive Analysis (RFM K-means + NLP Topic Model + SARIMAX)/RFM K-means/RFM_Kmeans_Analysis.py"
```
