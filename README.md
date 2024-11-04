![Profile Views](https://komarev.com/ghpvc/?username=anay-a-joshi&color=green)  

# CS 5165/6065 (Introduction to Cloud Computing) 
### Project 2: Flask Web Application on AWS EC2  


![AWS EC2](https://img.shields.io/badge/AWS-EC2-yellow)  
![Ubuntu](https://img.shields.io/badge/Ubuntu-24.04-orange)  
![Python](https://img.shields.io/badge/Python-3.x-blue)  
![Flask](https://img.shields.io/badge/Flask-2.x-black)  
![SQLite](https://img.shields.io/badge/SQLite-3-lightgrey)  
![Apache](https://img.shields.io/badge/Apache-2.4-red)  
![HTML](https://img.shields.io/badge/HTML-5-orange)  


A Flask-based Web Application deployed on an AWS EC2 instance, demonstrating user registration, data persistence using SQLite3, and an interactive user interface, as well as extra credit functionality like file upload and its word count display.  


## Overview  
This project is a fully functional web application built using Python and Flask, deployed on AWS EC2, demonstrating practical implementation of cloud infrastructure, web server configuration, database management, and user interaction. Designed to handle user registrations securely and efficiently, the application emphasizes cloud scalability, security, and user-friendly design.   


## Repository Structure  
This repository is organized to separate application logic, templates, database, and static content, providing a clear and scalable codebase for web development.  

* ```flaskapp.py``` - Main Flask application code, handling routing and logic.
* ```flaskapp.wsgi``` - WSGI entry point for running the Flask app with Apache.
* ```index.html``` - Wep Application Testing Code (optional)
* ```users.db``` - SQLite3 database for storing user information.
* ```templates/``` - HTML templates used for rendering different pages.
  - ```login.html``` - User login page.
  - ```layout.html``` - Layout template for consistent styling across pages.
  - ```profile.html``` - Displays user profile information after registration and logging in.
  - ```registration.html``` - User registration page.
  - ```success.html``` - Success page shown after registration or login (optional).
  - ```welcome.html``` - Welcome page shown upon successful login.
* ```uploads/``` - Folder for uploaded files (word count feature).
  - ```Limerick-1.txt``` - Example uploaded file used for word count demonstration.
* ```README.md``` - Project documentation, including setup and usage instructions.


## Key Features  

### 1. Scalable Cloud Deployment  
- **AWS EC2 Instance**: The application is deployed on an AWS EC2 instance running Ubuntu 24.04 LTS, ensuring scalability and reliability.  
- **Apache Web Server**: Configured with Apache using `mod_wsgi` to serve the Flask web application, enabling efficient request handling and reliable uptime.  

### 2. User Management System  
- **User Registration**: Provides a registration form for users to create an account by entering their username, password, first name, last name, and email.  
- **Login and Authentication**: A secure login system authenticates users by verifying their credentials before allowing access to their profile.  
- **Data Storage**: All user information is stored securely in an SQLite3 database, providing data persistence and reliability.  

### 3. Interactive User Interface  
- **Dynamic Profile Display**: After successful login, users are redirected to a profile page that displays their submitted information.  
- **Modern HTML-Based Forms**: User input is collected through clean, easy-to-use HTML forms, ensuring a simple and intuitive registration and login process.  

### 4. File Upload and Analysis  
- **File Upload Feature**: Users can upload a text file (`Limerick-1.txt`) via the web interface.  
- **Word Count Analysis**: The application processes the uploaded file, calculates the word count, and displays the result to the user.  
- **Download Link**: Users are provided with a download link to retrieve the uploaded file.  
- **Persistent File Information**: Upon user re-login, the application displays all user entered data, and previously uploaded files and allows users to download them again, demonstrating effective data persistence and user convenience.  
