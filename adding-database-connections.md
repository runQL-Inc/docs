---
layout: default
title: "Adding Database Connections"
nav_order: 6
---

# Adding Database Connections

Here’s how to connect different database types in runQL:

## BigQuery

To connect to BigQuery, follow these steps:

1. **Create a Service Account**: Ensure you have a Google Cloud service account with the necessary permissions.
2. **Obtain Credentials**: Download the JSON key file for the service account.
3. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **BigQuery** from the list of DBMS options.
   - Enter the connection name, project ID, and other required details.
   - Upload the JSON key file when prompted.
4. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your BigQuery instance.

## Databricks

To connect to Databricks, follow these steps:

1. **Generate a Personal Access Token**: In your Databricks account, generate an Auth Token with the necessary permissions.
2. **Find/Create a cluster to connect**: Find or create a new cluster, and navigate to Advanced Options > JDBC/ODBC to obtain the necessary host and path.
3. **Configure runQL**:
   - Navigate to **Add Connection** in your runQL organization.
   - Select **Databricks** from the list of DBMS options.
   - Enter the connection name, Databricks workspace URL, and other required details.
   - Input the generated access username, token, hostname, and path.
4. **Test Connection**: Click **Test Connection** to verify the connection.

## MSSQL

To connect to MSSQL, follow these steps:

1. **Gather Connection Details**: Obtain the server address, port, username, and password.
2. **Database Name (Optional)**: You may optionally add the database name you would like to be set as the default when writing queries.
3. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **MSSQL** from the list of DBMS options.
   - Enter the connection name, server address, port, and database name.
   - Provide the username and password.
4. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your MSSQL database.

## MongoDB

To connect to MongoDB, follow these steps:

1. **Obtain Connection URI**: Ensure you have the MongoDB connection URI, which includes the username, password, and host details.
2. **Configure runQL**:
   - Navigate to **Add Connection** in your runQL organization.
   - Select **MongoDB** from the list of DBMS options.
   - Enter the connection name and paste the MongoDB URI.
3. **Specify Database (Optional)**: If you want to connect to a specific database within MongoDB, specify it in the configuration.
4. **Test Connection**: Click **Test Connection** to verify the connection.

## MySQL

To connect to MySQL, follow these steps:

1. **Gather Connection Details**: Obtain the server address, port, database name, username, and password.
2. **Database Name (Optional)**: You may optionally add the database name you would like to be set as the default when writing queries.
3. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **MySQL** from the list of DBMS options.
   - Enter the connection name, server address, port, and database name.
   - Provide the username and password.
4. **Enable SSL (Optional)**: If your MySQL server requires SSL, ensure that the SSL option is enabled and configure the necessary certificates.
5. **Enable SSH (Optional)**: If your MySQL server requires SSH, you may submit the SSH Host, Port, Username, and Password instead.
6. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your MySQL database.

## Neo4j

To connect to Neo4j, follow these steps:

1. **Gather Connection Details**: Obtain the host, port, database name, username, and password.
2. **Database Name (Optional)**: You may optionally add the database name you would like to be set as the default when writing queries.
3. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **MySQL** from the list of DBMS options.
   - Enter the connection name, server address, port, and database name.
   - Provide the username and password.
4. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your MySQL database.

## Oracle

To connect to Oracle, follow these steps:

1. **Gather Connection Details**: Obtain the host address, port, service name or SID, username, and password.
2. **Install Oracle Client (If Required)**: Ensure that the Oracle client libraries are installed on the machine where runQL is hosted.
3. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **Oracle** from the list of DBMS options.
   - Enter the connection name, host address, port, and service name/SID.
   - Provide the username and password.
4. **Enable SSL (Optional)**: If your Oracle server requires SSL, configure the SSL settings accordingly.
5. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your Oracle database.

## Postgres

To connect to Postgres, follow these steps:

1. **Gather Connection Details**: Obtain the host address, port, database name, username, and password.
2. **Configure runQL**:
   - Navigate to **Add Connection** in your runQL organization.
   - Select **Postgres** from the list of DBMS options.
   - Enter the connection name, host address, port, and database name.
   - Provide the username and password.
3. **Enable SSL (Optional)**: If your Postgres server requires SSL, ensure that the SSL option is enabled and configure the necessary certificates.
4. **Test Connection**: Click **Test Connection** to verify the connection.

## Redshift

To connect to Amazon Redshift, follow these steps:

1. **Gather Connection Details**: Obtain the Redshift cluster endpoint, port, database name, username, and password.
2. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **Redshift** from the list of DBMS options.
   - Enter the connection name, cluster endpoint, port, and database name.
   - Provide the username and password.
3. **Enable SSL (Optional)**: If your Redshift cluster requires SSL, ensure that the SSL option is enabled and configure the necessary certificates.
4. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your Redshift cluster.

## Snowflake

To connect to Snowflake, follow these steps:

1. **Gather Connection Details**: Obtain your Snowflake account identifier, username, password, role, and warehouse.
2. **Database Name (Optional)**: You may optionally add the database name you would like to be set as the default when writing queries.
3. **Configure runQL**:
   - Navigate to **Add Connection** in your runQL organization.
   - Select **Snowflake** from the list of DBMS options.
   - Enter the connection name and account identifier.
   - Provide the username, password, role, warehouse, database, and schema.
4. **Enable SSL (Optional)**: Snowflake connections are encrypted by default, but ensure that any additional SSL settings are configured if required.
5. **Test Connection**: Click **Test Connection** to verify the connection.

## Trino

To connect to Trino, follow these steps:

1. **Gather Connection Details**: Obtain the Trino coordinator host address, port, catalog, and schema.
2. **Configure runQL**:
   - Go to **Add Connection** in your runQL organization.
   - Select **Trino** from the list of DBMS options.
   - Enter the connection name, coordinator host, port, catalog, and schema.
   - Provide any required authentication details.
3. **Enable SSL (Optional)**: If your Trino coordinator requires SSL, ensure that the SSL option is enabled and configure the necessary certificates.
4. **Test Connection**: Click **Test Connection** to ensure that runQL can successfully connect to your Trino instance.

