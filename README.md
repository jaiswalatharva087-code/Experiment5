arkdown
# 🎓 Student Management System (Java JDBC & MySQL)

A robust, console-based Java application that performs complete **CRUD (Create, Read, Update, Delete)** operations on a MySQL database using **JDBC (Java Database Connectivity)**. 

---

## **🚀 Features**
- **Create**: Add new student records with name, age, and grade[cite: 5, 6].
- **Read**: View and display all registered student records from the database[cite: 3, 4].
- **Update**: Modify existing student information dynamically by ID[cite: 10].
- **Delete**: Remove student records securely using parameterized SQL queries[cite: 1, 2].
- **Error Handling**: Comprehensive exception handling for database connectivity, SQL statements, and invalid user inputs.

---

## **🛠️ Tech Stack & Prerequisites**
- **Programming Language**: Java (JDK 8 or higher)
- **Database**: MySQL Server & MySQL Workbench
- **Library**: MySQL Connector/J (JDBC Driver)
- **IDE**: VS Code, IntelliJ IDEA, or Eclipse[cite: 9]

---

## **📁 Project Structure**
```text
StudentCRUD/
│── src/
│   └── StudentCRUD/
│       ├── DatabaseConnection.java
│       ├── InsertData.java
│       ├── DisplayData.java
│       ├── UpdateData.java
│       ├── DeleteData.java
│       └── Main.java
│── lib/
│   └── mysql-connector-j-9.2.0.jar
└── README.md
⚙️ Step-by-Step Setup Guide
1. Clone the Repository
Bash
git clone [https://github.com/your-username/your-repository-name.git](https://github.com/your-username/your-repository-name.git)
cd your-repository-name
2. Set Up the MySQL Database
Open your MySQL terminal or Workbench and run the following commands[cite: 9]:

SQL
CREATE DATABASE StudentDB;
USE StudentDB;

CREATE TABLE students (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age INT,
    grade VARCHAR(10)
);
3. Configure Database Credentials
Open src/StudentCRUD/DatabaseConnection.java and update your MySQL username and password[cite: 9]:

Java
private static final String URL = "jdbc:mysql://localhost:3306/StudentDB";
private static final String USER = "root";          // Replace with your MySQL username
private static final String PASSWORD = "yourpassword"; // Replace with your MySQL password
4. Compile and Run the Application
For Windows (Command Prompt / PowerShell):
Bash
# Compile the source files
javac -cp "src;lib/mysql-connector-j-9.2.0.jar" src/StudentCRUD/*.java

# Run the main application
java -cp "src;lib/mysql-connector-j-9.2.0.jar" StudentCRUD.Main
For macOS / Linux (Terminal):
Bash
# Compile the source files
javac -cp "src:lib/mysql-connector-j-9.2.0.jar" src/StudentCRUD/*.java

# Run the main application
java -cp "src:lib/mysql-connector-j-9.2.0.jar" StudentCRUD.Main
💻 Application Menu Preview
Plaintext
--- Student CRUD Menu ---
1. Insert Student
2. Update Student
3. Delete Student
4. Display Students
5. Exit
Enter your choice: 
🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check out the issues page.

📜 License
This project is open-source and available under the MIT License.
