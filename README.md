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
A friend who has is interested in opening a Bike Store as

He wants to get a head start and conduct research about how a as he is worried about struggling to become profitable due to his inexperience in running a business and lack of knowledge about the products that are associated with biking.


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

![Profit Margin by Product Category](Graphs/Profit_Margin_by_Product_Category.png)
![Sales by Age Group](Graphs/Revenue_by_Age_Groups.png)
![Revenue by Country](Graphs/Revenue_by_Country.png)
![Revenue by Product Category](Graphs/Revenue_by_Product_Category.png)
![Sales Count per Country](Graphs/Sales_Count_per_Country.png)
![Sales Count per Month](Graphs/Sales_Count_per_Month.png)
![Sales Count per Year](Graphs/Sales_Count_per_Year.png)
![Top 50 Products by Quantity Sold](Graphs/Top_50_Products_by_Quantity_Sold.png)






