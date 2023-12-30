# Banking-Management

## Overview

This Java-based Banking Management Project provides a command-line interface for basic banking operations. Users can perform operations such as Displaying Customer Records, Adding a Customer, Deleting a Customer, Updating Customer Details, Creating an Account, Displaying Account Details, Taking a Loan, Paying Loan Installments, Displaying Loan Details, Depositing Money, Withdrawing Money, etc.

## Features

- Display Customer Records
- Add a Customer
- Delete a Customer
- Update Customer Details
- Create an Account
- Display Account Details
- Take a Loan
- Pay Loan Installments
- Display Loan Details
- Deposit Money
- Withdraw Money

## Getting Started

### Prerequisites

- Java Development Kit (JDK)
- Eclipse IDE (or any Java IDE of your choice)

### External Libraries

This project utilizes JDBC (Java Database Connectivity) for database interactions. To configure the project in Eclipse:

1. Download the JDBC library (e.g., MySQL Connector/J) from the official website.
2. Open your Eclipse project.
3. Right-click on the project in the Project Explorer.
4. Select **Build Path > Configure Build Path**.
5. In the Libraries tab, click **Add External JARs**.
6. Select the downloaded JDBC library JAR file.
7. Click **Apply and Close**.

### Database Configuration

The project uses JDBC to connect to a Microsoft SQL Server database. Follow the steps below to configure your own database credentials:

1. Open the `DatabaseConnection` class in your Java project.

2. Locate the following code snippet:

   ```java
   // Load the JDBC driver for Microsoft SQL Server
   Class.forName("com.microsoft.sqlserver.jdbc.SQLServerDriver");
   String conurl = "jdbc:sqlserver://server_address;databaseName=your database name";
   con = DriverManager.getConnection(conurl, "your login id", "your password");

3. Replace the placeholder values with your actual database information:

Replace "server_address" with your SQL Server's address.
Replace "your database name" with the name of your database.
Replace "your login id" with your SQL Server login ID.
Replace "your password" with your SQL Server password.
Save the changes.

5. Now, when you run the project, it will connect to your SQL Server database using the specified credentials.

Note: Ensure that your SQL Server allows remote connections, and the JDBC driver JAR is in your project's classpath (as mentioned in the External Libraries section of the README).

## Usage

1. Clone the repository:

	```bash
	git clone https://github.com/kunalgupta72/Banking-Management.git

2. Open the project in your preferred Java IDE.

3. Configure external libraries following the steps above.

4. Run the banking_management.java

5. Follow the command line prompts to interact with the banking system.


## Contributing

Feel free to contribute by opening issues or submitting pull requests. For major changes, please open an issue first to discuss the proposed changes.

