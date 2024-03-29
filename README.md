# Azure OSS DB SKU Recommender (ODSR)

The OSS DB SKU Recommender (ODSR) project is part of a larger [collaborative effort](https://github.com/izzymsft/OSSDatabaseMigrationHackathon) to provide best practices for migrating PostgreSQL, MySQL and MariaDB workloads to Azure via a challenge-based training event. At its core, the goal of this project is to users to complete OSS DB migration scenarios in less time. 

ODSR enables users to migrate their OSS database installations to Azure with very little to no support when it comes to determining the equivalent SKU in Azure that will be compatible with the current data workload prior to migrating to Azure. 

It optimizes the migration operations while supplementing existing [tools](https://azure.microsoft.com/en-us/services/database-migration/) and [processes](https://datamigration.microsoft.com/) leveraged during OSS database migrations to Azure.

![alt text](ODSR.png "Azure OSS DB SKU Recommender ")

The current version of the ODSR project is designed to connect to an OSS DB instance such as PostgreSQL, MySQL or MariaDB running in an IaaS environment, on-premise or cloud PaaS offering. Once the connection is established ODSR gathers performance and profiling metrics over a minimum period of time (say 30 minutes or 2 hours) and at the end of the data collection phase, an assessment in performed where the aggregated metrics is presented to the user and used to suggest a compatible SKU in Azure for the PostgreSQL, MySQL or MariaDB workload.

