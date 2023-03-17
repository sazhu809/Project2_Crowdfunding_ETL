# Crowdfunding_ETL
# Instructions
The instructions for this mini project are divided into the following subsections:

 - Create the Category and Subcategory DataFrames
 - Create the Campaign DataFrame
 - Create the Contacts DataFrame
 - Create the Crowdfunding Database

## Create the Category and Subcategory DataFrames
1. Extract and transform the crowdfunding.xlsx Excel data to create a category DataFrame that has the following columns:

 - A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
 - A "category" column that contains only the category titles

2. Export the category DataFrame as category.csv and save it to your GitHub repository.

3. Extract and transform the crowdfunding.xlsx Excel data to create a subcategory DataFrame that has the following columns:

 - A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
 - A "subcategory" column that contains only the subcategory titles

4. Export the subcategory DataFrame as subcategory.csv and save it to your GitHub repository.

## Create the Campaign DataFrame
1. Extract and transform the crowdfunding.xlsx Excel data to create a campaign DataFrame has the following columns:

 - The "cf_id" column
 - The "contact_id" column
 - The "company_name" column
 - The "blurb" column, renamed to "description"
 - The "goal" column, converted to the float data type
 - The "pledged" column, converted to the float data type
 - The "outcome" column
 - The "backers_count" column
 - The "country" column
 - The "currency" column
 - The "launched_at" column, renamed to "launch_date" and with the UTC times converted to the datetime format
 - The "deadline" column, renamed to "end_date" and with the UTC times converted to the datetime format
 - The "category_id" column, with unique identification numbers matching those in the "category_id" column of the category DataFrame
 - The "subcategory_id" column, with the unique identification numbers matching those in the "subcategory_id" column of the subcategory DataFrame

2. Export the campaign DataFrame as campaign.csv and save it to your GitHub repository.

## Create the Crowdfunding Database
1. Inspect the four CSV files, and then sketch an ERD of the tables by using QuickDBDLinks to an external site..

2. Use the information from the ERD to create a table schema for each CSV file.

**Note:** Remember to specify the data types, primary keys, foreign keys, and other constraints.

3. Save the database schema as a Postgres file named crowdfunding_db_schema.sql, and save it to your GitHub repository.

4. Create a new Postgres database, named crowdfunding_db.

5. Using the database schema, create the tables in the correct order to handle the foreign keys.

6. Verify the table creation by running a SELECT statement for each table.

7. Import each CSV file into its corresponding SQL table.

8. Verify that each table has the correct data by running a SELECT statement for each.

# Results
## Create the Contacts DataFrame
Code for "Create the Contact DataFrame" can be found in the link below
https://github.com/sazhu809/Project2_Crowdfunding_ETL/blob/main/Project_files/ETL_Mini_Project_Starter_MGutieruiz_YZhu.ipynb

Task one: Extract and transform the crowdfunding.xlsx Excel data to create a category DataFrame that has the following columns:

 - A "category_id" column that has entries going sequentially from "cat1" to "catn", where n is the number of unique categories
 - A "category" column that contains only the category titles

![category_df](https://github.com/sazhu809/Project2_Crowdfunding_ETL/blob/main/Project_files/Results/category_df.png)

Figure 1 displays the category DataFrame with the "category_id" and the "category" columns.

Task two: Extract and transform the crowdfunding.xlsx Excel data to create a subcategory DataFrame that has the following columns:

 - A "subcategory_id" column that has entries going sequentially from "subcat1" to "subcatn", where n is the number of unique subcategories
 - A "subcategory" column that contains only the subcategory titles

![category_df](https://github.com/sazhu809/Project2_Crowdfunding_ETL/blob/main/Project_files/Results/subcategory.png)

Figure 2 displays the subcategory DataFrame with the "subcategory_id" and the "subcategory" columns.


## Create the Campaign DataFrame
