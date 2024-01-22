Building a Login System with Python Flask and MySQL.

There are a few steps we need to take before we create our python login and registration system, we need to download and set up Python and the packages we’re going to use.

Requirements
Download and install Python, for this project I will be using Python 3.7.2, make sure to check the box Add Python to PATH on the installation setup screen.
Download and install MySQL Community Server and MySQL Workbench, you can skip this step if you already have a MySQL server set up.
Install Python Flask with the command: pip install flask
Install Flask-MySQLdb with the command: pip install flask-mysqldb

File Structure & Setup
We need to create our project directory and files, you can put the directory anywhere on your computer, as long as Python can access it, create the directories and files below.

File Structure
  
  \-- pythonlogin
  |-- main.py
  \-- static
    |-- style.css
  \-- templates
    |-- index.html
    |-- register.html
    |-- home.html
    |-- profile.html
    |-- layout.html
  
Each file will contain the following:

main.py — This will be our main project file, all our Python code will be in this file (Routes, MySQL connection, validation, etc).
index.html — Login form created with HTML5 and CSS3.
register.html — Registration form created with HTML5 and CSS3.
home.html — The home template to display for logged-in users.
profile.html — The profile template to display for logged-in users.
layout.html — The layout template for the home and profile templates.
style.css — The CSS3 stylesheet for our login and registration system.


Make sure your MySQL server is up and running, it should have automatically started if you installed it via the installer.
Open Command Prompt, make sure you have the project directory selected, you can do this with the command cd c:\your_project_folder_destination on Windows.
Run command: set FLASK_APP=main.py
Run command: set FLASK_DEBUG=1
Run command: flask run
Debug mode will allow us to edit our files without constantly restarting the web server.
