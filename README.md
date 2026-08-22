# End-To-End-Supply-chain-Analysis
End-to-end supply chain analysis project combining sales, production, inventory, and logistics data to uncover key performance insights and operational inefficiencies using Excel and Tableau.

## Objective

- Analyze commercial performance

- Evaluate inventory performance

- Analyze logistics and transportation 

- Identify business recommendations

## Dataset Description

The dataset used is the **Supply Chain Dataset published by Amir Motefaker**, which simulates the operations of a mid-size beauty brand.

The dataset consists of a single, structured table containing **100 SKUs (Stock Keeping Units)** representing beauty andpersonal care products.

It provides a comprehensive view of supply chain activities, making it a strong foundation for analyzing both business performance and operational efficiency.

##  Data Cleaning & Preparation

Before starting the analysis, the dataset was carefully cleaned transformed using **Power Query in Excel** to ensure accuracy, consistency, and reliability of the results.

---

### Handling Missing Values

- No missing or null values were identified in the dataset

---

### Data Type Correction

- Converted numerical fields (Revenue, Sales, Production Volume) to appropriate numeric formats.
- Ensured percentage fields were correctly formatted.
- Standardized date/time-related fields where applicable (e.g., lead time, shipping time).

---

### Data Consistency 

- Verified consistency across categorical fields such as:
  - Product Category
  - Gender
  - Supplier
  - Carrier
  - Transportation Mode
 
---

###  Removing Duplicates

- No duplicate records are detected across SKU and product level data.

---
  
###  Final Dataset Readiness

After cleaning and transformation, the dataset was:
- Structured for analysis
- Free from inconsistencies and duplicates
- Ready for visualization and dashboard development

## Data Analysis & Insights

All analyses were conduxted using **Pivot Tables** to efficiently summarize and explore the data 

###  Sales and Revenue by Product & Customer Demographics

- Skincare is the best performing category with **44.97%** of total sales. This means customer demand is strong and steady.

- Haircare follows with **29.53%**, showing solid but secondary performance.
- Cosmetics represents the lowest share at **25.50%**, suggesting potential for growth or weaker positioning.

- Female customers drive the highest revenue in Skincare (**17.04%**) and Cosmetics (**8.70%**), highlighting strong engagement from this segment.
- The "Unknown" segment contributes significantly, especially in Haircare (**16.41%**), indicating missing or incomplete customer data.
- Male and Non-binary contributions remain moderate across all categories, with no dominant pattern.

###  Inventory and Production Performance by Product Category

Skincare demonstrates the highest inventory turnover (12.9), indicating strong demand and efficient stock movement. However, this high turnover combined with relatively lower stock levels suggests a potential risk of stock shortages. In addition, Skincare shows a notable production gap (3,635 units), making it a critical category that requires close monitoring to balance supply with its high demand.

Haircare presents moderate inventory turnover (8.3), reflecting acceptable but improvable efficiency. However, it has the largest production gap (6,346 units), indicating significant overproduction or slower sales velocity. This imbalance suggests inefficiencies in demand forecasting and a risk of excess inventory accumulation.

Cosmetics, on the other hand, shows the smallest production gap (704 units), indicating good alignment between production and demand. Despite this balance, it has the lowest inventory turnover (7.7), highlighting slower-moving stock and a potential overstock risk. This suggests that while production planning is accurate, demand generation or sales performance may need improvement.

### Product Quality (Defect Rates)

- Haircare has the highest defect rate (**2.48%**), indicating potential quality or production issues.
- Skincare follows closely (**2.33%**), which is concerning given its high sales volume.
- Cosmetics has the lowest defect rate (**1.92%**), suggesting better quality control.

---

### Shipping Cost Analysis

- Carrier B has the highest shipping cost (**236.90**), making it the most expensive option.
- Carrier C shows moderate cost (**162.38**).
- Carrier A is the most cost-efficient (**155.54**).

- The cost variation suggests an opportunity to optimize carrier selection for cost reduction.

---

###  Lead Time by Supplier

- Average lead time is relatively consistent across suppliers (~22–24 days).
- Supplier 5 and Supplier 4 have the longest lead times (**24 days**), which may impact supply chain responsiveness.
- Supplier 1 and Supplier 3 are faster (**22 days**), making them more efficient options.

---

###  Shipping Time by Carrier & Transportation Mode

- Carrier B has the fastest overall shipping time (**5.3 days avg**), making it the most efficient carrier.
- Carrier A (**6.1 days**) and Carrier C (**6.0 days**) are slightly slower.

- By transportation mode:
  - **Road** is generally the fastest (as low as **3.7 days** with Carrier C).
  - **Sea and Rail** tend to have longer delivery times (up to **7.4 days**).

- Carrier performance varies significantly by transportation mode, indicating optimization opportunities based on shipment type.

##  Dashboard Analysis & Insights

To provide a comprehensive view of the business, two dashboards were developed:

- **Commercial Performance Overview**: focuses on high-level metrics such as sales, revenue, customer behavior, and the alignment between production and demand.

