# Data Science Projects: 

### 1 - Project developed at a Leading Pharmaceutical Retailer in Brazil - Using Natural Language Processing (NLP) to Classify NPS Comments

The project involved structuring nine main topics to classify recurring issues in over 4,000 monthly comments using Amazon Comprehend, resulting in a 79% accuracy rate, reducing manual workload, enabling monthly tracking of topic volumes, and innovating in the company's Customer Experience sector.

**Problem:** 
- We faced a recurring issue where every month, we had to read over 4,000 comments and classify them. Apart from the time-consuming task of reading and categorizing, we lacked a structured hierarchy of reasons, hindering our ability to track the evolution of customer-reported issues in the comments.

**Solution:**
- **The first step** I took was to structure **nine main topics** for which we had enough **data to confidently classify** as recurring issues. I also drew inspiration from our customer service (SAC) reason hierarchy, considering the volume of inquiries per category. With this in place, I began researching **tools** and settled on the **Amazon Comprehend model**.

- During the **project planning phase**, I had to allocate time for learning how to use the Amazon tool, as I had **no prior experience** with it. I created a training dataset for the algorithm, grouping keywords by topic that had the highest occurrences in the 2023 comments and were also "unique," meaning they belonged exclusively to one topic.

- I used Python _(pandas, boto3)_ to prepare the training dataset, preprocess the comments, and interact with the **Amazon Comprehend API**. Additionally, I queried and processed the original comment data using **SQL** to extract relevant subsets from the customer feedback database.

- With the training dataset, we achieved **highly accurate comment classification** for new comments, **with a 79% correct classification rate.**

**Tools:**

- **Amazon Comprehend** for the ML algorithm
- **Python** with **pandas**, **boto3**, and **NumPy** for data processing and automation
- **Looker** for dinamic visualization

**Achievements:**
- Reduction in manual comment reading workload (**saving 2 days or 16 hours of work per month**).
- Monthly tracking of topic volumes to measure their evolution.
- **Innovation** in the company's Customer Experience (CX) sector.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### 2 - Project developed at a Global Footwear Retailer - Building a Unified Customer Intelligence Platform (C.L.I.P)

The project involved creating a customer-centric data infrastructure within Databricks, integrating multiple data sources to generate a unified view of the customer journey. This foundation enabled the development of advanced models, such as customer **churn prediction**, **product recommendation** _(Next Best Offer)_, **optimal timing for offers**, and **predictive modeling** of product and collection performance — enhancing strategic decision-making in marketing and merchandising.

**Problem:** 

- We had **fragmented customer data** across various systems, which made it difficult to understand customer behavior in a unified and scalable way. There was no reliable **data structure to support machine learning** use cases like churn prediction, recommendation, or product performance forecasting. Decisions in marketing and product development were made without **predictive insights** based on customer history or product features.

**Solution:**

I designed and built the entire **data pipeline using Databricks**, ingesting data from **CRM, e-commerce, retail systems, and transactional databases**. Used **PySpark** and **SQL** _(Spark SQL)_ to perform data transformations and create curated tables. Developed a centralized customer table that combined relevant behavioral and demographic information to represent the full customer journey.

On top of this foundation, I developed a set of machine learning models using Python:

  - **Customer segmentation** via **K-Means** clustering _(with scikit-learn)_, highlighting patterns and identifying potential churn risks.

  - **Churn prediction** model using **logistic regression** and **tree-based models**, trained on behavioral and transactional history.

  - **Next Best Product** model to recommend **personalized product offers**, based on purchase history and collaborative filtering.
    - I implemented a collaborative filtering algorithm using **alternating least squares (ALS)** from **pyspark.ml.recommendation**.

  - **Next Best Time to Offer**, suggesting the optimal timing to approach each customer based on recency-frequency patterns.
    - I applied **time-series feature** extraction from transaction history _(RFM: Recency, Frequency, Monetary)_ and used **binary classification models** _(logistic regression and gradient boosting with XGBoost)_ to predict the **probability of engagement** at different time windows. The model allowed for personalized timing of outreach, increasing the likelihood of conversion.

  - **Product performance prediction** using regression models _(e.g., XGBoost)_, **forecasting sales potential** for new shoes based on features such as **material, color, and category**.
    - I created a **supervised regression pipeline** using **tree-based algorithms** _(XGBoost, Random Forest)_ to estimate the **sales performance of new SKUs before launch**. Input features included product attributes _(e.g., silhouette, material, heel height)_, historical performance of similar items, and collection context.

  - **Collection performance prediction**, aggregating product-level insights to evaluate launch potential **before go-to-market.**
    - Built a second-level model that **aggregated predictions from individual SKUs** _(from the previous model)_, along with **collection-level attributes** _(theme, seasonality, brand fit)_, **to estimate overall collection sales uplift**. This helped merchandising teams **simulate different launch scenarios** and **optimize** the product mix. 


**Tools:**

 - **Databricks** for data integration and processing _(PySpark and Delta Lake)_

 - **Python** with pandas, scikit-learn, XGBoost, matplotlib, and MLflow for model tracking

 - **Power BI** for business-oriented dashboards and visualization

**Achievements:**

- Built a **customer 360º view**, enabling insights across marketing, CRM, and product teams.

- Enabled **early churn detection** and more effective retention strategies.

- Developed a dynamic **recommendation framework** that aligned products and timing to customer behavior.

- Empowered **data-driven product development**, reducing risk and increasing **assertiveness** in collection planning and inventory management.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

### Study Project - Enhancing Customer Loyalty and Value Perception in Financial Services: A Comprehensive NPS Analysis

![image](https://github.com/nicholastadeusantoss/nicholas-portfolio/assets/57444719/a51ca7f4-7ea3-4711-adf8-004ed3e50775)

As part of my professional portfolio, I undertook an analysis project focused on Net Promoter Score (NPS). This project demonstrated my commitment to placing the client's perspective at the forefront of my work.

**Objectives:**
- Calculate the NPS for our customer base.
- Identify the market segment with the highest NPS.
- Compare our NPS to industry benchmarks in the financial services sector.
- Explore any potential correlation between weekdays and NPS scores.
- Analyze whether clients who responded multiple times experienced an improvement in their perception of value.

**Solution:**
I began by defining clear objectives and breaking them down into manageable steps. These steps included data preparation, NPS calculation, market analysis, correlation analysis, and examining changes in client perceptions over time. 

**Tools:**
- Utilized **Python** and libraries such as **pandas**, **NumPy**, and **scikit-learn** for data - analysis and statistical modeling.
- Created data visualizations using **Tableau** to present project findings.
- Maintained project documentation and analysis in a **Kaggle** notebook.

**Links:**
- [Link to Kaggle Notebook](https://www.kaggle.com/code/nicholastadeu/nps-analysis-project)
- [Link to Tableau Dashboard](https://public.tableau.com/views/NPSAnalysis_16957541272620/NPSOverview?%253Alanguage=pt-BR&publish=yes&%253Adisplay_count=n&%253Aorigin=viz_share_link)
- [Link to LinkedIn Article](https://www.linkedin.com/pulse/enhancing-customer-loyalty-value-perception-financial-nicholas-tadeu/)
