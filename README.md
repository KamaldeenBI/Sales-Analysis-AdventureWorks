# Prodect Title: Sales-Analysis-AdventureWorks
# Project objective: 
Sales performance analysis provides several significant advantages to businesses and this includes identifying areas for improvement, tracking progress, as well as increasing revenue. I analyzed data from the adventure works database and carried out a Sales Performance Analysis. 
Adventure works is a large multinational manufacturing company that produces and distributes bicycle parts and accessories for commercial markets in north America, Europe, and Asia. 
The company has a staff strength of 500 workers
Additionally, Adventure Works employs several regional sales teams throughout its market base.
Adventure works have the following business questions:
1. The current market demand for the company’s products
2. The variation of sales from country to country, critically examined.
3. The current sales performance and how it compares to the past performance and industry benchmarks


# Steps taken towards the completion of this project include:
1.Install database backup
2.Read through requirements and prepare user user story
3. Identify required tables
4.Clean tables and create views
5 connect to views in power query
data transformation in power query
data modelling
create mearsures
Data vizualization
publish to powerbi service and github

# Data Transformation
The required tables that houses relevant data based on business questions at hand were queried by connecting to the Adventure works SQL database from within Power BI using import mode. 

![Screenshot (343)](https://user-images.githubusercontent.com/108130729/232272517-be526511-4692-428a-9373-594db696fcfd.png)

Loaded the select tables to Power Query editor due to  intent to transform the data and prepare it for modelling to achieve general optimal performance. 

![Screenshot (345)](https://user-images.githubusercontent.com/108130729/232272525-3e00e7a8-9f49-476c-9eb6-886a048c9898.png)


The conventional system of how the company stores Customer data wouldnt have allowed for a star schema in the Data modelling because fields like 'customer locations and sales regions have a separate table that houses them, the DimGeography' table which will force us to connect two dimensions table together which is not a standard practice towards achieving a star schema in Data Modelling. I therefore had to do a merge of four tables into two, all fields still co-existing except columns that won't be necessary for the current analysis project.
Dropped unwanted columns which will help reduce file size and increase performance, removed duplicates, Replaced values that were based on acronyms to standardize results of analysis, transformed the preloaded data table into a usable format that will help in historical analysis and forcasting sales as the business requests.

![Screenshot (353)](https://user-images.githubusercontent.com/108130729/232272586-5438cbef-eca9-4aed-9cff-07ee087ba78b.png)

Then applied all changes and loaded to Power BI desktop

Next step was to create relationships between the tables in the model view wihin PowerBI. I connected all dimension tables using the primary keys in each of those tables to match the corresponding foreign keys that existed in the fact table (FactInternetSales)

![Screenshot (375)](https://user-images.githubusercontent.com/108130729/232272593-1b29a928-9ab1-4c34-ab06-435482dd563b.png)

Created a new separate table to house mearsures that would be created for analysis to that it doesnt become defficult locating them when trying to find patterns and draw insights fromv the data. It also helps the structure look neat so that any third party looking to work with the file can easily comprehend the arrangements

# Results of Analysis
Recall, The business questions
1. The current market demand for the company’s products
2. The variation of sales from country to country, critically examined.
3. The current sales performance and how it compares to the past performance and industry benchmarks

Below is the created report to answer the three business questions critically on demand because of its intractive nature, each visual communicates with the others an the use of drilldown on some of the visuals will give the user a more detailed answer to their enquiries on the findings.

![Screenshot (392)](https://user-images.githubusercontent.com/108130729/232272622-20edfce4-6d13-4228-821d-edc33bb0fb60.png)

![Screenshot (384)](https://user-images.githubusercontent.com/108130729/232272634-fe66752a-9755-48e2-a1de-c1a145b2cef4.png)

![Screenshot (385)](https://user-images.githubusercontent.com/108130729/232272635-6747fc60-344f-4e09-961a-585dcd256e38.png)

![Screenshot (386)](https://user-images.githubusercontent.com/108130729/232272639-5686ab96-56f8-43bb-95bb-256a3f3c6a18.png)

![Screenshot (387)](https://user-images.githubusercontent.com/108130729/232272646-c62070a3-e71f-4438-be7a-fae62b6a5898.png)

![Screenshot (388)](https://user-images.githubusercontent.com/108130729/232272650-b0eabe32-5d1f-4cfb-ab51-c1e53e5756f9.png)

![Screenshot (389)](https://user-images.githubusercontent.com/108130729/232272670-df6b65cf-94d7-4fbd-853e-e7a9ddaabceb.png)

![Screenshot (391)](https://user-images.githubusercontent.com/108130729/232272675-16ca8cf9-821e-443a-87c9-4d57bc7ca90e.png)





Recommendations
