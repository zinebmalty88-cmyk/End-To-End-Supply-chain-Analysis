# End-To-End-Supply-chain-Analysis
End-to-end supply chain analysis project combining sales, production, inventory, and logistics data to uncover key performance insights and operational inefficiencies using Excel and Tableau.

## Objective

- Identify which product categories generate the highest revenue and sales  

- Determine Which categories are the most and least profitable

- Analyze how efficient is the supply chain in terms of lead time, shipping time, and inventory turnover  

- Determine Which carriers and transportation modes are the most costly or time-consuming  

- Identify if there are quality issues reflected in defect rates, and how do they vary across products  

- Determine How well is inventory managed, and which categories face stock availability issues

- Determine the main cost drivers in the supply chain, and where can optimization be applied?

## Dataset Description

This project uses a real-world dataset collected from a Fashion and Beauty startup, focusing on the supply chain of makeup and personal care products.

The dataset used is the **Supply Chain Dataset published by Amir Motefaker**, which simulates the operations of a mid-size beauty brand.

The dataset consists of a single, structured table containing **100 SKUs (Stock Keeping Units)** representing beauty and personal care products.

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

###  Sales and Revenue by Product & Customer Demographics

- Skincare is the top-performing category, contributing **44.97%** of total sales, indicating strong and consistent customer demand.
- Haircare follows with **29.53%**, showing solid but secondary performance.
- Cosmetics represents the lowest share at **25.50%**, suggesting potential for growth or weaker positioning.

