
# Fetch Rewards Coding Exercise - Analytics Engineer
This document provides a comprehensive overview of essential steps undertaken during the analysis, focusing on transforming unstructured JSON data into actionable insights through a structured relational database model.


# First: Review Existing Unstructured Data and Diagram a New Structured Relational Data Model
For solutions, please refer to the First_Review_Diagram folder. I have uploaded both a Schema Diagram PDF and an image to offer a clear understanding of the data.
1) The User table uses u_id as the Primary Key.
2) The Brands table identifies b_id as unique and establishes a composite Primary Key (barcode, brandCode) to facilitate its joining with the rewardReceipt table.
3) The Receipt table assigns r_id as the primary key and userId as the foreign key for linkage with the User table.
4) The rewardReceipt table, derived from the Receipt table due to its nested values necessary for further analysis, designates reward_id as the Primary Key, r_id as a foreign key to the 
   Receipt table, and (barcode, brandCode) as the composite Foreign Key.


# Second: Write Queries that Directly Answer Predetermined Questions from a Business Stakeholder
SQL queries are available in the Second_SQL_Queries directory, featuring scripts for table creation and solutions to the queries.

# Third: Evaluate Data Quality Issues in the Data Provided
A detailed assessment of Data Quality Issues can be found in the Third_Evaluate_DataQuality folder, which contains a Jupyter Notebook with Python scripts for detailed analysis of each JSON file.

# Fourth: Communicate with Stakeholders
The solutions for this section are located in the Fourth_Communicate folder.
