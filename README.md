# Outlier_analysis


![flow_chart](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/flow_chart.png)

 a. Think about what could be going wrong with our calculation. Think about a better
way to evaluate this data.

 * The average order value(AOV) is 3145.13 as calculated initially, but the max order value is 1800 times higher than the 75th percentile. Apparently, there may be some outliers spreading in the high-order-value region. It will bring up the average number and the stakeholder may make a wrong business decision based on the misleading result. To confirm the outlier issue, the boxplot was used to re-analyze the dataset. Two further actions can be considered: 
1. First action is to remove the outliers from dataset so the average order value would be more representative, and make a list all of the outliers for the Action 2.
2. Since the outliers make significant contribution to revenue for March 2017, it may be necessary to track outliers over the time to see if there is any need to create another business mode for these high end customers. 

>
b. What metric would you report for this dataset? 
  
  *  Prefer to use IQR but can be adjusted based on what the stakeholder need

  *  Had tried two metrics for this dataset: one is Z-Score and another is IQR. IQR provides better data metrics than Z-Score. Based the metric analyzed by Z-Score, the max order value is still 260 times higher than the 75th percentile and, according to the boxplot graph, several outliers are not identified. However, after IQR is applied, the max order amount is down to 730. However, this metric removes some data which is under 1000. Therefore, the criteria of how to define what outlier is need to be further confirmed by stakeholders and see if it is meet what they need.
  
#### < Z-Score >
  
  ![z_describe](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/z_describe.png)
  
  ![z_boxplot](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/z_boxplot.png)
  
#### < IQR >
  
  ![IQR_describe](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/IQR_describe.png) 
  
  ![IQR_boxplot](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/IQR_boxplot.png)
  
  ![IQR_distribution](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/IQR_distribution.png)
  
  ![Outlier_list](https://github.com/WeiTing83/Shopify_Technical_Challenge_Submission/blob/main/Question1/image/outlier.png)
>
c. What is its value? 

   Use IQR to remove outliers.
   
   AOV=293.715

