# Amazon_Product_Review_Analysis

## Pipeline

* From the [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), pick a dataset to analyze. **All the datasets have the same data columns as shown below**

![](screenshots/Amazon_Review_Datasets.png)

* Set up a Postgres database using AWS' relational databse service (RDS)

* In pgAdmin, run a new query to create the tables for the new database

* `Extract` one of the datasets and create a new DataFrame
  - For this project, a **furniture** dataset was selected

* `Transform` the extracted dataset into four DataFrames with the correct columns:
  - Customers Table DataFrame
  ![](screenshots/customers_table.png)
  - Products Table DataFrame
  ![](screenshots/products_table.png)
  - Review ID Table DataFrame
  ![](screenshots/review_id_table.png)
  - Vine Revie Table DataFrame
  ![](screenshots/vine_table.png)



