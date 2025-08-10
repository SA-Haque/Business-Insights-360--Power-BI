# Business Insights 360 - Power BI
I have worked on this Project while learning the Power BI course with codebasics. Link to the [Power BI](https://codebasics.io/courses/bootcamp/1/power-bi-data-analysis-with-end-to-end-project/lecture/1522) course.

Link to  [Interactive Dashboard](https://app.powerbi.com/view?r=eyJrIjoiMTRjMzQzYWItMzFmYi00NmM2LWJjMGQtMmEyNWMzYmI1M2M2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

---

# About the Company

 **AtliQ Hardware** is a hardware manufacturer company. They make hardware like PCs, Mice, laptops, and so on, and sell it to different customers like Croma, Best Buy, Staples, and even online stores like Amazon & Flipkart & these stores sell these products to the end consumers. AtliQ business has in different countries, for these, they have 3 different channels to sell this product **Retailer** (Croma, Amazon), **Direct** (AtliQ Exclusive, AtliQ e-store), & **Distributer** (Neptune).

 ---

 ### Problem Statement
 **AtliQ Hardware** has become one of the most fastest-growing companies, but they faced some bitter experiences in Latin America. They tried to establish their presence in Latin America, but they faced huge losses, because their decision to open their shop in Latin America had to be made based on some random surveys & data based on Excel files. Now, AtliQ hardware has decided to onboard a *Data Analytics* team to take accurate  data-driven decisions.

### Goal Of this Project

The goal of this project is to implement an advanced analytics solution using Power BI which covering all the departments (Sales, Finance, Marketing, Supply Chain & Executive)  which will help AtliQ Hardwares transform their raw data into actionable insights and enable the leadership team to take faster, data-driven decisions to support business growth.

---

 ### Data Model
 - Data Modeling plays a vital role in Analysis and is considered as the basement of the report. All the analysis will be done, based on the data Model.
 - Poor data modeling will **lead to inaccurate analysis, slow performance, data redundancy, and difficulties in maintaining or scaling the system**. Refer to this: [What is Data Modeling](https://www.microsoft.com/en-in/power-platform/products/power-bi/topics/data-modeling/what-is-data-modeling) for good Practice.
 - In this Project, we have followed the Snowflake Schema data model method --> [What is Snowflake Schema](https://www.databricks.com/glossary/snowflake-schema)

<img width="1289" height="775" alt="Adobe Express - file (2)" src="https://github.com/user-attachments/assets/4e119f42-cf5b-4982-8f1a-6cbfafae4c0c" />

### Key Metrics Tracked
* **Net Sales** 
* **Gross Margin** 
* **Net Profit**
* **Net Profit %** 
* **Net Error**
* **Forecast Accuracy**
* **ABS Error** (Absolute Error)

---

### Learning through this Project

**Tech Stacks**:

- SQL
- Power BI
- Excel
- DAX (Data Analysis Expression)
- DAX Studio (for optimizing the report)
- Project charter file (for gathering the requirements from the Stakeholders)

**In Power BI** :

- What are all the questions that should be asked before starting the project
- Creating calculated columns
- Creating a measure using DAX language
- Data modeling
- Using Bookmarks to switch between two visuals
- Page navigation with buttons
- Using the divide function to prevent zero division errors
- Creating a date table using Power Query
- Dynamic titles based on the applied filters
- Using KPI indicators
- Conditional formatting of the values in visuals using icons or background color
- Data validation techniques
- About Power BI services
- Publishing reports to Power BI services
- Setting up a personal gateway to set up the auto-refresh of data
- Power BI App creation
- Collaboration, workspace, and access permissions in Power BI services
- And many more 😊

**Business Related Terms** :

- Profit & Loss Statement (Gross Price to Net Profit)
- Fiscal-Year & Quarter (For Time intelligence Analysis)
- Forecast Accuracy, Net Error, ABS Error (Supply Chain Metrics)
- Market Share % 
- YTD - Year to Date
- YTG - Year to Go
- Direct
- Retailer
- Distributors
- Consumer

---

### Questions should be asked before starting the projects :

- What is the objective of building this Power BI dashboard?
- In what terms will the success of this project be measured?
- What will be the deadline of the project?
- Do the stakeholders expect a preview before the actual release?
- What are all the hopes stakeholders have for this project?
- What are all the fears the stakeholders have in terms of building this dashboard?
- Who all will be using this dashboard and for what purpose?
- What are all the expectations the stakeholders have by the completion of this project?
- What can go wrong while building this project?
- What are all the resources/ data needed to build this dashboard?
- Are there any inputs from stakeholders in terms of design and views of the dashboard?
- And many more based on the requirement.

---

# Understanding of Data :

Understanding what data is available will be more helpful while doing the analysis. before jumping into the analysis get good understanding of what are data available.

**Dimension table:** It will have the static data, like details of customers and products

**Fact table:** It will have the data about the transactions


### Dim_customer
- 27 distinct markets (ex, India, USA, Spain)
- 75 distinct customers throughout the market

**2 types of platforms**
- Brick & Motors - Physical/offline store
- E-commerce - Online Store (Amazon, Flipkart)

**Three channels**
- Retailer
- Direct
- Distributors
  
### Dim_market
- 27 distinct markets (ex, India, USA, Spain)
- 7 sub-zones

**4 Regions**
- APAC
- EU
- nan
- LATAM
  
### Dim_product
- There are 14 different categories, like Internal HDD, keyboard
- There are different variants available for the same product

**Divisions**

 *1. P & A*
   
   - Peripherals
   - Accessories
 
 *2. PC*
    
   - Notebook
   - Desktop
 
 *3. N & S*
    
  - Networking
  - Storage

### fact_forecast_monthly
- This table is used to forecast the customer’s needs in advance, which can help in

    *Higher customer satisfaction*

   *Reduced cost in warehouses for storage purposes*

- The table is denormalized by data engineering team, as it is a data warehouse which is aimed to be used for analytical work.
- All the date of the month will be replaced by the start date of the month
- It will have all the column names, and in the end, it will have the forecast quantity needed for the customer

### fact_sales_monthly

- This table is more or less is same as fact_forecast_monthly table, but the last column has the value of sold quantity instead of the forecast value.

### freight_cost

- This table has details of travel costs and other costs for each market for the fiscal year

### gross_price

- Has the details of gross prices with the product code

### manufacturing_cost

- Has the details of manufacturing cost with product code with year

### Pre_invoice_dedutions

- Has the details of pre-invoice deductions percentage for each customer for each year

### Post_invoice_deductions

- Post invoice deductions and other deductions details

---



 ### Home Page
 From here, we can navigate to different pages of the report
 
 <img width="1542" height="868" alt="Screenshot 2025-08-05 195001" src="https://github.com/user-attachments/assets/005442f3-811d-494f-8f9a-da3920121f72" />

  ### Finance View
  <img width="1763" height="988" alt="Screenshot 2025-08-10 234604" src="https://github.com/user-attachments/assets/bdfe1968-c964-4f8d-ba93-49e837c46a04" />

   ### Sales view
   <img width="1759" height="981" alt="Screenshot 2025-08-10 234628" src="https://github.com/user-attachments/assets/32f2c4c9-9e53-4a19-a4ad-fd94fb571922" />

   ### Marketing View 
   <img width="1757" height="991" alt="Screenshot 2025-08-10 234657" src="https://github.com/user-attachments/assets/b51fdb4e-44ca-4181-9a5c-63dca923530e" />

   ### Supply Chain View
  <img width="1759" height="992" alt="Screenshot 2025-08-10 234718" src="https://github.com/user-attachments/assets/34270105-aa17-4762-a0ff-3cb054120e0d" />

   ### Executive View 
  <img width="1744" height="989" alt="Screenshot 2025-08-10 195919" src="https://github.com/user-attachments/assets/853bae1a-87b8-4806-a4bb-2df07a45711f" />

  ### Info page
  <img width="1760" height="993" alt="Screenshot 2025-08-10 234800" src="https://github.com/user-attachments/assets/4bfe52af-e330-464f-8705-917f1512b634" />


You can find full report here : [Report](https://app.powerbi.com/view?r=eyJrIjoiMTRjMzQzYWItMzFmYi00NmM2LWJjMGQtMmEyNWMzYmI1M2M2IiwidCI6ImM2ZTU0OWIzLTVmNDUtNDAzMi1hYWU5LWQ0MjQ0ZGM1YjJjNCJ9)

---

# Project Outcome

Business Insights 360 is a multifunctional dashboard that provides a comprehensive view across various departments, including Finance, Sales, and more, to support the company in making data-driven decisions.

---


















### 📬 Contact

If you have any questions or feedback, feel free to reach out via:

* E- mail: \[s.a.haque.analyst@gmail.com]
* LinkedIn: \[https://www.linkedin.com/in/shahbaz-ali-haque/]
