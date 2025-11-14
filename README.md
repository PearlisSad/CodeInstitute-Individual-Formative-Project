Data set from: https://www.kaggle.com/datasets/serhatabuk/sales-data-csv

# Code Institute Data Analysis and AI: Individual Formative Project

This projects analyses dataset(found [here](https://www.kaggle.com/datasets/serhatabuk/sales-data-csv)) about a bike store based in Europe.
My goal was to find insdight through data about which products sell the most, which customers to appeal to the most and have a good sense of
which products to stock in order to generate the most profit.

## Setup
- To Create Virtual Environment `python -m venv venv`
- Activate Virtual Environment `venv\Scripts\activate` (windows) or 'source venv/bin/activate' (mac)
- Install dependencies using `pip install -r requirements.txt`

## Python Data Analysis/Visualisation Modules
 - **Numpy**:
 - **pandas**:
 - **matplotlib**:
 - **plotly**:
 - **seaborn**:

## User Story
A friend who has is interested in taking over his father's bike store as his father has stated that he would want to retire in the next 5 years.

He wants to get a head start and conduct research about which products to keep inventory of and how to prepare and study how these products are affected by the general demand.

In order to assist him in the research, I have found a data set about bike store sales in Europe to see if there are particular trends and patterns to look out for in order to keep the business running and maximising the profits to be earned.


## Data Set
| Column             | Data Type | Description                                      |
|--------------------|-----------|--------------------------------------------------|
| Date               | object    | Raw date string for the transaction             |
| Day                | int64     | Day of month         |
| Month              | object    | Month name                   |
| Year               | int64     | Year of the transaction                         |
| Customer_Age       | int64     | Age of the customer                             |
| Age_Group          | object    | Customer age group category                     |
| Customer_Gender    | object    | Gender of the customer                          |
| Country            | object    | Country of the transaction                      |
| State              | object    | State or region                                 |
| Product_Category   | object    | High-level product category                     |
| Sub_Category       | object    | Subcategory of the product                      |
| Product            | object    | Product name                                    |
| Order_Quantity     | int64     | Number of units ordered                         |
| Unit_Cost          | int64     | Cost per unit                                   |
| Unit_Price         | int64     | Selling price per unit                          |
| Profit             | int64     | Profit from the transaction                     |
| Cost               | int64     | Total cost of the order                         |
| Revenue            | int64     | Total revenue from the order                    |

### ETL process

EXTRACT
- loaded dataset, "sales_data.csv".

TRANSFORM
- Checked for missing values.
- Adjusted Date column into DateTime data type.
- Created "Calculated_Cost" column.
- Created "Calculated_Revenue" column.
- Created "Season" column.
- Created "Profit_Margin" column.

LOAD
- generated "clean_sales_data.csv".

## Insights

![Profit Margin by Product Category](Graphs/Profit%20Margin%20by%20Product%20Category.png)
- This tells us that 'Accessories' are the product category which has the most product margin.
- While having a bike is obviously important in order to participate in the activity, accessories could be more important to have alongside.

![Sales by Age Group](Graphs/Revenue%20by%20Age%20groups.png)
- This tells us that Adults and Young Adults are the majority of the people that purchasing from the store.
- This implies that Adults and Young Adults are the customers we need to market to.
- However, it is unsure whether this bike store is mostly online or not which could explain why the Seniors are not purchasing products.

![Revenue by Country](Graphs/Revenue%20by%20Country.png)
- This tells us that the United States and Australia are the countries that most revenue is generated.
- This could tell us that the environment in these countries may allow for bikes to be used effeciently.
- This also highlights which countries may use the services of the bike store more.

![Sales Count per Country](Graphs/Sales%20Count%20per%20Country.png)
- As expected from before, the United States and Australia are the top 2 countries that generate individual sales from the store.
- However, the United States have a significant upperhand in terms of sales.

![Revenue by Product Category](Graphs/Revenue%20by%20Product%20Category.png)
- While it was found that Accessories have the most profit margin out of all product categories, Bikes generate the most revenue for the store.

![Sales Count per Month](Graphs/Sales%20Count%20per%20Month.png)
- There is a trend found over the years of which months generate the most sales per month over a year.
- There seems to have the most sales around the end of Spring and start of Summer, which is then followed by a decline in July.
- This tells us it would be best to not restock around the months between July - October.

![Sales Count per Year](Graphs/Sales%20Count%20per%20Year.png)
- This illustrated a significant increase in sales per year between 2012 and 2013.
- This could be due to the store being more well known and therefor people are able to purchase products.

![Top 50 Products by Quantity Sold](Graphs/Top%2050%20Products%20by%20Quantity%20Sold.png)
- This tells us the 50 most sold products.
- There is a significant amount of Accessories and Clothing products.
- This highlights which products may need to be restocked more often than others as they seem to have more demand that the other products.

### AI Usage
I have used Generative AI to aid me in this project, however I have explicitly requested that it would only help me in debugging code and explanations and that it would NOT provide any help in gaining insights and analyse the dataset I have.






