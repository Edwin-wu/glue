# Glue Zeppelin Notebooks

### GlueNotebook1-ParquetConversion.json : Demonstrates Parquet Conversion of a CSV Dataset in S3 partitioned by columns

* Uses Spark Dataframes
* Uses boto3 to access Glue catalog
* Parses CSV files by File header
* Repartitions output Parquet data by chosen columns

### GlueNotebook2-MySQL2Redshift.json : Demonstrates a MySQL to Redshift load

* Uses Glue DynamicFrames
* Uses joins to denormalize MySQL tables
* Uses User Defined Functions for computed columns

### GlueNotebook2-MySQL2Redshift.json : Demonstrates a MySQL to Redshift incremental load by timestamp

* Uses external checkpointing to DynamoDB
* Uses Spark SQL for transforms and computed columns
* Uses Spark Redshift package for inserting data to Redshift
* Vaccuums Redshift table as a post load statement
