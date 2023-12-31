# Project 2: Crowdfunding ETL

This repository contains our work for the second project of the UofT SCS edX Data Bootcamp.

Contributors:
- Fanny Sigouin
- Chandler McLaren
- Saiyara Islam
- Donna Camille Velarde

This project is divided into the following subsections:

1. Create the Category and Subcategory DataFrames
2. Create the Campaign DataFrame
3. Create the Contacts DataFrame
4. Create the Crowdfunding Database

The work for this project is under the file `ETL_Mini_Project_FSigouin_CMclaren_DVelarde_SIslam.ipynb`.

## Creating the Category and Subcategory Dataframes

For this subsection, data was extracted from the `crowdfunding.xlsx` file into a dataframe. The category & subcategory column was split into two columns, category and subcategory. From there, lists of unique categories and subcategories were created to turn into two new dataframes: `category` and `subcategory`. Lastly, these dataframes were exported to CSV files: `category.csv` and `subcategory.csv`.

## Creating the Campaign Dataframe

For this subsection, the dataframe created from `crowdfunding.xlsx` was reused and further manipulated to create the campaign dataframe. Unwanted columns were dropped and data types were changed as necessary to produce a clean dataframe, exported to `campaign.csv`.

## Creating the Contacts Dataframe

For this subsection, data was extracted from the `contacts.xlsx` file into a dataframe to be transformed. Each row, stored as a dictionary, was separated into four final columns: `contact_id`, `first_name`, `last_name`, and `email`. It was then exported to `contacts.csv`.

## Creating the Crowdfunding Database

For the last subsection, the crowdfunding database was created using the SQLalchemy and psycopg2 modules. A connection was created between the file and PostgreSQL and the database was then created. The four CSV files created in the above subsections were then imported to the database into their respective tables, with primary and foreign keys. A schema of the database tables was also created using QuickDBD and can be found under `crowdfundingdb_schema.sql`.

## References
Data for this dataset was generated by edX Boot Camps LLC, and is intended for educational purposes only.  
