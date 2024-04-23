# learning-Snowflake
######################################################################################################
**SnowFlake** is a fully-managed cloud Data platform as a service, or it is a cloud native SaaS data warehouse platform.

Some experts/technie says **Snowflake** is a Data Platform as a Self-managed Service.
**Snowflake** is a true self-managed service, meaning,There is no hardware (virtual or physical) to select, install, configure, or manage.
There is virtually no software to install, configure, or manage.
Ongoing maintenance, management, upgrades, and tuning are handled by Snowflake.

**Snowflake** runs completely on cloud infrastructure. All components of Snowflake’s service (other than optional command line clients, drivers, and connectors), run in public cloud infrastructures.

**Snowflake** uses virtual compute instances for its compute needs and a storage service for persistent storage of data. Snowflake cannot be run on private cloud infrastructures (on-premises or hosted).

Snowflake is not a packaged software offering that can be installed by a user. Snowflake manages all aspects of software installation and updates.
########################################################################################################

**Please sign in and get the trial account first inorder to start/begin.**

https://snowflake.com/

Learn snowflake in 20 minutes, please go through the URL and make a hands-on on Snowflake Web UI or install snowSQL( CLI )
https://docs.snowflake.com/en/user-guide/tutorials/snowflake-in-20minutes#summary-clean-up-and-additional-resources

**SnowSQL** is the command line client for connecting to Snowflake to execute SQL queries and perform all DDL and DML operations, 
including loading data into and unloading data out of database tables.

Install **SnowSQL** by following this URL: https://docs.snowflake.com/en/user-guide/snowsql-install-config

Once Installed, connect snowsql to snowflake by opening a new command terminal:
**snowsql -a <orgname>-<account name> -u < username>**
You can find the relevent elements in your snowflake profile details
![image](https://github.com/sushantasen/learning-Snowflake/assets/89632159/e97d88bc-6d26-43c3-bb95-5fa78b0c7fd8)

If the above comamnd does not work, please Try below format:

**$ snowsql -a abc.xx.region-1.aws -u**  

if you account name is: abc.xx.region-1.aws.snowflakecomputing.com

account_identifier is: abc.xx.region-1.aws

When SnowSQL prompts you, enter the password for your Snowflake user.
![image](https://github.com/sushantasen/learning-Snowflake/assets/89632159/3c50c692-a378-43f1-8685-732a09e24427)

If you log in successfully, SnowSQL displays a command prompt that includes your current warehouse, database, and schema.
There is no warehouse, database, and schema selected for the current session by default. You create these objects in the next step

Please follow this URL :: https://docs.snowflake.com/en/user-guide/tutorials/snowflake-in-20minutes#summary-clean-up-and-additional-resources
Once you study this URL and execute all the steps, which means you know snowflake fundamentals of creating DB, schema, warehouse, load data from Internal stages, External stage, Insert additional data for the table, Manage and Query Data, Analyze data based on your business usecases, Clean up if required.

####################################################################

**Snowflake Architecture**

At the most basic level, Snowflake has 3 important components. 
**1. The Cloud services layer
2. Centralised storage layer 
3. The compute/Query Processing layer.**

**Cloud services** – This is the the “brains” of snowflake. This is where infrastructure management takes place, the optimiser is based (cost-based), metadata management and security (authentication and access control) are handled.

**Storage layer** – When data is loaded into Snowflake, Snowflake reorganizes that data into its internal optimized, compressed, columnar format. Snowflake stores this optimized data in cloud storages.Snowflake manages all aspects of how this data is stored — the organization, file size, structure, compression, metadata, statistics, and other aspects of data storage are handled by Snowflake. The data objects stored by Snowflake are not directly visible nor accessible by customers; they are only accessible through SQL query operations run using Snowflake..

**Compute / Processing** – Query execution is performed in the processing layer. Snowflake processes queries using “virtual warehouses”. Each virtual warehouse is an MPP(Massive Parallel Processing) compute cluster composed of multiple compute nodes allocated by Snowflake from a cloud provider.
Each virtual warehouse is an independent compute cluster that does not share compute resources with other virtual warehouses. As a result, each virtual warehouse has no impact on the performance of other virtual warehouses.

![image](https://github.com/sushantasen/learning-Snowflake/assets/89632159/a2e8a6c7-3892-4ed3-94d3-bb6f4c28d43a)




