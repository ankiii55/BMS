# Bank Management System (ATM Simulator System)

## Introduction

The **Bank Management System aka ATM Simulator System** is a Java-based project that mimics the functionalities of an ATM. Users can open a banking account, deposit and withdraw money, check mini statements, change their PIN, and more. This project is developed using **Core Java, Swing, and MySQL**.

## Features

- Open a new banking account
- Deposit money
- Withdraw money
- View mini statement
- Change PIN
- User authentication

## Technologies Used

- **Programming Language:** Core Java
- **GUI Framework:** Swing
- **Database:** MySQL

## Prerequisites

Ensure you have the following installed on your system:

- Java Development Kit (JDK 8 or later)
- MySQL Server
- MySQL Connector for Java
- JCalendar Library
- Any Java IDE (Eclipse, IntelliJ IDEA, or NetBeans)

## Installation & Setup

### 1. Clone the Repository

```sh
 git clone https://github.com/your-username/ATM-Simulator-System.git
 cd ATM-Simulator-System
```

### 2. Set Up MySQL Database

- Create a database in MySQL and import tables:

```sql
CREATE DATABASE bankSystem;
USE bankSystem;

CREATE TABLE signup(form_no VARCHAR(30), name VARCHAR(30), father_name VARCHAR(30), DOB VARCHAR(30), gender VARCHAR(30), email VARCHAR(60), martial_status VARCHAR(30), address VARCHAR(60), city VARCHAR(30), pincode VARCHAR(30), state VARCHAR(50));
SELECT * FROM signup;

CREATE TABLE signuptwo(form_no VARCHAR(30), religion VARCHAR(30), category VARCHAR(30), income VARCHAR(30), education VARCHAR(30), occupation VARCHAR(60), pan VARCHAR(30), aadhar VARCHAR(60), seniorcitizen VARCHAR(30), existing_account VARCHAR(30));
SELECT * FROM signuptwo;

CREATE TABLE signupthree(form_no VARCHAR(30), account_type VARCHAR(40), card_number VARCHAR(30), pin VARCHAR(30), facility VARCHAR(200));
SELECT * FROM signupthree;

CREATE TABLE login(form_no VARCHAR(30), card_number VARCHAR(50), pin VARCHAR(30));
SELECT * FROM login;

CREATE TABLE bank(pin VARCHAR(10), date VARCHAR(50), type VARCHAR(20), amount VARCHAR(20));
SELECT * FROM bank;
```

### 3. Configure Database Connection

Update database credentials in the Java project (`DatabaseConnection.java`):

```java
String url = "jdbc:mysql://localhost:3306/bankSystem";
String user = "your-mysql-username";
String password = "your-mysql-password";
```

### 4. Add Required Libraries

Ensure the following JAR files are added to your Java project's library:

- `mysql-connector-java-x.x.x.jar` (MySQL Connector for Java)
- `jcalendar-x.x.jar` (JCalendar Library for date selection)

### 5. Compile and Run the Application

- Open the project in your Java IDE.
- Build and run the `Main.java` file.

## Usage

1. Launch the application.
2. Create a new banking account.
3. Log in with your credentials.
4. Perform transactions such as deposit, withdrawal, or PIN change.

## Screenshots

(Add relevant screenshots of the application UI here)

## Contributing

If you would like to contribute, please fork the repository and submit a pull request.

## License

This project is open-source and available under the MIT License.

## Contact

For any queries or issues, reach out to [[your-email@example.com](mailto:your-email@example.com)].

