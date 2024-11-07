- MySQL Database: Ensure that you have MySQL installed and running.
- MySQL Connector: Make sure to include the MySQL JDBC driver in your project. If you're using Maven, add the following dependency to your pom.xml:

```xml
<dependency>
    <groupId>mysql</groupId>
    <artifactId>mysql-connector-java</artifactId>
    <version>8.0.32</version> <!-- Check for the latest version -->
</dependency>
```

- Create the Database and Table: Before running the program, create a database and a student table in MySQL:

```sql
CREATE DATABASE mydb;
USE mydb;

CREATE TABLE student (
    roll_no VARCHAR(10) PRIMARY KEY,
    name VARCHAR(100),
    marks INT,
    class VARCHAR(10)
);
```

#### Download JDBC mysql driver from here : [JDBC Driver zip file](https://dev.mysql.com/downloads/file/?id=534782)

#### extract the zip file

- Unzip the downloaded file to access the mysql-connector-java-x.x.x.jar file (where x.x.x is the version number).
- Open IntelliJ idea
- Go to File > Project Structure and click on + icon and locate the jar file.
- Click apply and ok
- run the code with proper username password configurations
