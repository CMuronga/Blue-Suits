# Blue-Suits

Project Overview
The Blue Suits Project is a comprehensive Python-based desktop application designed to assist lawyers and administrators with case management, employee tracking, and document handling. The application leverages a graphical user interface (GUI) built using tkinter and includes functionalities for database management, speech recognition, and file operations.

Features
User Authentication

Login functionality with role-based access (Admin, Lawyer).
Employee Management

Add, view, update, and delete employee records.
PDF Management

Upload and view case-related PDF files.
Speech Recognition

Voice commands for enhanced accessibility.
Database Integration

Handles employee and case records using an SQL database.
Modules
The project is divided into five main modules:

main.py

Entry point for the application.
Initializes the Tkinter application and handles page navigation.
home_page.py

Provides the login interface for the application.
admin_page.py

Allows administrators to manage employees and cases.
db_utils.py

Contains functions for database connectivity and CRUD operations.
pdf_utils.py

Handles PDF upload and viewing functionalities.
voice_utils.py

Manages speech recognition using the speech_recognition library.
Installation
Follow these steps to set up and run the project:

Clone the repository:

bash
Copy code
git clone https://github.com/your-repo/blue-suits.git
cd blue-suits
Install dependencies: Ensure you have Python 3.10+ installed. Install the required libraries:

bash
Copy code
pip install tk Pillow pyodbc smtplib speechrecognition
Configure the database:

Set up your SQL Server database.
Create tables for users, employees, and other relevant entities.
Update the connection details in db_utils.py.
Run the application: Execute the main.py file:

bash
Copy code
python main.py
Database Structure
The following tables are used in the application:

Users

username (Primary Key)
password (Hashed)
role (Admin, Lawyer)
Employees

emp_id (Primary Key)
name
email
phone
role
Cases

case_id (Primary Key)
case_name
description
assigned_to
Usage
Login

Use valid credentials to access the system.
Employee Management

Navigate to the Admin Page to view or manage employees.
PDF Operations

Upload and view case-related documents via the Admin Page.
Speech Recognition

Use the voice command feature for quick interactions.
Dependencies
Python 3.10+
Libraries:
tkinter: GUI framework.
Pillow: For handling images.
pyodbc: For database connectivity.
hashlib: For secure password hashing.
speech_recognition: For voice commands.
smtplib & email.mime: For email notifications.
Future Enhancements
Integration with cloud storage for better scalability.
Enhanced speech recognition features with NLP.
Advanced analytics and reporting for case and employee data.


Acknowledgments
Special thanks to the development team and contributors for their hard work in bringing the Blue Suits Project to life.
