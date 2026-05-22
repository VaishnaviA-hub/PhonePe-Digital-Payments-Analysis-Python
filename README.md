# PhonePe-Digital-Payments-Analysis-Python
Exploratory Data Analysis of PhonePe's transaction and user data across Indian states and districts (2018-2021) using Python. Investigates transaction trends, user adoption, device usage, and demographic impacts. Uncovers key insights on market penetration, common transaction types, and data quality for strategic decision-making.

## 🎯 Project Objective
To perform an in-depth Exploratory Data Analysis (EDA) of PhonePe's transaction and user data across Indian states and districts from 2018 to 2021. The goal is to identify trends, patterns, and insights into digital payment adoption, user behavior, and device usage to support strategic decision-making.

## Dataset
👉 [View Dataset](./phonepe-pulse-raw-data.xlsx)

## ❓ Questions
*   How do transaction trends and amounts vary across states and over time?
*   What are the most common transaction types in each state and quarter?
*   Which device brands have the highest number of registered users in each state?
*   What are the top districts per state based on population?
*   What is the Average Transaction Value (ATV) for each state, and what factors might explain discrepancies?
*   What are the app usage trends, and why might 'App Opens' be zero for periods with non-zero transactions?
*   Is there a unique mapping between district names and codes?
*   Are there data consistency issues between state and district-level datasets?
*   What is the ratio of registered users to the population by state, and what does a high ratio signify?
*   How does population density correlate with transaction volume at state and district levels?
*   What is the average transaction amount per user?
*   What is the device brand usage ratio across states?

## ⚙️ Process
1.  **Data Loading and Understanding:** Loaded five datasets (`stateTxn_Users`, `stateTxn_Split`, `stateTxn_DevData`, `distTxn_Users`, `distDemo`) into Pandas DataFrames. Displayed basic statistics, data types, and checked for missing values.
2.  **Exploratory Data Analysis (EDA):** Analyzed transaction trends by state, identified common transaction types, determined top device brands by registered users, listed top districts by population, calculated Average Transaction Value (ATV), and examined app usage trends.
3.  **Data Quality Checks:** Compared aggregated district-level data with state-level data to ensure consistency, specifically focusing on Transactions, Amount (INR), and ATV (INR).
4.  **Data Merging and Advanced Analysis:** Calculated the ratio of registered users to population by state, correlated population density with transaction volume, and computed the average transaction amount per user. Also analyzed device brand usage ratio.
5.  **Data Visualization:** Created various plots including line plots for transaction/amount trends, pie charts for transaction type distribution, and bar plots for population density and device brand usage ratios.

## Jupyter Notebook
👉 [View Notebbok](./PhonePe_CaseStudy.ipynb)

## 🔍 Insights
*   'Karnataka', 'Maharashtra', and 'Telangana' lead in transaction volume, while 'Lakshadweep', 'Andaman & Nicobar Islands', and 'Ladakh' have the lowest.
*   'Recharge & bill payments' is consistently the most common transaction type.
*   'Xiaomi' is the dominant device brand for registered users in many states.
*   High ATV in remote states (Ladakh, Andaman & Nicobar) might be due to larger, less frequent transactions, while low ATV in populous states (West Bengal, Delhi) is linked to frequent micro-transactions.
*   Discrepancies in 'App Opens' data suggest potential data collection gaps rather than actual zero activity.
*   Delhi shows a high user-to-population ratio (5.68), likely influenced by its large transient population.
*   There is a weak to no correlation between state-level population density and transaction volume, but a slight positive correlation at the district level.
*   'Telangana', 'Andhra Pradesh', and 'Karnataka' have the highest average transaction amounts per user.
*   Device brand usage varies significantly by state, with Xiaomi, Samsung, and Vivo having strong market presence.
  
## ✅ Final Conclusion
This comprehensive analysis of PhonePe's transaction and user data from 2018-2021 offers critical insights into India's digital payment landscape. We've uncovered regional disparities in transaction volumes, identified 'Recharge & bill payments' as a dominant transaction type, and observed the market penetration of leading mobile device brands. While state-level population density showed little correlation with transaction volume, areas for data consistency improvement, especially concerning ATV calculations, were highlighted. These findings are vital for formulating targeted strategies in market expansion, service innovation, and user engagement.