You can explore the dashboard here:  
🔗 [View Interactive Dashboard](https://public.tableau.com/app/profile/zineb.malty/viz/End-to-EndSupplyChainAnalysis/Dashboard8)

![Commercial Dashboard](https://github.com/zinebmalty88-cmyk/End-To-End-Supply-chain-Analysis/blob/main/Images/Commercial%20Dashboard%20(2).png?raw=true)

- **Operational Efficiency Analysis**: focuses on internal operations including inventory performance, logistics, supplier lead time, and product quality.

You can explore the dashboard here:  
🔗 [View Interactive Dashboard](https://public.tableau.com/app/profile/zineb.malty/viz/End-to-EndSupplyChainAnalysis/Dashboard8)

![Operational Dashboard](https://github.com/zinebmalty88-cmyk/End-To-End-Supply-chain-Analysis/blob/main/Images/Operational%20Dashboard%20(2).png?raw=true)

**Note**: An interactive navigation button is available at the top of the dashboard, allowing users to switch seamlessly between the Commercial and Operational views.

---

###  Commercial Performance Overview

The commercial performance is summarized through two key indicators:

- Total Revenue ($577,604.82) All Revenue from sales activity. This indicates strong business results and highlights the success of pricing and sales tactics.

- Total Sales (46,099 units) shows the number of products sold. High sales volume implies strong customer demand and market engagement across all product categories.

The primary product category is skincare, which contributes 44.97% of total sales and generates the highest revenue, thereby acting as the main driver of the company's business performance. Haircare provides moderate performance, with Cosmetics still the lowest performing category, indicating potential for growth..

The profit analysis reveals that Skincare (219,399) is the most profitable category and a key driver of business growth. Haircare (157,127) has stable profitability with room for further optimization with cost/demand increase. Cosmetics ( 148,155 ) is the least profitable and may require strategic actions such as pricing, cost reduction or marketing activities to improve its performance to be in line with the higher performing categories

Customer demographic analysis shows that female customers contribute significantly to revenue, particularly in Skincare. However, the high contribution of the "Unknown" segment, especially in Haircare, highlights a lack of complete customer data, which may limit accurate segmentation and targeted strategies.

---

###  Operational Efficiency Analysis

The operational performance indicators provide a clear overview of supply chain efficiency:

- Stock Availability (48.40%) More than 50% of products are not available. It indicates risks of stockouts, loss of sales and the need for improved inventory planning.

- Lead Time (16 days) represents the total time from supplier to delivery. This period shows opportunities for better supplier coordination & internal processing.

- Total Supply Chain Cost Total operating cost. This KPI is a must-watch to keep logistics and production costs in check and service levels up.

- The Defect Rate (2.28%) demonstrates that the percentage of defective products is relatively low and the quality performance is acceptable. However, continuous improvement is still recommended.

Inventory performance varies significantly across categories. Skincare has the highest inventory turnover, indicating strong demand and fast stock movement. However, with overall stock availability at only 48.4%, its fast-moving inventory may increase the risk of stockouts, making timely replenishment essential. Cosmetics has the lowest inventory turnover, suggesting slower-moving inventory and a potential risk of excess stock. Haircare shows moderate inventory turnover, indicating an opportunity to better align inventory levels with demand

From a logistics perspective, Carrier B is the most expensive logistics wise and Carrier A is the cheapest. Carrier B is fastest in terms of delivery performance, but it’s also the most expensive. It’s a trade-off between cost and speed

Finally, defect rate analysis indicates that Skincare and Haircare have higher defect levels compared to Cosmetics, which may impact customer satisfaction and increase operational costs, especially in high-volume categories like Skincare.


##  Recommendations & Key Actions

Based on the analysis, several strategic and operational improvements can be implemented to enhance overall business performance:

###  Profit Optimization

- Skincare is the most profitable business. The company should grow its marketing and have enough stock to reap the benefits.
- Increase Haircare performance through better pricing strategies and cost controls to drive margins.
- Improve profitability of Enhance Cosmetics by assessing pricing and creating demand through strategic promotions.

---

###  Inventory Optimization

- Increase safety stock levels for Skincare to prevent potential stockouts due to its high turnover.

---

###  Customer Data & Segmentation

- Improve data collection processes to reduce the "Unknown" customer segment and enable more accurate customer segmentation.
- Leverage female customer dominance in key categories (especially Skincare) for targeted marketing campaigns.
- Develop personalized strategies for underperforming segments (Male and Non-binary) to increase engagement.

---

### Logistics Cost & Efficiency

- Optimize carrier selection by balancing cost and delivery performance:
  - Use Carrier A for cost efficiency.
  - Use Carrier B for faster deliveries when speed is critical.
  - 
---

### Stock Availability Optimization

-Align Skincare’s inventory strategy with its high turnover and availability by closely monitoring demand and replenishment to prevent stockouts while maintaining high service levels.

---

### Quality Improvement

- Investigate high defect rates in Haircare and Skincare to identify root causes in production or handling.
- Strengthen quality control processes, especially for high-volume products like Skincare.

##  Conclusion

This project established a comprehensive analysis of an end-to-end supply chain of beauty and personal care company, merging both business performance and operational efficiency perspectives.

The analysis found that Skincare products are in high demand and represent the main revenue driver, but also inefficiencies such as risks of overstock and variability in logistics performance. Further opportunities were identified to improve inventory management, and improve transportation strategies.

Overall, this project demonstrates how data-driven insights can be used to identify inefficiencies, improve decision-making, and optimize supply chain performance in a real-world business context.
