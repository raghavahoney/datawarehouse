# datawarehouse
data ware house

Technology Stack Used:

Spring Boot
Hibernate (JPA))
Java 8
MySql


Deployment Instructions:

1. Create the database schema datawarehouse_db and run the sql statements in "db.sql" file
2. Packaging has been done as JAR. Go to project directory through terminal/cmd and run command "mvn spring-boot-run".
3. Launch the view through http://localhost:8099/upload


Brief on development:

1. Composite Primary Key defined on id + fileName for Valid and Invalid tables.
2. logback used for logging.
3. To achieve optimal performance, used JDBC Batch Size param in JPA. Tried with various values for param and observed difference in process duration.
4. Also tried with Stateless session (Persistence session) bean to get rid of cache clearing and observed less process duration. But code has been committed with StateFul session.


