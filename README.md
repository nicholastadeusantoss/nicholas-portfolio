# Data Projects: 

### 1 - Using Natural Language Processing (NLP) to Classify NPS Comments in the Pharmaceutical Retail Sector

![image](https://github.com/nicholastadeusantoss/nicholas-portfolio/assets/57444719/a51ca7f4-7ea3-4711-adf8-004ed3e50775)

The project involved structuring nine main topics to classify recurring issues in over 4,000 monthly comments using Amazon Comprehend, resulting in a 97% accuracy rate, reducing manual workload, enabling monthly tracking of topic volumes, and innovating in the company's Customer Experience sector.

**Problem:** 
- We faced a recurring issue where every month, we had to read over 4,000 comments and classify them. Apart from the time-consuming task of reading and categorizing, we lacked a structured hierarchy of reasons, hindering our ability to track the evolution of customer-reported issues in the comments.

**Solution:**
- The first step I took was to structure nine main topics for which we had enough data to confidently classify as recurring issues. I also drew inspiration from our customer service (SAC) reason hierarchy, considering the volume of inquiries per category. With this in place, I began researching tools and settled on the Amazon Comprehend model.

- During the project planning phase, I had to allocate time for learning how to use the Amazon tool, as I had no prior experience with it. I created a training dataset for the algorithm, grouping keywords by topic that had the highest occurrences in the 2023 comments and were also "unique," meaning they belonged exclusively to one topic.

- With the training dataset, we achieved highly accurate comment classification for new comments, with a 97% correct classification rate.

**Tools:**

- **Amazon Comprehend** for the ML algorithm
- Utilized **Python** with the pandas library
- **Tableau** for dinamic visualization

**Achievements:**
- Reduction in manual comment reading workload (**saving 2 days or 16 hours of work per month**).
- Monthly tracking of topic volumes to measure their evolution.
- **Innovation** in the company's Customer Experience (CX) sector.


### 2 - Enhancing Customer Loyalty and Value Perception in Financial Services: A Comprehensive NPS Analysis


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
