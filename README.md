# sales-analytics
#Introduction

Welcome to this Power BI project, where it focuses on the dynamic world of retail analytics using a comprehensive dataset capturing essential details of  business operations. In this project, the intricate web of sales transactions, customer interactions, and product performance to uncover valuable insights that drive informed decision-making and enhance business outcomes.

The dataset provides a granular view of each transaction, encompassing critical attributes such as order ID, order date, ship date, ship mode, customer demographics, product details, sales metrics, and payment information. With this detailed dataset, meaningful actionable insights are generated that propel our retail business forward with a 15 days sales forecast.

#Transformation

After Importing the data set from get data and loaded in PBI desktop. For cleaning the data if necessary the table opened in edit query mode, and checked the column quality to ensure 100% valid and 0% error and 0% null values present. 

Ind1 and ind2 columns were deleted as all of the rows of these columns are null. 
As the Return column contains all N/A values, the values were replaced with 0.
Checked the data type of each column and changed the data type of order date column to date/time mode and for Returns column data type changed from text to whole number

Another column added to find out how many average days needed to ship the delivery.

AvgDelivery = DATEDIFF(STORE_DATA[Order Date],STORE_DATA[Ship Date],DAY)


#Visualisation
The dashboard includes various visualisations and filters to analyse sales data effectively:

Background

From the format page of the visual, the background image has been uploaded from canvas background. 
Then for each visual, the background has been set to 100% transparency to make the background visible, and the values as well as title colours also changed to make it well visible. 

Cards:

Cards display key metrics such as total orders, total sales, total profit, and total shipping days.

Map:

A map visualisation is generated to visualise profit and sales by state. States are plotted on the map, with bubble sizes indicating the sum of sales and tooltips showing the sum of profit.

Donut Chart:

Three donut charts provide insights into the distribution of sales by payment mode, sales by region, and sales by segment.The respective charts have total sales under values, and under legend part, payment mode,  region and segment respectively. The label contents changed to category, percent of values to get a clear visualisation.

Area Chart:

Two area charts represent total sales over time.. One chart displays total sales by month, while the other shows total sales by profit. In the first chart,the x-axis includes order date and month (in the first one), and the second chart includes order date, date and month and the legend includes order date and year for both cases. The y-axis represents the sum of sales and sum of profit, respectively. Order date added to legend and from order date selected year from date hierarchy to make the different visual for different year separately. Further customisation done to remove grid lines and titles.

Clustered Bar Chart:

Three clustered bar charts visualise sales data based on different categories. They depict sales by ship mode, sales by category, and sales by sub-category. The x-axis represents the sum of sales, while ship mode, category, and sub-category are included on the x-axis for three charts and the y-axis represents Total sales. Some customisation like data labels were made value inside, and for bars changed the colours for each bar.

Slicer:

A slicer allows users to filter data by region. The slicer is styled as a tile for easy selection.
These visualisations and filters provide a comprehensive overview of sales data, enabling users to analyse trends, identify patterns, and make data-driven decisions.

Line Chart

Two line charts added to generate the visuals for monthly total sales (total sales variation over month), where order date is added in x-axis and sum of sales in y-axis. In the second line chart, the extra part is the zoom slider that makes a clear understanding of change in total sales in different time frames. Forecast was set on and forecast length was set to 15 with 95% confidence interval.

#Insight
The noticeable surge in sales during the latter half of both 2019 and 2020 suggests potential seasonality or external factors influencing consumer purchasing behaviour. Further investigation into the drivers behind this trend could provide valuable insights for future sales forecasting and planning.

The average shipment delivery time of 4 days indicates efficient logistics management, contributing to positive customer experiences and satisfaction. This highlights the importance of maintaining and optimising delivery processes to meet customer expectations and drive repeat business.

With total profit nearing 175k and total sales reaching 1.6 million, it's evident that the company is performing well financially. However, identifying areas with the highest profitability margins and focusing resources accordingly could further enhance overall profitability and sustainability.

The stark difference in sales performance between regions underscores the importance of targeted marketing and sales strategies tailored to specific geographical areas. Understanding the unique preferences and needs of customers in each region can help optimise marketing efforts and drive sales growth.

The dominance of cash on delivery as the preferred payment mode suggests a need for diversification in payment options to cater to varying customer preferences. Introducing alternative payment methods could potentially attract new customers and improve overall sales conversion rates.

The strong performance of standard class shipments, mobile phones, and office supplies indicates potential areas of strength within the product offerings. Capitalising on these high-performing categories through targeted marketing campaigns and product promotions could further drive sales and revenue growth.

Overall, these insights provide valuable guidance for strategic decision-making, enabling the company to capitalise on strengths, address weaknesses, and optimise operations for sustained success in the competitive market landscape.

# sales-analytics

## Introduction

Welcome to the Sales Analytics project! This Power BI project is dedicated to exploring the dynamic realm of retail analytics using a comprehensive dataset that captures essential details of business operations. Through detailed analysis of sales transactions, customer interactions, and product performance, this project aims to uncover valuable insights that drive informed decision-making and enhance business outcomes.

## Transformation

Upon importing the dataset into Power BI Desktop, several transformations were performed to clean and refine the data for analysis. This included removing unnecessary columns, handling null values, adjusting data types, and deriving new metrics such as average delivery time for shipments.

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








 
