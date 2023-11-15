# Maven Market Project - Analyzing Data of a Grocery Chain Firm
## Introduction

![](MavenMarket.png)

This Project Case is part of the Microsoft Power BI Desktop for Business Intelligence Course on [Udemy](https://www.udemy.com/course/microsoft-power-bi-up-running-with-power-bi-desktop/) online platform by Maven Analytics. In this case, I worked with data from **Maven Market**, a multi-national grocery chain with locations in **Canada, Mexico** and the **United States**. I worked through the entire business intelligence workflow: **connecting and shaping the data, building a relational model, adding calculated fields, and designing an interactive report**.

## Problem Questions

## Datasets
There are 7 Datasets used in this project, i.e.:
1. Customer Table Dataset (MavenMarket_Calendar.csv)

| Field Name | Data Type |
| ------ | ------ |
| customer_id | Whole Number|
| customer_acct_num | Text |
| first_name | Text |
| last_name | Text |
| customer_address | Text |
| customer_city | Text |
| customer_state_province | Text |
| customer_postal_code | Text |
| customer_country | Text |
| birthdate | Date |
| marital_status | Text |
| yearly_income | Text |
| gender | Text |
| total_children | Whole Number |
| num_children_at_home | Whole Number |
| education | Text |
| acct_open_date | Date |
| member_card | Text |
| occupation | Text |
| homeowner | Text |
| full_name | Text |
| birth_year | Text |
| has_children | Y/N |

2. Products Table Dataset (MavenMarket_Products.csv)

| Field Name | Data Type |
| ------ | ------ |
| product_id | Whole Number |
| product_brand | Text |
| product_name | Text |
| product_sku | Text |
| product_retail_price | Decimal Number |
| product_cost | Decimal Number |
| product_weight | Decimal Number |
| recyclable | Decimal Number |
| low_fat | Decimal Number |
| discount_price | Fixed Decimal Number (Currency) |
  
3. Calendar Table Dataset (MavenMarket_Calendar.csv)

| Field Name | Data Type |
| ------ | ------ |
| date | Date |
| Start of Week | Date |
| Name of Day | Text |
| Start of Month | Date |
| Name of Month | Text |
| Quarter | Whole Number |
| Year | Whole Number |

4. Regions Table Dataset (MavenMarket_Regions.csv)

| Field Name | Data Type |
| ------ | ------ |
| region_id | Whole Number |
| sales_district | Text |
| sales_region | Text |

5. Stores Table Dataset (MavenMarket_Stores.csv)

| Field Name | Data Type |
| ------ | ------ |
| store_id | Whole Number |
| region_id | Whole Number |
| store_type | Text |
| store_name | Text |
| store_street_address | Text |
| store_city | Text |
| store_state | Text |
| store_country | Text |
| store_phone | Text |
| first_opened_date | Date |
| last_remodel_date | Date |
| total_sqft | Whole Number |
| grocery_sqft | Whole Number |
| full_address | Text |
| area_code | Text |

6. Transaction Table Dataset (MavenMarket_Transactions_1997 & MavenMarket_Transactions_1998.csv)

| Field Name | Data Type |
| ------ | ------ |
| transaction_date | Date |
| stock_date | Date |
| product_id | Whole Number |
| customer_id | Whole Number |
| store_id | Whole Number |

7. Return Table Dataset (MavenMarket_Returns_1997-1998.csv)

| Field Name | Data Type |
| ------ | ------ |
|return_date | Date |
| product_id | Whole Number |
| store_id | Whole Number |
| quantity | Whole Number |

## Connecting and Shaping the Data

There are several steps in this phase in order to connect and shape the Data used in this case.

**1. Update Power BI options and settings by:** 

- Deselecting the "Autodetect new relationships after data is loaded" option in the Data Load tab
- Making sure that Locale for import is set to "English (United States)" in the Regional Settings tab

**2. Connect to the MavenMarket_Customers csv file by:

- Naming the table "Customers", and making sure that headers have been promoted
- Confirming that data types are accurate (Note: "customer_id" should be whole numbers, and both "customer_acct_num" and "customer_postal_code" should be text)
- Adding a new column named "full_name" to merge the the "first_name" and "last_name" columns, separated by a space
- Creating a new column named "birth_year" to extract the year from the "birthdate" column, and format as text
- Creating a conditional column named "has_children" which equals "N" if "total_children" = 0, otherwise "Y"

## Building a Relational Model

## Adding Calculated Fields

## Building Interactive Report
