<div style="text-align: center;">
  <h1 style="background-color: #1B4B5E; color: white; padding: 20px 40px; margin-bottom: 20px; border-radius: 8px;">
    <strong style="font-size: 2em;">CAV AUTOINSURANCE</strong>
</div>


<div style="text-align: center; margin-top: -10px;">
  <span style="color: white; font-size: 1.3em;">By Cavalier</span>
</div>

<hr style="border: 5px solid #1B4B5E; width: 80%; margin: 20px auto;">

- ⭐[Ivan Robi Septian](https://github.com/Ivan-R-Septian), [Shafa Salzabila Meidita](https://github.com/shafameidita), [Ammar Muzaki Maftuh](https://github.com/Zacky182)
- 📊[Tableau Dashboard](https://public.tableau.com/app/profile/ivan.robi.septian/viz/CAVAutoinsurance-Storyboard_17266649540990/CavalierStoryboard)
- 📓[Notebook Analysis](https://github.com/PurwadhikaDev/CavalierGroup_DTI_01_FinalProject/blob/main/Autoinsurance_Cavalier.ipynb)
- 🔖[Customer Lifetime Value Dataset](https://www.kaggle.com/ranja7/vehicle-insurance-customer-data)

<p align="center">
  <img src="https://i.imgur.com/omRnugM.png" alt="logo" width="400px" />
</p>

## Context
**CAV AutoInsurance**, a reputable auto insurance consulting provider established in 2000, operates in a highly competitive market. To sustain growth and improve its market position, the company aims to enhance its marketing strategies and customer retention efforts. Specifically, **CAV AutoInsurance** seeks to develop a more targeted approach to customer retention and optimize its marketing campaigns. By understanding the value of each customer, the company intends to allocate resources more effectively, maximize the impact of its campaigns, and ultimately drive better customer engagement and increased profitability.

## Business Problem Statement
In 2011, CAV AutoInsurance client's was confronted with a substantial obstacle, with only 14.6% of their insured customers electing to renew their policies following a retention campaign. This low renewal rate revealed that 85.4% of their customers were not engaged, indicating that their current strategy of treating all customers the same was both ineffective and resource-intensive. The broad, one-size-fits-all approach failed to address the diverse needs of their customer base, emphasising the necessity for a more targeted and efficient strategy to enhance customer retention and optimise marketing efforts.

1. The marketing team launched a new campaign, categorizing efforts based on the Months Since Policy Inception, dividing them into three equal segments. This campaign was structured into three tiers, each with different costs:
- Marketing Campaign Low: 539 customers (0-34 months) at $25 each.
- Marketing Campaign Medium: 513 customers (35-63 months) at $50 each.
- Marketing Campaign High: 509 customers (64-99 months) at $150 each.

2. CAV AutoInsurance is experiencing significant challenges in analyzing Customer Lifetime Value (CLV) and improving customer retention. The company currently faces an 85.4% customer churn rate, and recent marketing efforts, segmented by the number of month since policy inception <sup>[1](https://www.upwork.com/hire/data-analysts/cost/)</sup>, have not produced the expected results, leading to inefficient use of resources and low customer engagement. The current manual process for CLV analysis, which costs $20 per customer and takes approximately per hours, is both costly and time-consuming, limiting the company’s ability to scale its operations effectively.

The company recognised the need for a more advanced solution and engaged a data science team to develop a new strategy based on customer data. This strategy aims to predict and understand the value of each customer, creating a more targeted approach that will engage customers more effectively and improve retention by focusing on their specific needs.

Key Points:

1. What steps can we take to optimise our sales strategy in order to retain our customers?
2. How can machine learning models be developed to accurately predict Customer Lifetime Value (CLV)? This will enable us to understand customer value and make decisions regarding management strategies.
3. How can we develop a clustering model to effectively segment customers? This will help us to manage risk and improve customer engagement and retention.
4. How can we accurately predict customer behaviour and optimise marketing strategies across diverse customer segments? This will help us to maximise revenue and retention. We must identify the most impactful characteristic influencing customer decisions.

## Summary
In 2011, CAV AutoInsurance faced a significant challenge with an alarming 85.4% customer churn rate. In response, the marketing team launched a new campaign, categorizing efforts based on the Months Since Policy Inception, dividing them into three equal segments.

**Segmentation Analysis**

Without machine learning, the average CLV for each campaign category was:

Campaign Category

- Marketing Campaign High: $6,763.52
- Marketing Campaign Medium: $6,702.34
- Marketing Campaign Low: $6,424.82

With machine learning, the average CLV for each cluster was:

Cluster

- Gold: $13,807.61
- Silver: $8,600.64
- Bronze: $4,010.23

The machine learning approach provided a more accurate representation of customer value, revealing significant differences across clusters, as opposed to the traditional categories, which showed incorrect CLV order.

**Cost Savings Calculation**
The campaign from marketing team was structured into three tiers, each with different costs:

- Marketing Campaign Low: 539 customers (0-34 months) at $25 each.
- Marketing Campaign Medium: 513 customers (35-63 months) at $50 each.
- Marketing Campaign High: 509 customers (64-99 months) at $150 each.

Total Marketing Campaign Cost: $115,475

While using machine learning-driven clusters, the campaign costs were recalculated:

- Bronze Campaign: 869 customers x $25 = $21,725
- Silver Campaign: 516 customers x $50 = $25,800
- Gold Campaign: 176 customers x $150 = $26,400

Total Marketing Campaign Cost: $73,925

Cost Savings: $38,575

By leveraging machine learning, CAV AutoInsurance not only achieved more accurate customer segmentation but also optimized its marketing spend. This advanced approach led to smarter resource allocation, potentially saving the company substantial amounts of money and effort by targeting the right customers with the right offers. This resulted in a total cost savings of $38,575


## Recommendation
**Model Recommendations**:
- Ensure a comprehensive data dictionary is in place, so that all features used in the model are well-defined and not based on assumptions. This will prevent misunderstandings and ensure consistency in data interpretation.
- Verify that there are no data entry errors during dataset collection, particularly in critical features like Income, Months Since Policy Inception, and Months Since Last Claim.
- Incorporate additional features, such as Customer Satisfaction and Retention Rate, to better assess customer loyalty.
- Expand the dataset, especially above $16,484 price range, to enhance the model's predictive accuracy.
- Improve the model's predictive performance through parameter tuning, using the current benchmarks as a reference point for optimization.
- Explore using DBScan clustering for customer segmentation. This method is more robust to outliers and can handle larger datasets, which may improve segmentation quality.

**Business Recommendations**:
- Enhance Offer2 Agents Channel Reach Across Other Offer Type:
    - Offer2 is particularly successful in driving renewals via the Agent channel. CAV AutoInsurance should explore ways to replicate this success in other Offers. Suit the offer presentation or providing special incentives in these channels could help increase renewals by 40%. 
    - Expand Digital Outreach for Web and Call Center Channels, Web and Call Center channels show moderate engagement, their renewal rates lag behind. CAV AutoInsurance could improve digital communication strategies, such as personalized email campaigns or online customer support, to boost customer confidence in renewing policies through these channels.

- Combine the CLV prediction model with clustering segmentation to optimize customer targeting in marketing campaigns. Aim for a 20% increase in conversion rates over the next 1 years by identifying and segmenting high-value customers. Adjust marketing messages to the specific needs of these segments, which will improve customer acquisition and retention, especially in the Gold insurance segment.

- Enhance customer service by creating a dedicated support team for Gold customers. Introduce regular engagement initiatives to increase customer satisfaction by 20% and reduce churn by 7.5% within the next year. Provide specialized training to support staff and implement engagement tools like personalized communications and loyalty programs to build stronger relationships.

- Increase the Number of Policies in the Gold cluster to leverage its significant impact on customer retention, targeting a 15% improvement in retention rates. Optimize Monthly Premium Auto to enhance overall customer lifetime value (CLV), aiming for a 10-15% uplift across all clusters. Additionally, use insights from Income and Employment Status to Adjust marketing strategies, with the goal of boosting engagement rates by approximately 10%. Implementing these strategies can lead to improved profitability and a stronger competitive advantage.

- Invest in utilizing a Data Scientist to automate Customer Lifetime Value (CLV) analysis through machine learning. By implementing this approach, the company can achieve significant cost savings of $6,322 compared to manual analysis and reduce the project timeline by 11.4 weeks, resulting in approximately 74.03% time savings. This strategic shift not only enhances operational efficiency but also allows the organization to reallocate resources toward more strategic initiatives, ultimately driving greater value and insights from the CLV analysis.

- Permanently implement machine learning for customer segmentation and CLV prediction because it can significantly reduce marketing costs by 38.4%, achieved through more efficient resource allocation and precise targeting of customers. This approach not only optimizes the use of marketing budgets but also enhances the effectiveness of campaigns, ensuring that resources are directed towards the most valuable customer segments. By leveraging machine learning, the company can make decisions that maximize both cost efficiency and marketing impact, leading to improved overall business performance.

- Develop an application based on the created model to streamline predictions and segmentation, supporting CAV Autoinsurance's operational goals.

# **Thank You**
