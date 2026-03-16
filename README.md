# Basic SQL Database Query (Command Line)

This project demonstrates how to **create, manage, and query a SQL database directly from the Windows command line** using XAMPP as the local server environment to run **Apache HTTP Server** and **MariaDB**.

After completing the **Tools of the Trade: Linux and SQL** course from the Google Cybersecurity Professional Certificate, I decided to revisit SQL from a more practical and security-focused perspective. Although I already had basic knowledge of SQL queries, I wanted to strengthen my understanding of how SQL is used in **real-world cybersecurity operations**, particularly within **Security Operations Centers (SOC)**.

SQL is an essential skill for security analysts and engineers because it enables them to:

* Query authentication logs
* Investigate suspicious login activity
* Analyze security events stored in databases
* Perform forensic analysis on compromised systems
* Extract relevant information during incident response

To practice this, I set up a **local database environment** using XAMPP and interacted with the database entirely through the **Windows Command Prompt** instead of using graphical database tools. This helped me better understand how database interactions work at a lower level and improved my confidence working with command-line tools.



## Project Objectives

The goal of this project was to:

* Set up a **local database server**
* Create a **custom SQL database**
* Design tables related to cybersecurity roles and data
* Practice querying and modifying data through SQL commands
* Understand how SQL can be applied to **security investigations**



## Technologies Used

* XAMPP – Local server environment
* MariaDB – SQL database engine
* Apache HTTP Server – Web server included in XAMPP
* Windows Command Prompt – Database interaction interface


## Key SQL Operations Practiced

During this project I practiced several SQL operations including:

### Creating a Database

```sql
CREATE DATABASE CyberSecurity;
```

### Creating Tables

```sql
CREATE TABLE Security_Engr (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    role VARCHAR(50),
    specialization VARCHAR(100)
);
```

### Adding Columns

```sql
ALTER TABLE Security_Engr
ADD age INT,
ADD course VARCHAR(100);
```

### Inserting Data

```sql
INSERT INTO Security_Engr (name, role, specialization)
VALUES ("Gabriel", "Security Engineer", "AppSec");
```

### Querying Data

```sql
SELECT * FROM Security_Engr;
```

### Updating Records

```sql
UPDATE Security_Engr
SET age = 21, course = 'Cybersecurity'
WHERE id = 1;
```

---

## Why This Project Matters for Cybersecurity

In cybersecurity operations, many systems store logs and events inside databases. Security professionals often rely on SQL queries to:

* Investigate suspicious activities
* Track login attempts
* Identify compromised accounts
* Analyze system logs
* Support incident response investigations

Developing strong SQL skills allows security professionals to **quickly extract relevant information from large datasets during security incidents**.


## What I Learned

Through this project I improved my ability to:

* Work with SQL databases from the command line
* Build and modify database tables
* Query and manipulate data efficiently
* Understand how SQL can be used during security investigations
* Practice database interaction without relying on GUI tools

I also discovered that working through the command line gives better insight into **how database systems operate behind the scenes**.


## Future Improvements

Next steps for this project include:

* Creating **tables that simulate real security logs**
* Running **SQL queries to detect suspicious login patterns**
* Building **sample incident investigation queries**
* Automating log analysis using **Python and SQL**


#cybersecurity #sqlquery
