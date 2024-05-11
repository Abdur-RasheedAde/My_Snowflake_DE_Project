# Cricket Analaysis Project with Snowflake

![Slide1](https://github.com/Abdur-RasheedAde/Snowflake_Projects/blob/main/SNOWFLAKEHOME.png)

##  Introduction
This is a Big Data-Data Engineering (End-to-end) project exploring snowflake cloud. The project injest a json file, perform all necessary ETL processes and created a Snowflake dashboard to visualise the data. 

## Data Source:
The data used is a Cricket World Cup match in 2023 which comes in a json file injested directly from a folder;  
* Cricket World Cup Match in 2023 [Downloadjsonfilehere](https://drive.google.com/drive/folders/1ls9ST-q6c2fCZZOuaC8Bd5lugrTKbVIE?usp=drive_link)

## DE Technical Skills:
+ Schema Creation
+ Data Injestion
+ Data Warehousing
+ Extract, Transform and Load (ETL) process
+ Flattering of JSON file into a Table
+ Data Modelling (Fact and Dimention table)
+ Data Visualization - dashboard
+ Feedback and Continuous Improvement
  
## Data Engineering Process
1. Creation of database and 4 Schemas: A database (DB) known as CRICKET is created with 4 Schemas (LAND, RAW, CLEAN and CONSUMPTION) for proper logical description and arrangement of the DB. The Star-schema was eventually used in Data Modelling so as to give the datawarehouse a legible understading (get the code here)[] 
2. Data Injestion and Loading: Data is injested into the LAND schema and reloaded into the RAW schema (access the code here)[]
3. Flattening of Data: Since the data uploaded are ojects, they need to be flatenned so as to create the CLEAN proper column based table (get code here)[]
4. Creation of Player and Country table: This is achieved by flattening the json objects in the RAW schema to create a Player and Country column Table (get code here). These 2 tables are connected with the help of a primary and foreign key respectively (get code here)[] 
5. Extract Data from Inning Array: This is another strategy of the ETL process to transform an array into a proper column based table. This is used to get the Delivery clean Table
6. Data Validation: There is an absolute need to check the degree of correctness of a data after the whole ETL process (get code here) [] 
7. Creation of Dimention Tables: 5 Dimention tables are created including referee_dim, team_dim, player_dim, venue_dim and match_type_dim tables while poluating data into them and establishing different relationship between them as well
8. Creation of Date Dimention Table: A date dimention table is also created so as to link it to the match_fact_table
9. Creation of Fact_Tables: 2 Fact tables are created Match_type and Delivery tables and are both populated with data

## Report Design and Visualization
The Report Canvas was designed in Power Point and imported to PowerBI as canvas background. Here is a sample of the slide in Power Point   
<img src="https://github.com/Abdur-RasheedAde/Financial_Report/blob/main/Slide2.PNG" width=50% height=50%>  
5 pages were created; Home, Consolidated, Stationery, Cosmetics and Electronics. 
_Home_ page is the landing page while _Consolidated_ has the general report without filter while other pages has filtered reports accroding to their page name.
On each page, the new card visual is used to hold Total Sales, Gross Sales and Profit, Line Chart is used for the series analysis while a column and bar chart are adopted for the Continental and Country analysis respectively. The last image is the button for page navigation. 

## Conclusions and Recommedations

1. Haut needs to conduct market analysis to increase sales in Q1 and Q2 and offer seasonal products that appeal to customers in the first half of the year
2. Haut’s management should continue their market strategy that leads to higher profits and better customer satisfaction
3. The cosmetics product category demands more research and development to boost its sales and profitability
4. Promotions (discounts) drive most of the sales in Haut stores, making them competitive in the dynamic market. Therefore, other promotional and marketing strategies should be implemented to enhance sales and profit
5. Products in Africa and China stores should be tailored to the specific needs of these markets through careful research

## Deployment to Power BI Service
This Report is deployed to Power BI service from my Microsoft developer account and publish to the web for everyone to have access to it.
[HautSupermarketAnalysis](https://app.powerbi.com/groups/me/reports/66ab0071-4b25-41c8-99fd-fd006603aacd/ReportSection6239a8326550e132bae6?ctid=32796be2-60fb-4da2-8d26-06e5938e6e6b&experience=power-bi)  

To Open a developer Microsoft account, kindly check this article [OpenMicrosoftdeveloperaccount](https://techcommunity.microsoft.com/t5/educator-developer-blog/register-for-microsoft-365-and-power-apps-developer-account-with/ba-p/3490280)

Thanks for taking time to go through this report! 🤝
