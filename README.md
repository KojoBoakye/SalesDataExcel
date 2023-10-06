# SalesDataExcel
Analysing sales data in spreadsheet (Excel)

## Goals and Purpose:

The primary goal of the "Sales Data Analysis" project was to identify and and gain valuable insights in a company's sales data to answer some stakeholder questions.

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
<img width="452" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/b621c290-4060-4e32-80c7-b5311dac701a">

2.	For question two I had to find the number of sales made across seasons. With reference to www.britishcouncil.org; the seasons in UK are;
   Spring (March, April and May)<br>
  	Summer (June, July and August)<br>
  	Autumn (September, October and November)<br>
  	Winter (December, January and February)<br>
I used nested IF statement to group the sales into these 4 seasons.<br>

By observation ; <br>
Products from category04 are sold in high quantity across all seasons followed closely by products from category02 and Category05<br>

Products from Category03 does not sell in a high quantity across all seasons. Except during the Summer. <br>
<img width="360" alt="image" src="https://github.com/KojoBoakye/SalesDataExcel/assets/82205211/02a92feb-c7d6-41f3-b954-b03b5d2797c6">

 




 
