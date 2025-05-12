This project demonstrates how to establish a connection between a Java application and a MySQL database using JDBC (Java Database Connectivity). It is a beginner-friendly project created for understanding the core concepts of database integration with Java. The project focuses on inserting data into a student table, showcasing how to use PreparedStatement to securely and efficiently handle SQL queries.
The application connects to a local MySQL server where a database named krce is assumed to exist. A table called student is used to store records containing student ID, name, age, gender, and address. The Java program opens a connection to the database, prepares an SQL insert statement, sets values using setter methods, and executes the statement to insert two student records into the table.
To make the program more secure and prevent SQL injection attacks, PreparedStatement is used instead of the standard Statement. It also supports setting different values for multiple inserts efficiently. The program includes exception handling for SQLException to catch and print meaningful error messages like constraint violations or connection failures.
For better practice, the database table is designed with id as an AUTO_INCREMENT primary key. This avoids duplicate key errors and allows the database to manage unique identifiers.
This project is ideal for students, beginners, or anyone looking to understand how Java applications interact with relational databases. It provides a practical foundation for more advanced concepts like CRUD operations, database transactions, and integration with web frameworks.
This example can easily be extended to include features like data retrieval, updating records, deletion, and user input through a GUI or web interface.
Overall, the project is a fundamental building block for backend development using Java and databases.

This project is a simple Java console application demonstrating how to connect to a MySQL database using JDBC and perform basic data insertion operations into a student table. It includes:

    Establishing a connection with a MySQL database

    Using PreparedStatement for secure and parameterized SQL queries

    Handling exceptions and avoiding SQL injection

    Demonstrating insertion of multiple records

🛠 Technologies Used:

    Java (JDK 8+)

    MySQL

    JDBC (Java Database Connectivity)

    IntelliJ IDEA / Eclipse (or any Java IDE)

    MySQL Workbench / phpMyAdmin (for managing the DB)

📂 Table Structure:

CREATE TABLE student (
    id INT PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(50),
    age INT,
    gender VARCHAR(10),
    address VARCHAR(100)
);

🚀 How to Run:

    Ensure MySQL server is running.

    Create a database named krce.

    Run the above SQL to create the student table.

    Update database credentials (username, password) in the Java code.

    Compile and run the DatabaseConnectivity class.

✅ Output:

After execution, the console will display:

Saved successfully in database

And the records will be visible in the student table.
