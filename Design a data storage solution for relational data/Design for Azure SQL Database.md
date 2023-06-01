Relational data is a type of structured data that has a shared schema. It's often stored in database tables with rows, columns, and keys, and used for application storage like e-commerce websites. As the CTO for Tailwind Traders, you're responsible for designing databases for Azure to support existing structured data on-premises. You're looking for a storage solution to support existing data and future relational data workloads initiated by the company.

## Azure SQL Database

Azure SQL Database is a PaaS deployment option of Azure SQL that abstracts both the OS and the SQL Server instance. An Azure SQL database is a fully managed service. You don't have to deal with complex database tasks like configuring and managing high availability, tuning, and backups. The service automatically upgrades each SQL database to run the most recent version of SQL Server. You get the latest SQL Server capabilities without having to perform manual updates.

### Things to know about Azure SQL Database

Review the following characteristics of the SQL Database deployment option:

- It's a highly scalable, intelligent, relational database service built for the cloud with the industry's highest availability SLA.
    
- SQL Database is the only deployment option that supports scenarios that require very large databases (currently up to 100 TB) or autoscaling for unpredictable workloads (serverless).
    
- You can create a **SQL Database elastic database pool**, where all databases in the pool share the same set of compute and storage resources. Each database can use the resources it needs, within the limits you set, depending on current load.
    
- There are two primary pricing options for SQL Database: DTU and vCore. A serverless option is also available for a single database.
    
    [![Diagram of the two primary Azure SQL Database pricing options, vCore and DTU.](https://learn.microsoft.com/en-us/training/wwl-azure/design-data-storage-solution-for-relational-data/media/select-azure-sql-database-pricing-model.png)](https://learn.microsoft.com/en-us/training/wwl-azure/design-data-storage-solution-for-relational-data/media/select-azure-sql-database-pricing-model-large.png#lightbox)
    
    - **vCore**: A vCore is a virtual core. You choose the number of virtual cores and have greater control over your compute costs. This option supports the Azure Hybrid Benefit for SQL Server and reserved capacity (pay in advance).
        
    - **DTU**: A DTU (Database Transaction Unit) is a combined measure of compute, storage, and I/O resources. The DTU option is a simple, preconfigured purchase option.
        
    - **Serverless**: A compute tier for single databases in SQL Database. The serverless model automatically scales compute, based on workload demand, and bills only for the amount of compute used.
        

#### Business scenario

Let's explore a business scenario for Azure SQL Database. AccuWeather has been analyzing and predicting the weather for more than 55 years. The company chose the Azure platform for its big data, machine learning, and AI capabilities. AccuWeather wants to focus on building new models and applications, not on managing databases. The company chose SQL Database to use with other services, like Azure Data Factory and Azure Machine Learning to quickly and easily deploy new internal applications to make sales and customer predictions.

![Illustration that shows a business scenario for Azure SQL Database.](https://learn.microsoft.com/en-us/training/wwl-azure/design-data-storage-solution-for-relational-data/media/azure-sql-database.png)

### Things to consider when using Azure SQL Database

Consider how Azure SQL Database can be included in your relational data storage plan for Tailwind Traders:

- **Consider vCore pricing**. (Microsoft recommended) Select compute and storage resources independently for multiple SQL databases or an elastic database pool. Use Azure Hybrid Benefit for SQL Server or reserved capacity (pay in advance) to save money. You control the compute and storage resources that you create and pay for.
    
- **Consider DTU pricing**. Choose this simple, preconfigured purchase plan for a bundled measure of compute, storage, and I/O resources to support multiple SQL databases. This option isn't available for Azure SQL Managed Instance.
    
- **Consider serverless option**. Use the serverless compute tier for a single SQL database. You're billed only for the amount of compute used.
    
- **Consider elastic database pools**. Buy a set of compute and storage resources to share among all SQL databases in an elastic pool. For more information, see [SQL elastic pools](https://learn.microsoft.com/en-us/azure/azure-sql/database/elastic-pool-overview).
