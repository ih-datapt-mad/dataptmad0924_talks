![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# SQL Setup Workshop

## Quickstart: Create a Single Database - Azure SQL Database

1. Follow the steps in: [Azure SQL Database Quickstart](https://learn.microsoft.com/en-us/azure/azure-sql/database/single-database-create-quickstart)


```
Resource Group name: rg_ironhack

Server name: AdventureWorks

Database name: sql<student>123

Username: azureuser

Password: P@$$w0rd123
```


> __IMPORTANT:__ You'll need to configure a free Azure Subscription here: [Azure Free Account](https://azure.microsoft.com/en-us/pricing/purchase-options/azure-account?icid=azurefreeaccount)

---

2. Once you've configured the Database, you'll need to download and install the database client, **Azure Data Studio**, a versatile and user-friendly tool for working with SQL databases. Follow these steps:

   - Download the application from the official link: [Download Azure Data Studio](https://learn.microsoft.com/en-us/azure-data-studio/download-azure-data-studio)  
   - Install Azure Data Studio by following the instructions for your operating system.  
   - Launch the application and set up a connection to your Azure SQL Database:  
     1. Select "New Connection."
     2. Input your server details:
        - **Server Name**: `AdventureWorks.database.windows.net`
        - **Authentication Type**: SQL Login
        - **Username**: azureuser
        - **Password**: P@$$w0rd123
     3. Click "Connect."

> __IMPORTANT:__ Ensure you configure your firewall rules in Azure to allow your current IP address. To do this:
> - Go to the Azure Portal.
> - Navigate to your SQL Server.
> - Add a new IP address under the **Firewall and Virtual Networks** section.  
> - Use the "Add Client IP" button to automatically detect and allow your current IP.

---

## Other Options Available

A. **DBeaver: An Overview**  

   **DBeaver** is a popular open-source database management tool that supports various database types, including SQLite. It is highly customizable and ideal for managing databases with an intuitive graphical interface.  

   - **Installation**:  
     1. Download DBeaver from [DBeaver Download](https://dbeaver.io/download/) based on your operating system.
     2. Follow the installation guide to set up the application.  
   - **Using DBeaver with SQLite**:  
     1. Launch DBeaver and create a new connection by selecting the "+" icon.
     2. Choose "SQLite" from the list of database types.
     3. Provide the file path for your SQLite database file or create a new file.
     4. Test the connection and save it.  

:exclamation: **NOTE:** Ensure you download the necessary database drivers when prompted during the connection setup. DBeaver will typically alert you to missing drivers and provide an option to download them automatically. Without these drivers, you will not be able to connect to your database.

---

B. **DB Fiddle: An Online Database Tool**  

   **DB Fiddle** ([DB Fiddle Website](https://dbfiddle.uk/)) is an online SQL query sandbox. It allows you to run and test SQL queries directly in a web browser without needing to install a local database.  

   - **How it works**:  
     1. Navigate to the website and select a database engine, such as **T-SQL** for Microsoft SQL Server.
     2. Use the editor to write and execute queries.
     3. View the results in real-time in the interface.  

> __IMPORTANT:__ Always ensure you select **T-SQL** as the language to maintain compatibility with Azure SQL.  

:exclamation: **NOTE:** Document all your queries in a `.sql` file for easy reference and reproducibility. These files can be used to re-execute queries or share your work with teammates.

---

### Happy Querying!