- Female customers drive the highest revenue in Skincare (**17.04%**) and Cosmetics (**8.70%**), highlighting strong engagement from this segment.
- The "Unknown" segment contributes significantly, especially in Haircare (**16.41%**), indicating missing or incomplete customer data that could impact segmentation accuracy, This may indicate a significant opportunity to improve customer data collection in this specific segment to better understand who is actually purchasing these products.
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
🔗 [View Interactive Dashboard](https://public.tableau.com/views/End-To-End-Supply-Chain-Analysis/CommercialDashboard)

![Commercial Dashboard](images/Commercial%20Dashboard.png)

- **Operational Efficiency Analysis**: focuses on internal operations including inventory performance, logistics, supplier lead time, and product quality.

You can explore the dashboard here:  
🔗 [View Interactive Dashboard](https://public.tableau.com/views/End-To-End-Supply-Chain-Analysis/OperationalDashboard)

![Operational Dashboard](images/Operational%20Dashboard.png)

**Note**: An interactive navigation button is available at the top of the dashboard, allowing users to switch seamlessly between the Commercial and Operational views.

---

###  Commercial Performance Overview

The commercial performance is summarized through two key indicators:

- Total Revenue ($577,604.82) reflects the overall income generated from sales activities. This indicates strong business performance and highlights the effectiveness of pricing and sales strategies.

- Total Sales (46,099 units) represents the volume of products sold. A high sales volume suggests strong customer demand and market engagement across product categories.

Skincare emerges as the leading product category, contributing 44.97% of total sales and generating the highest revenue, making it the core driver of business performance. Haircare follows with moderate performance, while Cosmetics remains the lowest-performing category, indicating potential growth opportunities.

The profit analysis highlights strong performance in Skincare (219,399), making it the most profitable category and a key driver of business growth. Haircare (157,127) shows stable profitability with potential for further optimization through cost or demand improvements. Cosmetics (148,155), being the least profitable, may require strategic actions such as pricing adjustments, cost reduction, or marketing efforts to enhance its performance and align it with higher-performing categories.

Customer demographic analysis shows that female customers contribute significantly to revenue, particularly in Skincare. However, the high contribution of the "Unknown" segment, especially in Haircare, highlights a lack of complete customer data, which may limit accurate segmentation and targeted strategies.

---

###  Operational Efficiency Analysis

The operational performance indicators provide a clear overview of supply chain efficiency:

- Stock Availability (10.36%) indicates relatively low inventory coverage, suggesting potential risks of stockouts and the need for improved inventory planning.

- Lead Time (16 days) reflects the overall time required from supplier to delivery. This duration highlights opportunities to optimize supplier coordination and internal processing.

- Total Supply Chain Cost represents the overall operational expenses. Monitoring this KPI is essential to control logistics and production costs while maintaining service levels.

- Defect Rate (2.28%) shows a relatively low percentage of defective products, indicating acceptable quality performance, though continuous improvement is still recommended.

Inventory performance varies significantly across categories. Skincare achieves the highest inventory turnover, confirming strong demand and efficient stock movement, but it may also face stock availability risks due to high consumption. Cosmetics shows the lowest turnover, indicating slower-moving inventory and potential overstock issues, while Haircare remains moderate but affected by overproduction.

From a logistics perspective, Carrier B stands out as the most expensive option, while Carrier A offers the lowest cost. However, when considering delivery performance, Carrier B provides the fastest shipping times, highlighting a trade-off between cost and speed.

The stock availability analysis shows that Skincare has the highest availability, indicating better inventory coverage and lower risk of stockouts. Haircare follows with a moderate level of availability, suggesting relatively balanced inventory management. In contrast, Cosmetics records the lowest availability, which may lead to higher stockout risks and indicates a need for improved replenishment planning to meet demand effectively.

Shipping time analysis reveals that transportation mode plays a key role in delivery performance. Road transport is generally the fastest, while sea and rail are slower, especially for certain carriers. This suggests that optimizing both carrier selection and transportation mode is essential for improving delivery efficiency.

Finally, defect rate analysis indicates that Skincare and Haircare have higher defect levels compared to Cosmetics, which may impact customer satisfaction and increase operational costs, especially in high-volume categories like Skincare.


##  Recommendations & Key Actions

Based on the analysis, several strategic and operational improvements can be implemented to enhance overall business performance:

###  Profit Optimization

- Focus on expanding Skincare by reinforcing marketing and ensuring sufficient inventory to capitalize on its high profitability.
- Improve Haircare performance by optimizing pricing strategies and controlling costs to increase margins.
- Enhance Cosmetics profitability by reviewing pricing, reducing operational costs, and boosting demand through targeted promotions.

---

###  Inventory Optimization

- Increase safety stock levels for Skincare to prevent potential stockouts due to its high turnover.
- Reduce excess inventory in Cosmetics by optimizing stock replenishment cycles and improving sales strategies.
- Monitor Haircare inventory closely to avoid further accumulation caused by overproduction.

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
- Review shipping strategies to reduce reliance on high-cost carriers without compromising service levels.

---

### Stock Availability Optimization

- Increase inventory levels for Cosmetics to reduce stockout risks and ensure better product availability for customers.  
- Optimize demand forecasting and replenishment planning for Haircare to maintain a balanced inventory without overstocking.  
- Align inventory strategy for Skincare with its strong availability by monitoring demand closely to avoid excess stock while sustaining high service levels.

---

### Transportation Strategy

- Prioritize road transportation for faster deliveries where feasible.
- Limit the use of slower transportation modes (sea and rail) for time-sensitive products.
- Align transportation mode selection with product type and urgency.

---

### Quality Improvement

- Investigate high defect rates in Haircare and Skincare to identify root causes in production or handling.
- Strengthen quality control processes, especially for high-volume products like Skincare.
- Maintain current quality standards in Cosmetics as a benchmark for other categories.


##  Conclusion

This project provided a comprehensive analysis of the end-to-end supply chain of a beauty and personal care company, combining both business performance and operational efficiency perspectives.

The analysis revealed strong demand for Skincare products, making it the key revenue driver, while also highlighting inefficiencies such as overstock risks, and variability in logistics performance. Additionally, opportunities were identified to optimize inventory management, and enhance transportation strategies.

Overall, this project demonstrates how data-driven insights can be leveraged to identify inefficiencies, improve decision-making, and optimize supply chain performance in a real-world business context.
