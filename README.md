## 📌 Project Overview
This project focuses on the end-to-end lifecycle of a healthcare dataset—from raw, unstructured data to a high-fidelity analytical dashboard. The core challenge involved a dataset of 54,000+ hospital records containing significant naming inconsistencies and structural errors.

This synthetic healthcare dataset sourced from [Kaggle](https://www.kaggle.com/) which provides a foundation for my analysis, its contains a detail of patient information such as blood type, medical condition, admission type etc. I answered seven most critical questions such as the top 8 doctors by revenue, average length of stay by admission type, which admission type is more expensive and more.

## The Questions
In this project, I tasked myself with answering these seven most critical questions to help the department understand what happened and what should be the next decisions.

1. Top 8 doctors by revenue
2. Total billing by insurance provider
3. Which admission type is more expensive
4. Top 8 hospitals with the highest revenue
5. Average length of stay by admission type
6. Monthly admission trend
7. Which month generated the most revenue

## Tools I Used
During the analysis, I explored the power of a varies of analytical tools:

- **Excel:** Used for basic cleaning and removing of duplicates
  
- **Power Query:** I harnessed the power of this tool by applying deep cleaning on the data like replacing missing values, converting DATE column from text to date, and helped me ordered hospitals names from "Sons and Miller" to "Miller and Sons". I further used this tool to create four different tables which include the Facts Table and three dimensional tables namely, Doctor Table, Hospital Table, and Insurance Table. This way, we can avoid chocking all the data into one table and make the visualization process easier.
  
- **Power BI:** My go-to tool for outstanding visualizations and creating executive-ready dashboards. Its also helped me established relationship among the three dimensional tables and the Facts Table, by connecting these three dimensional tables to the main table which is the Facts Table, will help us reduce noise and visualize our data with ease.

### Data Preparation & and Cleanup
This section demonstrate the steps taken to prepare the data for analysis, ensuring accuracy and usability

### Import and Clean up Data
I began by importing the dataset into excel and use the necessary functions, followed by initial data cleaning task to ensure usability

## Q1 Who are The Top 8 Doctors by Revenue?
A horizontal bar chart was selected for the "Top 8 Doctors" visual to prioritize categorical readability and ranking efficiency. By orienting the labels horizontally, we ensure that full names are legible without truncation. The descending sort order provides an immediate "leaderboard" view, allowing stakeholders to compare revenue performance across the top tier of medical staff with minimal cognitive effort.

## Visual

![top_8_doctors_By_revenue](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Top_8_Doctors.png)

*A clustered bar chart showing the top 8 doctors by revenue*

## Insight
**Identifying Revenue Drivers:**
The visual shows that revenue is relatively evenly distributed among the top tier of performers. There is no "superstar" doctor significantly outperforming the rest, the gap between the top performer, Jessica Williams ($80K), and the eighth, Kimberly Gonzalez ($59K), is only $21K. This suggests a healthy, balanced contribution across the lead medical staff rather than a dependency on a single individual.


## Q2 Total Billing by Insurance Provider
I chose a column chart here because it effectively highlights the magnitude of billing for each provider while providing a necessary visual break from the horizontal rankings elsewhere on the page. It allows us to immediately see that while Cigna leads at $9.9M, the market is highly competitive and evenly split across all five providers, with less than a $1M spread between the top and bottom.

## Visual

![top billing by insurance provider](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Top%20billing%20by%20insurance.png)

*This column bar chart is showing us the total billing by insurance provider*

## Insight
Analyzing the Total Billing by Insurance Provider, reveals a specific narrative regarding the hospital's financial ecosystem:

**Market Equilibrium:** The most striking insight is the high level of competition and balance among providers. There is no single dominant payer; instead, the revenue is distributed almost equally across all five major companies.

**Cigna as the Lead Payer:** While the field is crowded, Cigna represents the largest individual revenue stream at $9.9M. This indicates that Cigna is a primary strategic partner for the hospital’s billing department.

## Q3 Which Admission Type is More Expensive
A horizontal bar chart was selected for this comparison to optimize for rapid scanning and ranking. Since the goal was to identify the most expensive admission type, the descending sort order and horizontal labels provide the most intuitive 'leaderboard' experience for the stakeholder.

## Visual
![which admission type is more expensive](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Which%20admission%20type%20most%20expensive.png)

*A horizontal bar chart showing the most expensive admission type*

## Insight
**Elective Procedures as the Primary Revenue Driver:** Elective admissions are the most expensive category, generating $16.2M. This indicates that scheduled procedures (like surgeries or specialized treatments) are a higher financial priority for the hospital than emergency or urgent care.

**Marginal Difference Between Urgent and Emergency:** There is a relatively small gap between Urgent ($15.3M) and Emergency ($14.9M) billing. This suggests that while elective care is the leader, the hospital maintains a very high and consistent volume of non-scheduled, high-acuity care that nearly matches the revenue of the elective department.

## Q4 What are The Top 8 Hospitals by Revenue
For the Top 8 Hospitals by Revenue visual, the horizontal bar chart remains the optimal choice

## Visual
![top 8 hospitals by revenue](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Top%208%20hospitals.png)

*A horizontal bar chart showing the top 8 hospitals by revenue*

## Insight
**Significant Performance "Step-Down":** There is a noticeable "cliff" or drop-off in revenue after the top three. While Williams Inc generated $116K, the fourth-ranked facility, Thompson PLC, drops to $98K—a significant 15% decrease. This indicates a distinct gap between the "high-tier" and "mid-tier" hospitals.

## Q5 What are The Average Length of Stay by Admission Type?
For the Average Length of Stay by Admission Type visual, a column bar chart was chosen to highlight volume and facilitate a quick comparative analysis across categories.

## Visual
![what are the average length of stay](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Average%20length%20of%20stay.png)

*A column bar chart demonstrating the average length of stay by admission type*

## Insight
- **Elective Stays are Longest:** Surprisingly, Elective admissions have the highest average length of stay at 15.6 days. This suggests that scheduled procedures at these facilities may involve complex recovery periods or intensive post-operative care.

- **Emergency vs. Urgent Parity:** There is a very narrow margin between Emergency (15.3 days) and Urgent (14.6 days) admissions. This indicates that regardless of how a patient enters the system (immediate emergency vs. pressing urgency), the clinical pathway and recovery time remain relatively consistent.

## Q6 Monthly Admission Trends
I used line chart to plot the monthly admission trends for better insights

## Visual
![monthly admission trends](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Monthly%20admission%20trends.png)

*A line chart admission trend by month*

## Insight
**Extreme Seasonal Dip in February:** The most significant insight is the sharp decline in February, where admissions drop to their lowest point of 142. This could indicate a shorter month effect or a specific seasonal trend in hospital availability.

**Plateau Performance:** The hospital hits a consistent "ceiling" of 155 admissions in multiple months (January, March, May, July, August, October, and December), suggesting a maximum capacity or a standard operational target.

## Q7 Year-to-Date Revenue Trend
**Continuous Progression:** Line charts are the gold standard for time-series data. Unlike bars, which emphasize individual totals, a line emphasizes the movement and relationship between consecutive months.

## Visual
![year-to-date revenue trend](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/monthly_revenue_trend.png)

*A line chart showing year-to-date revenue trend*

## Insight
**Peak Performance in October:** The hospital achieved its highest monthly revenue in October at $4.28M. This serves as the primary benchmark for peak operational capacity during the year.

**Initial Q1 Volatility:** The year began with a strong January ($4.18M), followed by a significant dip in February and a recovery in March. This suggests a highly variable start to the fiscal year.

**Q2 Low Point:** Revenue bottomed out in April ($3.55M), representing the lowest financial point in the dataset. Identifying the cause of this dip (e.g., lower elective surgery volume) would be a key diagnostic priority.

**Steady Mid-Year Recovery:** Following the April low, the hospital saw a consistent "wave" of recovery through the summer months, maintaining a range between $3.78M and $3.93M.

**Year-End Decline:** After the October peak, revenue showed a steady downward trend, ending the year in December at $3.63M, which is nearly $1M lower than the peak two months prior.

## What I Learned
Here are few knowledge that I gained from this project:

**Data Cleaning:** Through out this project, I learned that data cleaning is the foundation of every analysis. In order to get an accurate result, the data must be clean, and organize. And I learnt that from the very beginning of this project.

**Power Query:** Due to the inconsistent entries and missing values of this dataset, I used advance features in power query to professionally handle these errors which helped me brush up on my skills.

**Dax Formulas:** After cleaning and standardizing the dataset, I imported it into Power BI and wrote some dax functions to calculate all the metrics including  total revenue, length of stay, and average length of stay. This really helped me improve my skill on calculating metrics by writing dax code.

**Visualization:** As you all know a cleaned and organized data cannot provide any readable insight. And that's where visualization comes in, by visualizing this data shows that I have immensely upgraded my skills when it comes to this part of data analytics.

## 🏁 Conclusion
This project successfully transformed a fragmented healthcare dataset into a centralized, high-fidelity analytical tool. By bridging the gap between raw data engineering and strategic visualization, the project achieved the following outcomes:

**🛠️ Technical Problem Solving**
The most significant hurdle was the structural inconsistency within the hospital naming conventions. By implementing a custom Python/Regex cleaning pipeline, I standardized over 54,000 records, ensuring data integrity and enabling accurate grouping and regional analysis. This phase highlighted the importance of "Data Wrangling" as a prerequisite for trustworthy business intelligence.

**💡 Data-Driven Insights**
The first dashboard [here](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Dashboard_1.png) and the final dashboard [here](https://github.com/AlhajiMarrah/Power-BI-Data-Project/blob/main/Dashboard_2.png) uncovered several critical operational patterns:

**Revenue Stability:** A balanced distribution of billing across insurance providers (less than a $1M spread) indicates a healthy, diversified revenue risk profile.

**Performance Benchmarking:** Identified the "Elite 3" hospitals and top medical staff, providing a benchmark for operational excellence across the network.

**Operational Consistency:** Despite fluctuations in admission routes (Emergency vs. Elective), the hospital maintains a consistent two-week average patient turnover, allowing for predictable resource planning.

**🎯 Final Impact**
The resulting Hospital Operational Performance Overview serves as more than just a collection of charts, it is a diagnostic tool. It empowers hospital administrators to move from reactive management to proactive strategy—optimizing high-value elective pipelines and identifying seasonal trends before they impact the bottom line.




