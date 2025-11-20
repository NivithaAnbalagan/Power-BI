# Bank Customer Analysis
This project presents an interactive Power BI dashboard designed to analyze key customer insights from a banking dataset. It helps identify customer behavior patterns, product usage using data visualization and DAX-driven metrics.
## Project Overview
The goal of this project is to enable data-driven decision-making by analyzing customer demographics, financial activity, and banking product adoption. The dashboard provides meaningful insights to help improve customer retention and targeted marketing.
## Key Insights
- Customer segmentation based on demographics and behavior
- Churn trends and major factors influencing customer drop-off
- Loan, credit card, and deposit product utilization
- Revenue contribution and high-value customer identification
## Tools & Technologies
- Power BI Desktop
- Power Query
- DAX (Data Analysis Expressions)
## Dashboard
 <img width="882" height="497" alt="image" src="https://github.com/user-attachments/assets/1e3adcee-4ef0-4816-b443-98f1e969375e" />
 
## Dashboard Insights
1. Customer Activity Chart
This chart represents the proportion of active and inactive customers. It visually highlights how customer engagement levels vary within the bank.

3. Monthly Trend Chart
The trend chart shows how customer behavior changes month by month. It helps in identifying specific months with higher or lower activity or exits, giving insights into seasonal or operational factors.
4. Gender Distribution Chart
This chart illustrates the distribution of customers based on gender. It helps to understand the balance between male and female customers and how their engagement levels differ.
5. Credit Score Category Chart
This visualization represents customers grouped by their credit score levels such as “Good,” “Very Good,” and “Excellent.” It helps the bank identify which credit groups are more likely to remain active or inactive.
6. Summary Cards
The dashboard includes cards that provide a quick overview of total customers, active/inactive members, and credit card users. These cards make it easy to view the bank’s key statistics at a glance.
## DAX Formulas Used
- Max_Credit = MAX(Bank[CreditScore])

- Totalcustomer = COUNT(Bank[CustomerId])

- Active Member = CALCULATE(COUNT(Bank[IsActiveMember]),KEEPFILTERS(Bank[IsActiveMember]=1))

- Inactive Member = CALCULATE(COUNT(Bank[IsActiveMember]),KEEPFILTERS(Bank[IsActiveMember]=0))
  
- Credit Holder = CALCULATE(COUNT(Bank[HasCrCard]),KEEPFILTERS(Bank[HasCrCard]=1))
  
- Not Credit Holder = CALCULATE(COUNT(Bank[HasCrCard]),KEEPFILTERS(Bank[HasCrCard]=0))
  
- Retain Customers = CALCULATE(COUNT(Bank[Exited]),KEEPFILTERS(Bank[Exited]=0))
  
- Exit Customers = CALCULATE(COUNT(Bank[Exited]),KEEPFILTERS(Bank[Exited]=1))

## Conclusion
The findings of this project demonstrate the value of visual analytics in enabling the bank to gain a deeper understanding of its customer base and support data-driven strategic decision-making. Based on the insights derived, several recommendations can be implemented to strengthen overall business performance:

- Develop structured engagement initiatives aimed at reactivating customers who exhibit low or declining activity levels.

- Enhance service quality and operational responsiveness to improve retention, particularly among customers with strong credit standing.

- Introduce periodic customer feedback assessments to evaluate satisfaction levels and identify areas requiring service improvement.

- Expand the use of personalized communication and tailored product offerings to foster stronger, long-term customer relationships.
