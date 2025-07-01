# Predict Customer Personality to Boost Marketing Campaign Using Machine Learning

## Project Overview

Understanding customer profiles and transactional behaviors is crucial for designing effective product sales strategies. This project utilizes **Machine Learning (K-Means Clustering)** to segment customers for targeted marketing, enabling companies to deliver the right treatment to customers based on their specific challenges, enhancing their experience, improving transaction satisfaction, and ultimately increasing sales performance.

---

## Dataset

- **Source:** `marketing_data.csv`
- Contains:
  - Customer demographic information (Age, Education, Marital Status, Income)
  - Purchasing behavior (product category spending)
  - Website visit and purchase channels
  - Response to marketing campaigns
These datasets simulate realistic employee data for demonstration and learning purposes, including employee demographics, job classifications, salary ranges, and exit details.

> **Source**: Public sample dataset hosted on GitHub  
> [View Dataset on GitHub](https://github.com/denindrap23/Machine-Learning/blob/main/Predict-Customer-Personality-to-boost-marketing-campaign-by-using-Machine-Learning/marketing_campaign_data.csv)

---

## Project Objectives

- To **understand customer profiles and purchasing behavior** for improved marketing strategies.
- To **segment customers using K-Means Clustering** for personalized marketing retargeting.
- To provide actionable recommendations that enhance customer experience and sales performance.

---

## Tools and Libraries

- **Python 3.x**
- `pandas`, `numpy` - Data processing and feature engineering
- `seaborn`, `matplotlib` - Data visualization
- `scikit-learn` - Clustering, PCA, t-SNE, scaling, evaluation

---

## Workflow

### 1. **Data Cleaning & Preprocessing**  
   - Handling missing values.
   - Encoding categorical features (`Marital_Status`, `Education`, etc.).
   - Feature engineering:
     - `Age` (calculated as 2025 - Year_Birth)
     - `Total_Amount_Spent`
     - `Conversion Rate`
   - Scaling numerical features using `StandardScaler` for clustering.

### 2. **Exploratory Data Analysis (EDA)**  
   - Analyzing distributions of `Income`, `Age`, `Total Amount Spent`, and `Conversion Rate`.
   - Analyzing correlations between spending, income, and visit frequency.

### 3. **Data Modelling: Clustering (K-Means)**  
   - Using **Elbow Method** to determine the optimal number of clusters.
   - Applying K-Means clustering and appending cluster labels to the dataset.

### 4. **Model Evaluation**  
   - **Silhouette Score** for cluster validation.
   - **PCA** and **t-SNE** for 2D cluster visualization.

### 5. **Customer Personality Analysis**  
   - Analyzing each cluster’s profile:
     - Low Spender
     - Mid Spender
     - High Spender
     - Risk of Churn
   - Reviewing spending, income, web visits, and conversion rates per cluster.

### 6. **Recommendations & Potential Impact**  
   - Developing targeted marketing strategies for each customer segment.

---

## Key Visualizations

- **EDA:**
  - Distribution plots of spending, income, and age.
  - Scatterplots and jointplots (`Income` vs `Total Spent`, `Age` vs `Conversion Rate`).
- **Clustering:**
  - Elbow method plots for selecting `k`.
  - PCA and t-SNE visualizations for cluster distribution.
  - Boxplots of income, spending, and web visits per cluster.

---

## Insights

- **High Spender:** High income and spending; ideal for loyalty programs.
- **Mid Spender:** Moderate spending; potential for upselling through targeted promotions.
- **Low Spender:** Low spending; requires educational campaigns to increase engagement.
- **Risk of Churn:** Moderate-to-high spending but low visit frequency; needs retention-focused treatment.

---

## Business Impact

- Enables **personalized marketing retargeting** based on accurate customer segmentation.  
- Improves customer satisfaction and loyalty.  
- Reduces churn risk for high-potential customers.  
- Drives sales growth through focused marketing strategies.
