# PowerBI-Project---Business-Insights-360


## Project Overview

AtliQ Hardware is growing rapidly in the recent years, and they have decided to implement the data analytics using PowerBI in their company for the first time to surpass their competitors in the market and to make data driven decisions. This project is hoped to give answers to the questions of stakeholders in terms all the aspects like Finance, Sales, Marketing, Supply Chain, etc.

# Live Report Link in the "About" Section 👉

## Tech stacks

- SQL
- PowerBI Desktop
- Excel
- DAX Language
- DAX studio (for optimizing the report)
- Project charter file

## PowerBI Techniques Learnt

- What are all the questions should be asked before staring the project?
- Stakeholder Management
- Creating calculated columns &  measures using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using divide function to prevent zero division errors
- creating date table using "m" language
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting the values in visuals using icons or background color
- Data validation techniques
- PowerBI services
- Publishing reports to PowerBI services
- Setting up personal gateway to set up the auto refresh of data
- PowerBI App creation
- Collaboration, workspace, access permissions in PowerBI services
- And many more 😅

## Business Related Terms

- Gross price
- Pre-invoice deductions
- Post-Invoice deductions
- Net Invoice sales
- Gross Margin
- Net sales
- Net profit
- COGS - Cost Of Goods Sold
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumers

## Company’s Background

AltiQ hardware is a company which has grown vastly in the recent years, and opened business all over the globe. It is a company which sells, computer and computer accessories through three mediums/channel

- Retailers
- Direct
- Distributors

Recently the company has faced a unforeseen loss by opening store in Latin America based on the surveys, intuition and some excel analysis and also the company’s competitors has handful of analytics team to perform analysis and make data driven decision. So, the AltiQ hardware has no other option other than building their analytics team for data driven insights and decisions in the future to survive better in the industry. 

Project kick off session, where you should get clear of for what and why this project and all other questions you have with, regards to the project!!

### A Data Analyst's Strategies & Questions to ask in a Stakeholder meeting!

#### Strategies:

- In what terms the success of this project will be measured?
- do the stakeholders expecting pre-view before the actual release?
- What are all the hopes stakeholders have out of this project?
- what are all fears the stakeholder have in terms of building this dashboard?
- what are all expectation the stakeholders have, by the completion of this project?
- What can go wrong while building this project?
- what are all the resources/ data needed to build this dashboard?

#### Queries:
- What is the objective of building this PowerBI dashboard?
- What will be time dead-line of the project?
- Who are all will be using this dashboard and for what purpose?
- Asking inputs from stakeholders in terms of design and views of the dashboard?

After the project kick off meetings, the data engineering team has given the data as per the request of data analytics team, let’s explore them.

### Dataset **Understanding.**

Understanding what data is available, will be more helpful while doing analysis. before jumping on to the process. 

Dimension table : It will have the static data like details of customers and products

Fact table : It will have the data about the transactions  

- gdb041:
    - dim_customer
        - **27** distinct markets (ex India, USA, spain)
        - **75** distinct customers thorough out the market
        - **2** types of platforms
            - Brick & Motors - Physical/Offline store
            - E-commerce - Online Store (Amazon, Flipkart)
        - Three channels
            - Retailer
            - Direct
            - Distributors
    - dim_market
        - **27** distinct markets (ex India, USA, spain)
        - **7** sub-zones
        - **4** regions
            - APAC
            - EU
            - nan
            - LATAM
    - dim_product
        - Divisions
            - P & A
                - Peripherals
                - Accessories
            - PC
                - Notebook
                - Desktop
            - N & S
                - Networking
                - Storage
        - There are 14 different categories, Like Internal HDD, keyboard
        - There are different variants available for the same product
    - fact_forecast_monthly
        - This table is used to forecast the customer’s need in advance, which can help in
            - Higher customer satisfaction
            - Reduced cost in warehouses for storage purpose
        - The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
        - All the date of the month will be replaced by the start date of the month
        - It will have all the column names and in the end it will have the *forecast quantity* need of the customer
    - fact_sales_monthly
        - This table is more or less is same as *fact_forecast_monthly* table, but the last column has the value of *sold quantity* instead of *forecast value*.
- gdb056
    - freight_cost
        - This table has details of travel cost and other cost for each market with fiscal year
    - gross_price
        - Has the details of gross prices with product code
    - manufacturing_cost
        - Has the details of manufacturing cost with product code with year
    - Pre_invoice_dedutions
        - Has the details of pre invoice deductions percentage for each cutomer with year
    - Post_invoice_deductions
        - Post invoice deductions and other deductions details

## Importing data into PowerBI

- As the database is **MySQL** in this project, we need to import the datasets from Mysql database to PowerBI by providing the Database access credential.

## Data Model

- Data modeling plays a vital role and is considered as the basement of report. All the visuals will be build upon the data model.
- Poor data modeling affects the overall performance of the report.
- Following good practices of data modeling is must. Refer this page to get to know the good practices [Blog](https://addendanalytics.com/blog/data-modelling-best-practices/)
- In this project, we have followed Star Schema data modeling method.

<img src="https://github.com/user-attachments/assets/9b424208-2ca5-4121-b91a-7ab6037c6769" class="center">

### Dashboard designing

Based on the mockups received as requirement, the team will start designing the visuals and create measures as and when required.
(https://github.com/user-attachments/assets/5c4e19f7-9186-49d7-a096-da4fd3e54f04)

## Home view

In Home view, for all the views, button will be available. User will land on specific view page by clicking the button.

- Info
- Finance View
- Sales View
- Marketing View
- Supply chain View
- Executive View
- Support

## Overall Report


"https://github.com/user-attachments/assets/b011feb0-598e-4196-8b37-4b742c67c9c2"



you can find the full report file here In **"About"** section of this Repository.

## Project Outcome

By using this report, decisions can be taken based on the data. Further it will help in answering *n* number of **why** questions based on the situations.

