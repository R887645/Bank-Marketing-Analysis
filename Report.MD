# Introduction

I revisited my bank marketing project, originally built in Power BI nearly two years ago. The dashboard was designed to evaluate subscription campaign performance and client segmentation, but at the time, it lacked the clarity, structure, and interactivity needed to drive strategic decision‑making.

Rebuilding the project allowed me to apply advanced skills in data modeling, DAX analysis, wireframing, and interactive dashboard design. The result is a two‑page dashboard that separates Campaign Performance from Client Segmentation & Strategic Insights, providing stakeholders with a cleaner narrative and actionable insights.

---

## Business Problem

Despite running multiple marketing campaigns over several years, the bank lacked a structured analytics system to evaluate performance and identify high-value customer segments effectively.

Key business questions included:

- How effective are marketing campaigns over time?  
- Which contact channels generate the best conversions?  
- What customer segments deliver the highest value?  
- Where are the biggest opportunities for future targeting?

This project addresses these gaps by providing a clean, interactive analytics solution built entirely in Power BI.

---

## Project Scope

The project followed a complete analytics workflow:

- Data collection and exploration  
- Data preparation and Data cleaning  
- Data Cleaning (Standardization of fields and categories)
- Data modeling using a star schema  
- Creation of DAX measures  
- Dashboard wireframing in PowerPoint  
- Report development in Power BI  
- Interactivity enhancements (bookmarks, slicers, navigation)

---

## Data Overview

### Datasets Used

**Campaign Data**
- Contact method  
- Call duration  
- Subscription outcome  
- Full Date

**Client Data**
- Age  
- Job category  
- Marital status  
- Education level  
- Account balance  

**Performance Metrics**
- Contact volume  
- Subscription counts  
- Monthly and yearly trends  

---

## Data Preparation

The following preparation steps were completed:

- Creation of a proper date column for time intelligence  
- Cleaning and standardization of categorical fields of about 
- Normalization of job and education categories using a list in Power BI 
- Removal of inconsistencies and formatting issues  
- Creation of calculated metrics and segmentation logic  
- Client grouping based on balance and engagement  

![Bank_Power_Query](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Bank_PowerQuery.png?raw=true)

---

## Data Modeling

A structured star schema was implemented:

- Central Fact Table: Subscriptions  
- Supporting Dimension Table:  
  - Calendar Date Table

This model enabled efficient filtering, accurate aggregations, and seamless time-based analysis.

![Bank_Data Modelling](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Bank%20Data%20Modelling.png?raw=true)


---

## DAX Measures Implemented

### Anchor Metrics

1. Total Contacts  
2. Total Subscriptions  
3. Subscription Rate  
4. Average Call Duration  
5. Subscription Rate
6. Total Clients Balance

### Time Intelligence Metrics

5. Month-over-Month Subscription Growth  
6. Year-over-Year Subscription Growth 
7. Previous-Month Subscriptions
8. Previous-Year Subscriptions

![Bank_DAX_Measure](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Time%20intelligence%20DAX_bank.png?raw=true)  ![Bank_DAX_Measure](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Anchor%20measure_bank.png?raw=true)



These measures powered KPI cards, trend analysis, and comparative insights across the dashboard.

---

## Dashboard Design Process

### Wireframe Development

Before building the report, a structured wireframe was created in PowerPoint to define:

- Page objectives  
- KPI placement  
- Chart selection  
- Navigation flow  
- User interaction design  

![Bank_Wireframe](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/2026_%20Dashboard_Wireframes.png?raw=true)
![Bank_Wireframe](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/2026_%20Dashboard_Wireframes_2.png?raw=true)


This approach ensured a business-focused and uncluttered final dashboard.

---

## Dashboard Breakdown

### Page 1 – Campaign Performance Overview

**Focus:** High-level performance monitoring and trend analysis

Key analytical components include:

- Total contacts and subscriptions  
- Subscription rate trends  
- Monthly and yearly performance comparison  
- Conversion analysis by duration  
- Outcome distribution  
- Performance across multiple years 

![Bank_campaign_performance](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Campaign%20Performance.png?raw=true)

**Strategic Insights**

- The campaign reached 5,000 contacts, with an average call duration of 263.96 seconds. Subscription rate stood at 11.52%, translating into 521 total subscriptions.

- Monthly growth analysis revealed volatility, with September recording the highest growth (+31.71%) and March the lowest (-29.41%).

