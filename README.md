# hospital-management-system-python-tkinter-mysql
A Python Hospital Management System built with Tkinter for the user interface and MySQL for persistent data storage.  It manages patient information and prescriptions, offering a basic framework for handling essential hospital data.


# Hospital Management System (Python, Tkinter, MySQL)

This Python project implements a basic Hospital Management System with a graphical user interface built using Tkinter and MySQL for data persistence. It manages patient information and prescriptions. This project is intended for educational purposes and demonstrates basic database interaction and GUI development in Python.

## Features

* **Patient Management:**
    * Add new patient records (ID, NHS Number, Name, DOB, Address).
    * View and search patient records.
    * Update existing patient information.
    * Delete patient records.
* **Prescription Management:**
    * Create new prescriptions, linking them to patients.
    * Store prescription details (medicine name, dosage, frequency, issue/expiry dates).
    * View and manage prescriptions.
* **Data Storage:** Uses a MySQL database to store patient and prescription data.
* **GUI:**  User-friendly interface built with Tkinter.
* **Prescription Printing:** Generates a prescription summary that can be printed (basic text output).

## Technologies Used

* Python 3.x (Recommended: 3.7 or higher)
* Tkinter (Built-in with Python)
* MySQL Connector/Python (You'll likely use `mysql-connector-python`)

## Installation

# Clone the Repository:
   ```bash
   git clone [https://github.com/](https://github.com/)[YourUsername]/hospital-management-system-python-tkinter-mysql.git  # Replace with your username
   cd hospital-management-system-python-tkinter-mysql

## 2. Install Required Libraries:
pip install mysql-connector-python

## 3. Set up the MySQL Database:
Create a Database: Use a MySQL client (like MySQL Workbench or the command line) to create a database named hospitaldata (or whatever you prefer – just make sure it matches in your code).
SQL

CREATE DATABASE hospitaldata;
USE hospitaldata;  -- Select the database

## Create the Table: You'll need to create the hospital table. Here's a sample SQL script (adjust data types as needed):
SQL

CREATE TABLE hospital (
    Name_of_tablets VARCHAR(255),
    Reference_no VARCHAR(255) PRIMARY KEY,  -- Assuming Reference_no is unique
    Dose VARCHAR(255),
    Numberoftablets VARCHAR(255),
    Lot VARCHAR(255),
    Issuedate VARCHAR(255),
    Expdate VARCHAR(255),
    Dailydose VARCHAR(255),
    Storage VARCHAR(255),
    nhsnumber VARCHAR(255),
    patientname VARCHAR(255),
    DOB VARCHAR(255),
    patientaddress VARCHAR(255)
);
Configure Database Connection: Open the hospital_management.py file and update the database connection details (host, user, password) to match your MySQL setup.

## 4. Run the Application:

python hospital_management.py

## Usage:
Run the script. The GUI window will appear.
Enter patient and prescription information in the respective fields.
Click the "Prescription" button to generate a prescription summary in the text box on the right.
Use the other buttons (Prescription Data, Update, Delete, Clear, Exit) to manage data.

## Screenshots
![image](https://github.com/user-attachments/assets/de74ade1-a14c-459b-b33b-a076683b6061)


## License

This project is licensed under the MIT License - see the LICENSE file for details.
