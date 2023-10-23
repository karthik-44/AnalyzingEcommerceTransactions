# AnalyzingEcommerceTransactions
This [project](https://hicounselor.com/projects/analyzing-e-commerce-transactions-data-cleaning-cohort-analysis-and-sql) is offered by Hicounselor.

### Problem Context
In the fast-changing world of online shopping, our data whiz, Alex, embarked on an exciting journey.  
With Python and SQL as trusted companions, he explored a vast e-commerce dataset in three key phases: 
 - Data Cleanup
 - Cohort Analysis
 - SQL Insights.

### First phase - Data Cleanup with Python  
Alex carefully combed through the dataset, fixing missing information and sorting out errors. He made sure the data was ready for the next steps.  

### Second phase - Cohort Analysis with Python
Alex grouped customers based on their shopping habits and timelines. This revealed secrets about customer loyalty and how people shop online, like deciphering a hidden code.  

### Final phase - SQL Insights
Using SQL, he found answers to important questions. SQL helped Alex find these answers, giving us a full picture of e-commerce questions we expect to find.  
With each line of code and every SQL query, Alex didn't just find answers; he paved the way for smarter decisions. This project wasn't just about numbers; it was about helping e-commerce thrive in a competitive world.  
Join us on this data-driven journey as we follow Alex's steps, revealing the secrets of online shopping success.  
The below are the steps for answering the questions of tasks in each module.  

## Module 1
### Task 1: Polishing the Dataset for Insights
In the realm of e-commerce, data analyst Alex undertook the critical mission of transforming the "transaction_dataset.csv" into a strategic asset. He meticulously cleaned the data to ensure precision, eliminating extraneous columns such as "product_class" and "product_size." Furthermore, he revamped column names to enhance clarity.

The objective of this task was both simple and pivotal: to equip the organization with top-tier data for facilitating informed decision-making. It aimed to create a well-defined pathway towards data-driven insights that would steer the e-commerce platform toward resounding success.




In the ever-evolving realm of e-commerce, our mission is to unravel the intricate tapestry of customer behavior and engagement. We embark on a journey of data exploration and analysis, starting with the meticulous cleaning of our transaction dataset. By isolating and understanding 'Approved' transactions, we aim to uncover the patterns that lead to customer satisfaction and loyalty. Our voyage continues as we delve into cohort analysis, charting the trajectories of customer groups over time. Through these tasks, we seek to decipher the secrets of customer retention, identify growth opportunities, and ensure our e-commerce platform thrives in a dynamic digital landscape. This is a story of data-driven discovery, where each task brings us closer to delivering an exceptional online shopping experience.


## Module 2
### Task 1: Harvesting 'Approved' Transactions
Cohort of Approved Transactions - Filtering for Excellence:

At the heart of any data analysis lies the importance of clean and relevant data. In this first task, we're importing the necessary tools and filtering our dataset to focus exclusively on 'Approved' transactions. This is crucial because it helps us narrow down our analysis to the transactions that are most likely to provide insights into customer behavior and engagement, enabling us to make data-driven decisions.

### Task 2: Transforming Date Data into Month Indices
Once we've filtered our data, the next logical step is to extract and transform the specific information we need. By creating a new DataFrame and introducing features like the transaction date in 'YYYYMM' format and the transaction month index, we're preparing our data for deeper analysis. These features will help us understand when and how customers interact with our platform, laying the foundation for cohort analysis.

### Task 3: Unveiling Cohort Months: Identifying First Transaction Months for Customers
Understanding the concept of cohort months is pivotal for cohort analysis. By determining when each customer joined a cohort, we're segmenting our customer base into meaningful groups. This task is essential because it establishes the basis for tracking customer behavior over time, allowing us to uncover trends and patterns within these cohorts.

### Task 4: Cohort Connection: Merging Transaction Data with Customer Cohort Months
To perform cohort analysis effectively, we need to merge our transaction data with the cohort information. Joining these DataFrames is crucial because it links each transaction to its respective cohort, forming the backbone of our cohort analysis. It enables us to trace how customer behavior changes over time within specific cohorts, providing invaluable insights for strategic decision-making.

### Task 5: Cohort Index Creation: Tracking Customer Transaction Month Relationships
The cohort index represents the customer's journey within their cohort. Calculating this index is significant because it quantifies how long a customer has been a part of their cohort. This information is fundamental to cohort analysis as it allows us to compare the behavior of customers at various stages of their engagement, helping us identify trends and preferences.

### Task 6: Cohort Customer Count Analysis: Building 'final_df' for Insights
This task helps us refine and summarize our cohort data. By creating the 'final_df,' we're simplifying our analysis, making it easier to interpret and visualize. This DataFrame contains the count of customers in each cohort at different time points, giving us a clear picture of customer retention and engagement patterns.

### Task 7: Cohort Data Transformation: Creating 'cohort_data' for Analytical Insights
Cohort analysis involves studying how groups of customers evolve over time. The 'cohort_data' table is instrumental in this endeavor. It organizes customer counts by cohort and time, providing a structured view of customer behavior. This table is essential for creating visualizations and making data-driven decisions about marketing, product development, and customer retention.

### Task 8: Cohort Analysis: Calculating Cohort Percentages for Evolution Insight
Percentages speak volumes when it comes to understanding customer engagement. Calculating cohort percentages allows us to see how each cohort's size changes over time relative to its initial size. This step is crucial because it helps us gauge the effectiveness of our strategies in retaining and engaging customers. Ultimately, it guides us in optimizing our efforts to improve customer loyalty and satisfaction.

## Module 3
### Task 1: Data Download, Import, and Database Connection.

### Task 2: What are the unique brands available in the dataset?
We are enquiring about the unique brands available in the dataset to gain insights into the variety of products and manufacturers present in our sales records. This information can help us understand the market presence and popularity of different brands among our customers.

There are **7** unique brands namely: 
Solex,
Trek Bicycles,
OHM Cycles,
Norco Bicycles,
Giant Bicycles,
WeareA2B,
Nio Cycles.

### Task 3: How many unique customers made transactions in the dataset?
We are investigating the number of unique customers who have made transactions in the dataset to assess the extent of our customer base. Understanding the total count of customers can aid in customer segmentation and targeted marketing efforts to enhance our business's customer relations and profitability.

There are **3494** unique customers.

### Task 4: How many transactions were approved and how many were not approved?
We are examining the number of transactions that were approved and those that were not approved to assess the overall success rate of transactions in our dataset. This information helps us evaluate our operational efficiency and customer satisfaction, as well as identify any potential issues that may require attention to improve the approval process.

Found **19821** approved transcations and **179** unapproved transactions.

### Task 5: List the top product lines with the highest average list price.
We are inquiring about the top product lines with the highest average list price to identify the product categories that generate the highest revenue for our business. This knowledge can guide pricing strategies and marketing efforts, as well as help us understand customer preferences for premium products.


|product_line|	average_list_price|
|----|----|
|Touring	|1620.209822|
|Standard	|1102.751771|
|Road|	1018.017164|
|Mountain|	628.535981|



### Task 6: List the product_id, list_price, and standard_cost of the products where the list_price is greater than twice the standard_cost.
We are querying for the product_id, list_price, and standard_cost of products where the list price is greater than twice the standard cost. This analysis helps us identify products with a significant profit margin, which is crucial for pricing decisions and profitability assessment.

There are 6800 instances of products where list price is atleast twice the standard_cost.

|product_id	|list_price	|standard_cost|
|----|----|----|
|3	|2091.47	|388.92|
|37	|1793.43	|248.82|
|88	|1198.46	|381.1|
|78	|1765.30	|709.48|
|15	|1292.84	|13.4|


