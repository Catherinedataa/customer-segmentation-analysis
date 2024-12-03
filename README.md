# ** Customer Segmentation Analysis for Axis Retail Solutions**

## **Overview** 
Understanding customer behavior is essential for any successful strategy in today's competitive e-commerce landscape. This project focuses on **customer segmentation** for **Axis Retail Solutions**, an e-commerce company that sells high-quality retail products across the globe. The company has been accumulating data regarding the demographic segments of its customers, their buying behavior, geographical trends, and response to various marketing campaigns. However, this data had yet to be leveraged to drive strategic decisions.
It identifies actionable insights in the following ways: customer profile and behavior, purchase pattern, effectiveness of marketing campaigns, amongst others. With segmentations through clusters, Axis Retail Solutions would seek to create targeted marketing activities towards engagement levels and revenue growth. 

## **Insights and recommendations are structured around these key focus areas:**
**Customer Demography and Geographical Dispersion**
Evaluate Customer Dispersion in geographies to identify potential high market pockets and strong potential engaging pockets.

Analyze how age, income, education, and family size affect the purchase pattern.

**Purchase Patterns**
Recognize which customer segments are most active in certain product categories and identify which segments provide the highest revenue streams.

**Campaign Responsiveness**
Understand how different customer segments respond to marketing campaigns; identify the most effective engagement strategies for each segment.

