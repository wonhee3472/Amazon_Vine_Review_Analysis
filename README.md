# Amazon_Product_Review_Analysis

## Pipeline of Performing ETL on Amazon Product Reviews

* From the [Amazon Review Datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt), pick a dataset to analyze. **All the datasets have the same data columns as shown below**

![](screenshots/Amazon_Review_Datasets.png)

* Set up a Postgres database using AWS' relational databse service (RDS)

* In pgAdmin, run a new query to create the tables for the new database

* `Extract` one of the datasets and create a new DataFrame
  - For this project, a **furniture** dataset was selected

* `Transform` the extracted dataset into four DataFrames with the correct columns and `Load` them into their respective tables in pgAdmin:
  - Customers Table DataFrame
  ![](screenshots/customers_table.png)
  - Products Table DataFrame
  ![](screenshots/products_table.png)
  - Review ID Table DataFrame
  ![](screenshots/review_id_table.png)
  - Vine Revie Table DataFrame
  ![](screenshots/vine_table.png)


## Pipeline of Determining Bias of Vine Reviews

* The same dataset (`furniture`) from above was selected for analysis
* Total Number of Furniture Reviews
![](screenshots/total_number_views.png)
* Total Number of `5-star` Furniture Reviews
![](screenshots/total_number_5_star_reviews.png)
* Total Number of `Helpful 5-star` Furniture Reviews
![](screenshots/total_number_helpful_5_star_reviews.png)
* Total number of all other Reviews that are `not 5 star rated` & Total Number of all other `non 5-star` helpful Reviews
![](screenshots/all_other_reviews.png)


