# Retail Dashboard

This is a dashboard with multiple interconnected idioms as follows:
1. Bar Chart; 
2. Stacked Area Chart;
3. Slopegraph; 
4. Treemap; 
5. Wordcloud; 
6. Line Chart; 

Scripting: D3

Parent Dataset (although modified): https://www.kaggle.com/frtgnn/dunnhumby-the-complete-journey?select=product.csv

In accordance with the dataset, following are the questions we are trying to answer through this project:
● Which dept or class (of products) appealed most to the different customer age groups in 2007? or in 2008?
● What was the 'brand' popularity among customers belonging to different income levels in 2007? or in 2008?
● What’s the monthly trend in sales for 2007? or for 2008?
● Were the total sales per year (per dept) in 2008 more than those of 2007?
● Which Countries are stronger/weaker on profits? ● Does giving discounts improve the sales?


ABSTRACT
“Retail sales tracks consumer demand for finished goods by measuring the purchases of durable and non-durable goods over a defined period of time.” (https://www.investopedia.com/terms/r/retail-sales.asp)
It’s important for a company to keep track of its profits and sales so that they know which of their products are generating revenue, the influence of the type of product brand regarding the sales, in which country or city they should be investing more or even stop investing, which departments are generating more profit and if the customer age group or the customer income level impact on the sales.
With our project and visualization we aim to provide answers to these questions by showing multiple idioms, all connected between themselves, that take into account variables like, “Month”, “Country”, “Brand”, “Year”, “Customer Income Level”, “Department”, “Customer Age Group”, and more variables that we will show in future sections of this report.
Author Keywords
Retail; Sales; Profits; Pricing;

INTRODUCTION
Retail is an everyday affair for everyone and has been so for a really long time. From Mom&Pop stores to Giant Retailers, everybody is trying to go digital for all their processes - from POS to their merchandising solutions and hence ‘data’ has become the centre for everything. Be it demand forecasting, or budgets, or pricing strategies or even the in-store product display takes into account the past sales and profit trends. And exactly this is what we planned to explore with our project.
Interesting enough to bring all 3 of us onboard, while we were still struggling to find a feasible dataset for other under-consideration ideas that matched our combined interest, the Retail-POS dataset we finalised (aggregated at the week level) came in handy.

In accordance with the dataset, following were the questions (refined over the course) we decided to answer through this project:
● Which dept or class (of products) appealed most to the different customer age groups in 2007? or in 2008?
● What was the 'brand' popularity among customers belonging to different income levels in 2007? or in 2008?
● What’s the monthly trend in sales for 2007? or for 2008?
● Were the total sales per year (per dept) in 2008 more than those of 2007?
● Which Countries are stronger/weaker on profits? 
● Does giving discounts improve the sales?

We wanted to answer these questions because none of the visualizations we found when we were doing research for this project answered all of them. This is further explained in the “related work” section.
As we said before, what we expected by going with this approach is to know how a person’s income level and age affect the type of products they buy, how the number of sales changes in the different months of the year and in the different countries where the store operates.
Our aim was to create a dashboard where the user could see all of this information in one screen, see the evolution of sales in the different months, see what departments sell more and see the products that sold the most given in each category that the user wants to see. The user can also see the effect of the discounts on the sales of a given product.

RELATED WORK
When we were doing the research for our project we found different visualizations that were related to our project but they were composed by a single graph, most of them with no interactivity where we could only see a specific aspect of that specific store or product, like the one on figure 1.

What we wanted was a dashboard that showcased the information for all the aspects of the store. We wanted the user to have information on the type of customers the store as, what are the trends in sales over the months, see how much a discount affects the sales of a products, and what are the most popular products in the different departments and different sub departments (that we call classes) and also what type of brand the customers prefer overall.
We could only find graphs that showed the attributes that we wanted to show individually, we could not find a connected dashboard that showed in depth information about a specific store and its customers.
The graphs that are found online only showed a limited amount of data and in all the years of experience dealing with datasets and information on sales and retail revenue there were no graphs that connected the different data collected from a store.

THE DATA
Retail Dashboard is based on a subset of retail sales dataset (https://www.kaggle.com/frtgnn/dunnhumby-the-complete-j ourney?select=product.csv) however sliced and/or aggregated at different levels.
It essentially has following linked entities
1. Product:
a. The smallest saleable unit in retail
b. It has a 3 level hierarchy
i. Products are grouped into sub classes
ii. Sub classes are grouped into Classes
iii. Classes are group into Departments
2. Stores:
a. Only Physical stores
b. Grouped at the Country level
3. Customer
a. Customer is essentially who buys the
products at a store
b. Customers are global here - no
relationship between stores and customers
c. Customer Database is maintained and has
essentially
i. Customer Ids
ii. Customer Age groups
iii. Customer Income Levels
and several different datasets were built for different types of idioms.

VISUALIZATION
Overall Description
Our Retail Dashboard essentially can be seen split into 2 sections each has its own set of filters and visualises different levels of info, although based on the same dataset.
On applying necessary filters, the upper-part of the dashboard can give out info on and/or comparisons for:
 1. Total Sales per Month per filtered Year per filtered Customer Age Group (ordered by Month)
 2. Total Profits per Month per filtered Year per filtered Customer Age Group (ordered by Month)
 3. Total Sales per Country per filtered Year per filtered Customer Age Group (ordered by Country Name)
 4. Total Profits per Country per filtered Year per filtered Customer Age Group (ordered by Country Name)
 6. Comparison Sales for each Brand for various customer-income-level-groups per filtered Year, per filtered Customer Age Group
 7. Comparison Profits for each Brand for various customer-income-level-groups per filtered Year, per filtered Customer Age Group
 8. Comparison Sales for each Department (of product) for 2007 and 2008 per filtered Customer Age Group
 9. Comparison Profits for each Department (of product) for 2007 and 2008 per filtered Customer Age Group
10. Comparison Sales or distribution over containing classes (of products) per filtered Year per filtered Customer Age Group
11. Comparison Profits or distribution over containing classes (of products) per filtered Year per filtered Customer Age Group
12. Top Selling Products of the company per per filtered Year per filtered Customer Age Group
13. Top Profit-making Products of the company per per filtered Year per filtered Customer Age Group

While on the lower part:
The line chart shows “What would have been the sales” ( per filtered Product over the weeks of the filtered Year-Quarters ) if there was no discount on the weeks when there was a discount. Essentially it gives out the actual quantity vs the projected quantity if there was no discount on that week.