An interactive Power BI dashboard: [here](https://github.com/Catherinedataa/customer-segmentation-analysis/blob/master/customer-segmentation.pbix) 

Jupyter notebook where the analysis and clustering was done: [here](https://github.com/Catherinedataa/customer-segmentation-analysis/blob/master/customer_personality.ipynb)

## Data Structure
The original dataset had 28 columns, which were:
•	Demographics
- ID, Year_Birth, Education, Marital_Status, Income, Kidhome, Teenhome, Dt_Customer, Country.

•	Customer Behavior
- Recency, NumDealsPurchases, NumWebPurchases, NumCatalogPurchases, NumStorePurchases, NumWebVisitsMonth, MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, MntGoldProds.

•	Engagement
- AcceptedCmp1, AcceptedCmp2, AcceptedCmp3, AcceptedCmp4, AcceptedCmp5, Response, Complain.

•	New Features:
- Age from Year_Birth, Customer Enrollment Days from Dt_Customer, NumKids from Kidhome and Teenhome, MntTotal from MntWines, MntFruits, MntMeatProducts, MntFishProducts, MntSweetProducts, and MntGoldProds.
- TotalPurchases from NumDealsPurchases, NumWebPurchases, NumCatalogPurchases and NumStorePurchases, and Num_Accepted sum of accepted campaigns.

•	Transformations:
- Encoded categorical features: Marital_Status, Education, Country, Campaign_Engagement, and normalized numerical columns.

•	Clustering:
- **K-Means** was applied to create three clusters based on customer spending, purchasing, and engagement patterns. Added two new columns: Cluster and Category of Cluster.

The enriched dataset, stored in the customer_personality_cluster_output table, was used to create the dashboard, linking customer traits to actionable insights.
![image](https://github.com/user-attachments/assets/57da53e2-cf14-4d5d-99e2-74c3d13b813c)


## Executive Summary
**Overview of Findings** 
Axis Retail Solutions' customer segmentation analysis uncovered three distinct clusters with varying behaviors, preferences, and purchasing tendencies. This segmentation provides actionable insights to optimize marketing strategies and enhance revenue growth.

- **Cluster 1**: Price-sensitive customers contributing minimal revenue despite accounting for a significant portion of the customer base.
- **Cluster 2**: Moderately engaged customers with average purchasing power and steady interaction levels.
- **Cluster 3**: High-value customers demonstrating strong brand loyalty, consistent engagement, and significant contributions to overall revenue.
- 
  Below is an overview page from the Power BI dashboard, with additional examples provided throughout the report.
![image](https://github.com/user-attachments/assets/7dd91e3f-f913-4d1e-ab98-3a525de11a12)

The interactive Power BI dashboard can be accessed here : [here](https://github.com/Catherinedataa/customer-segmentation-analysis/blob/master/customer-segmentation.pbix) 

**Customer Demographics and Geographic Insights**

Analysis of demographic characteristics revealed distinct trends across the clusters:

- **Cluster 1**: Mature-middle-income customers living in Spain, Saudi Arabia, Canada, and India, with higher internet visits but lower purchases. Moderated spending on Wine and Meat products with poor campaign contact.
  
- **Cluster 2**: Older, high-income earners spread across Spain, Saudi Arabia, Canada, and India, with the strongest online purchasing. High spending on Wines, Meat Products, and Gold Products; moderate campaign responsiveness.
  
- **Cluster 3**: Affluent customers with incomes between $100,001–$250,000. Majority from Spain, Saudi Arabia, and Canada. High catalog and store purchases, highest spenders in all categories, and most responsive to campaigns.

- **Top-performing regions**: Spain, Saudi Arabia, and Canada constantly outperformed others by a margin in revenue and engagement, showing strong market presence and customer loyalty.
- **Growth opportunities**: While India and Australia are smaller markets, they have considerable untapped potential that can offer promising prospects by targeting campaigns for expanded reach.

This geographic segmentation emphasizes the need for region-specific strategies to fortify dominant markets and capitalize upon emerging opportunities.

![image](https://github.com/user-attachments/assets/22a0470e-6297-472a-a2cf-0a2344b79d57)
![image](https://github.com/user-attachments/assets/622af40a-37f9-4850-a608-8994137a7b12)


**Purchasing Patterns**

The purchasing behaviors show the following trends:
- **Cluster 1**: Fewer purchases, cost-effective options, limited product variety.
- **Cluster 2**: Moderate purchase frequency, balanced spending habits, wide range of product interests.
- **Cluster 3**: Frequent purchases, premium products, contributing significantly to overall revenue.

**Conversion Rates**: Cluster 3 has the highest conversion efficiency, while Cluster 1 has the lowest engagement and conversion success.

![image](https://github.com/user-attachments/assets/c8b1b6e5-0e0f-45b2-b94a-2f5cbfc1a0f2)
![image](https://github.com/user-attachments/assets/d0fd7ee0-ce6b-4e56-9d92-28472be6f3d2)



**Campaign Responsiveness**

Customer responsiveness to marketing campaigns showed a very distinct pattern:

- **Cluster 1**: Passive, rarely responding to campaigns. Campaigns targeted at this group had the least impact.
- **Cluster 2**: Medium level of responsiveness, with participation in seasonal promotions and targeted discounts.
- **Cluster 3**: Very responsive; frequently engaged with multiple campaigns, mainly those offering premium or exclusive value.

The effectiveness of campaigns was mixed, with the most interest shown in personalized, high-value campaigns, while generic promotions achieved less success.

![image](https://github.com/user-attachments/assets/6e190e95-a5f4-4730-9e8d-1189a0cc96b7)

## Recommendations

### Cluster 1: Price-Sensitive and Browsing-Centric Customers
- **Convert Browsing into Purchases through Increased Engagement**: Targeted promotions such as personalized discounts or time-sensitive offers.
- **Focus on Cost-Effective Products**: Offer more economical product variants and bundle discounts for value-for-value purchases.
- **Better Campaign Targeting**: Design more personalized campaigns aligned with their interests, and consider retargeting to re-engage inactive customers.

### Cluster 2: Moderately Engaged, Balanced Spenders
- **Capitalize on Seasonal Campaigns and Targeted Discounts**: Expand seasonal promotions and create exclusive bundles.
- **Enhance Campaign Personalization**: Use data to send tailored offers based on their previous purchases.
- **Segment and Re-engage**: Design re-engagement campaigns for dormant customers.

### Cluster 3: High-Value, Premium Product Consumers
- **Expand Premium and Exclusive Campaigns**: Continue promoting high-end products and create VIP or loyalty programs.
- **Target Value-Driven Messaging**: Focus on campaigns that highlight added value and quality.
- **Nurture High-Engagement Campaigns**: Offer more interactive campaigns or early access offers.

### Cross-Cluster Recommendations
- **Optimize Marketing Channels**: Improve content and messaging for channels with low engagement.
- **Target Growth Markets**: Focus on underrepresented regions like India and Australia, using tailored local content and campaigns.

---

## Caveats
- **Data Representativeness**: Analysis is based on available data, which may not fully represent the entire customer base. Further data collection and segmentation could provide more accurate insights.
- **External Factors**: Economic cycles, market conditions, or unforeseen occurrences may impact customer behavior and the effectiveness of strategies.
- **Campaign Execution**: Proper execution of recommended campaigns is crucial for their success. Any flaw in implementation could diminish expected outcomes.

  