- Year-over-year subscriptions grew by +9.45%, signaling long-term improvement.

- A combo chart comparing average duration and subscription rate showed that longer conversations correlated with higher conversions, reinforcing the importance of engagement quality.

- A pie chart revealed that 88.48% of contacts did not subscribe, highlighting room for strategic improvement.

- Yearly subscription performance from 2015 to 2024 showed peaks in 2016 and 2022, with more modest results in other years.


---

### Page 2 – Client Segmentation & Strategic Insights

**Focus:** Understanding customer behavior and value contribution

Key analyses include:

- Subscriptions by marital status  
- Subscriptions by education level  
- Balance-based client segmentation  
- Job category performance  
- Scatter plot analysis of balance vs engagement  

![Bank_client_segmentation](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Clients%20segmentation%20Insights.png?raw=true)


**Strategic Insights**

- Marital status analysis revealed that married clients led with 221 subscriptions, followed by singles and divorced clients.

- Education level analysis showed that secondary and tertiary education groups dominated subscriptions, while primary and unknown categories lagged.

- Balance segmentation provided critical strategic insight: although the low balance group had the highest subscription count (269), the high balance group contributed the most monetary value (€3.0M).

- Job category analysis highlighted the bottom five performers — students, entrepreneurs, housemaids, unemployed, and unknown — all with low subscription counts.

- A scatter plot of client balance versus subscription duration by job revealed which job categories were both wealthy and engaged, offering a roadmap for targeted marketing.

**Interactivity Features**

- Home page created for flexibility
- Year and job category slicers across both pages
- Bookmark-based reset functionality across the two pages
- Page navigation buttons across both pages 
- Dynamic KPIs and visuals  
![Bank_Data Modelling](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Bank_Bookmark.png?raw=true) ![Bank_list](https://github.com/R887645/Bank-Marketing-Analysis/blob/main/Bank_list_creation.png?raw=true)


**[View the Full Interactive Dashboard Here](https://app.powerbi.com/view?r=eyJrIjoiNTYzZmMxZGMtNTI4Ni00MDI2LWJjNGItNmJmY2FiMDk3YTk2IiwidCI6ImZjY2Y0MmRmLTE2ZDktNGU4Ny1hNmUwLWU0OTYyMjAxN2Y3NCJ9)**

---

## Business Recommendations

As a Marketing Data Analyst, I would recommend that the bank:

- Target high-balance clients with personalized campaigns, as they yield the most financial value despite lower volume.

- Optimize contact methods, cellular leads in volume, but telephone offers deeper engagement.

- Refine messaging for low-performing job categories, or consider excluding them from future campaigns.

- Treat duration as a proxy for engagement, since longer calls tend to convert better.

- Prioritize secondary and tertiary education groups, as they show strong subscription behavior.

---

## Tools & Technologies

- Power BI  
- Power Query  
- DAX  
- Microsoft PowerPoint (Wireframing)  
- Data Modeling (Star Schema Design)

---

## Challenges Encountered
During the course of this analysis, I faced a few technical and design challenges that ultimately strengthened the dashboard:

- **Date Column Import:** Initially, the dataset lacked a proper date column, which made time intelligence measures difficult. I resolved this by restructuring the data and introducing a full date dimension, enabling accurate MoM and YoY analysis.

- **Bookmark Interactivity:** Implementing bookmarks with reset functionality and smooth navigation was complex at first. After several iterations, I successfully integrated them, enhancing the dashboard’s usability and stakeholder experience.

Overcoming these challenges not only improved the dashboard but also deepened my expertise in Power BI’s advanced features.

## Conclusion

This project demonstrates my expertise in marketing analytics, data modeling, DAX analysis, wireframing, and interactive dashboard design. 
By revisiting and rebuilding the dashboard after almost 2 years, I transformed a static report into a dynamic analytical tool that separates performance from segmentation, helping stakeholders make smarter, data-driven decisions.

I am open to collaborating on projects where data storytelling, campaign analysis, and client segmentation can drive meaningful business outcomes.                                                                                                                 

---

### “The data didn’t change. The analysis did.”

---

### Author  
(Abdu-Azeez Rofiah Kehinde) 
Marketing Data Analyst | Business Intelligence Professional | [LinkedIn](https://www.linkedin.com/in/rofiah-abdul-azeez/) 
