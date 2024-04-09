# sales-analytics

## Introduction

Welcome to the Sales Analytics project! This Power BI project is dedicated to exploring the dynamic realm of retail analytics using a comprehensive dataset that captures essential details of business operations. Through detailed analysis of sales transactions, customer interactions, and product performance, this project aims to uncover valuable insights that drive informed decision-making and enhance business outcomes and foecastinf the business for the next 15 days.

## Data Preparation

After importing the dataset into Power BI Desktop using the "Get Data" function, the data was loaded for analysis. In order to ensure data integrity and quality, the dataset underwent a thorough cleaning process in the query editor mode.

### Data Cleaning Process:

1. **Quality Check**: The table was opened in edit query mode to assess the quality of the columns. It was crucial to ensure that all columns contained 100% valid data with 0% errors and null values.

2. **Column Deletion**: Columns "Ind1" and "Ind2" were identified as containing null values in all rows. As these columns did not provide any meaningful data, they were deleted from the dataset.

3. **Handling N/A Values**: The "Return" column was found to contain only N/A values. To address this, all N/A values in the "Return" column were replaced with 0 to maintain data consistency.

4. **Data Type Adjustment**: The data types of each column were carefully reviewed and adjusted as needed. Specifically, the data type of the "Order Date" column was changed to date/time mode to facilitate time-based analysis. Additionally, the data type of the "Returns" column was changed from text to whole number to ensure consistency in data representation.

### Additional Calculations:

To further enhance the analysis, an additional column was created to calculate the average number of days needed to ship deliveries. This was achieved by calculating the difference in days between the "Order Date" and "Ship Date" columns using the DATEDIFF function:

```DAX
AvgDelivery = DATEDIFF(STORE_DATA[Order Date], STORE_DATA[Ship Date], DAY)
```


## Visualization

The project dashboard comprises various visualizations and filters to analyze sales data effectively:

- **Background**: The background image was customized for visual appeal, and transparency settings were adjusted for clarity.
  
- **Cards**: Key metrics such as total orders, sales, profit, and shipping days are displayed through cards.

- **Map**: A map visualization illustrates profit and sales by state using bubble sizes and tooltips for enhanced insights.

- **Donut Chart**: Three donut charts provide insights into sales distribution by payment mode, region, and segment.

- **Area Chart**: Two area charts represent total sales over time, one by month and the other by profit.

- **Clustered Bar Chart**: Three clustered bar charts visualize sales data by ship mode, category, and sub-category.

- **Slicer**: A slicer allows users to filter data by region for focused analysis.

- **Line Chart**: Two line charts display monthly total sales variation with a zoom slider and forecast length for 15 days.

## Insight

- **Seasonal Trends**: There is a noticeable surge in sales during the latter half of both 2019 and 2020, suggesting potential seasonality or external factors influencing consumer behavior.

- **Delivery Efficiency**: An average shipment delivery time of 4 days indicates efficient logistics management, contributing to positive customer experiences.

- **Financial Performance**: With total profit nearing 175k and total sales reaching 1.6 million, the company exhibits strong financial performance.

- **Regional Disparities**: The stark difference in sales performance between regions underscores the importance of targeted marketing strategies.

- **Payment Preferences**: The dominance of cash on delivery suggests a need for diversification in payment options to cater to varying customer preferences.

- **Product Insights**: Strong performance in certain product categories indicates potential areas of strength within the product offerings.

These insights provide valuable guidance for strategic decision-making, enabling the company to capitalize on strengths, address weaknesses, and optimize operations for sustained success in the competitive market landscape.

![sales-forcast gif](https://github.com/roy-deblina/Sales_dashboard/assets/164593876/ebb137f8-2236-4fa4-a958-92ef1b51cf75)
![sales gif](https://github.com/roy-deblina/Sales_dashboard/assets/164593876/37f914ff-9381-4c24-8d71-89b50167e0ca)













 
