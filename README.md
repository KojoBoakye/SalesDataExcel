 # SalesDataExcel
Analysing sales data in spreadsheet (Excel)

## Goals and Purpose:

The primary goal of the "Sales Data Analysis" project was to identify and and gain valuable insights in a company's sales data to answer some stakeholder questions.

<br>

## Data Source:

The dataset used for this project was obtained from Kaggle, specifically from the contributor Bhavana Joshi. 
<br>
<br>
## Analysis Report:
<br>
<br>
> The **ASK** Phase:

Stakeholder Questions to be answered.

1.	What are the top-selling products over the two-year period, 

2.	Can you identify any seasonality patterns in sales data for different product categories?

3.	What is the overall revenue generated from sales over the two-year period, and how does it vary by month and year?

4.	Are there any specific days of the week that tend to have higher sales volumes?

5.	What is the average profit margin for each product category, and how has it changed over the two years?

6.	How does the price elasticity of demand vary across different product categories, and how can this information be used to optimize pricing strategies?

   <br>
   <br>

> The PREPARE Phase:

I collected this dataset from Kaggle. The data was stored in a .xlsx file
Which contained two sheets; A master sheet which contains the details of the products being sold and the Input Data sheet which contains details of each sale made over two years.
The Master Data Sheet included records about all the products being sold.
The columns in the sheet were:
Product Id
Product Name
Category
Unit of measurement
Buying and Selling Price

The Input Data Sheet  included records about all the products being sold.
The columns were:
Date 
Product ID 
Quantity
Sale Type
Payment Mode

The columns in the Input Data sheet were not enough to analyze the data to  answer the stakeholder’s questions.

<br>
<br>

> The **PROCESS** Phase:

I cleaned the data thoroughly and checked for null values in all the columns.
I checked the values in all the records to make sure they were the right data types.

I used the VLOOKUP function to aggregate the data with the master table data.
With the product ID being the primary key.

After aggregation I now had the buying and selling prices involved in each sale.

I used the PRODUCT function to find the Total Buying Value and the Total Selling Value of Each sale.

This data was now clean and adequate hence I proceeded with my analysis to answer the question.

 
<br>
<br>
 
> The ANALYSIS and SHARE Phase:

1.	Using Pivot tables  I analyzed how sales are distributed over the yers and how the sales evolved over the two year period.
   The top 5 selling products are:
  	**Product44**<br>
  	**Product42**<br>
  	**Product41**<br>
  	**Product34**<br>
  	**Product32**
  	<br>
   <br>
   <img width="452" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/b621c290-4060-4e32-80c7-b5311dac701a">
<br>
<br>

2.	For question two I had to find the number of sales made across seasons. With reference to www.britishcouncil.org; the seasons in UK are;
   Spring (March, April and May)<br>
  	Summer (June, July and August)<br>
  	Autumn (September, October and November)<br>
  	Winter (December, January and February)<br>
   I used nested IF statement to group the sales into these 4 seasons.<br>

   By observation ; <br>
   Products from category04 are sold in high quantity across all seasons followed closely by products from category02 and Category05 

   Products from Category03 does not sell in a high quantity across all seasons. Except during the Summer. 
<br>
<br>
      <img width="360" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/02a92feb-c7d6-41f3-b954-b03b5d2797c6">

 <br>
 <br>

3. Overall revenue = Total Selling Value <br>
   The overall revenue in 2021 is **£187284.32**<br>
   The overall revenue in 2022 is **£214127.6** <br>

   There was a significant increase in revenue from 2021 to 2022
 <br>
 <br>
      <img width="445" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/e43223a5-d0f1-4ad8-94d5-d0026756eb3d">

<br>
<br>
      In both years the revenue increases in the last months of the year<br>
      Revenue increased significantly in November of 2021 and October 2022 and falls at the beginning of the year.
      <img width="387" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/35088e21-940f-48c4-a73a-14585f8a8c10">
      <br>
      <br>

 4.	Using Pivot tables, I analyzed the number of sales per day. <br>
      The average sales per day is 75.29 <br>
      Monday: 86 (Higher than the overall average)<br>
      Tuesday: 73 (Slightly lower than the overall average)<br>
      Wednesday: 71 (Slightly lower than the overall average)<br>
      Thursday: 68 (Lower than the overall average)<br>
      Friday: 72 (Slightly lower than the overall average)<br>
      Saturday: 75 (Slightly higher than the overall average)<br>
      Sunday: 82 (Higher than the overall average)
      <br>
      <br>
      <img width="347" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/6707a490-084a-41ff-877b-3de9b7fa0991">
      <br>
      <br>
      There are specific days of the week that tend to have higher sales volumes, with Monday, Sunday, and Saturday being the days with higher sales.
   	<br>
      <br>


  5. 	Profit Margin = (Revenue – Cost of Products)/Revenue * 100 <br>
      I used this formula to create a calculated field in a pivot table.<br>

        Categories 01,03 and 04 recorded a significant increase in profit margin over the two years. <br>

        Category 02 recorded a slight increase in profit margin over the two years.<br>

        Category 05 recorded a significant decrease in profit margin.<br>
        <br>

        <img width="358" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/396be77e-33fe-41b7-8adb-3e47db0a8dce">
   <br>
   <br>

   6. Price elasticity of the products in the various categories is not calculable because the prices of the products in the data did not change over the two years.

   



  
        





 




 
