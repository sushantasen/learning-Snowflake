# learning-Snowflake
SnowFlake is a fully-managed cloud Data platform as a service, or it is a cloud native SaaS data warehouse platform.

Please sign in and get the trial account first inorder to start/begin.

https://snowflake.com/

Learn snowflake in 20 minutes, please go through the URL and make a hands-on on Snowflake Web UI or install snowSQL( CLI )
https://docs.snowflake.com/en/user-guide/tutorials/snowflake-in-20minutes#summary-clean-up-and-additional-resources

SnowSQL is the command line client for connecting to Snowflake to execute SQL queries and perform all DDL and DML operations, 
including loading data into and unloading data out of database tables.

Install SnowSQL by following this URL: https://docs.snowflake.com/en/user-guide/snowsql-install-config

Once Installed, connect snowsql to snowflake by opening a new command terminal:
snowsql -a <orgname>-<account name> -u < username>
You can find the relevent elements in your snowflake profile details
![image](https://github.com/sushantasen/learning-Snowflake/assets/89632159/e97d88bc-6d26-43c3-bb95-5fa78b0c7fd8)

If the above comamnd does not work, please Try below format:

$ snowsql -a abc.xx.region-1.aws -u  

if you account name is: abc.xx.region-1.aws.snowflakecomputing.com

account_identifier is: abc.xx.region-1.aws

When SnowSQL prompts you, enter the password for your Snowflake user.
![image](https://github.com/sushantasen/learning-Snowflake/assets/89632159/3c50c692-a378-43f1-8685-732a09e24427)

If you log in successfully, SnowSQL displays a command prompt that includes your current warehouse, database, and schema.
There is no warehouse, database, and schema selected for the current session by default. You create these objects in the next step

Please follow this URL :: https://docs.snowflake.com/en/user-guide/tutorials/snowflake-in-20minutes#summary-clean-up-and-additional-resources
Once you study this URL and execute all the steps, which means you know snowflake fundamentals of creating DB, schema, warehouse, load data from Internal stages, External stage, Insert additional data for the table, Manage and Query Data, Analyze data based on your business usecases, Clean up if required.




