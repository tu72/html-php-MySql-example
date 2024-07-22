 # Button Press Tracker

This project is a simple web application that allows users to press directional buttons and tracks the last button pressed. It uses HTML for the frontend, PHP for backend processing, and MySQL for data storage.

## Prerequisites

- XAMPP (latest version)
- Web browser

## Setup Instructions

1. Install XAMPP:
   - Download XAMPP from the official website: https://www.apachefriends.org/index.html
   - Install XAMPP following the installation wizard instructions for your operating system.

2. Start XAMPP:
   - Launch the XAMPP Control Panel.
   - Start the Apache and MySQL services by clicking the "Start" button next to each.
   - ![image](https://github.com/user-attachments/assets/b91a1b8a-6a9a-42b0-a686-01789f7e11f2)


3. Set up the project:
   - Navigate to the XAMPP installation directory C:\xampp on Windows
   - Find the "htdocs" folder.
   - Place the following files in this folder:
     - index.html
     - fetchLastInput.php
     - saveButtonPress.php

4. Set up the database:
   - Open your web browser and go to http://localhost/phpmyadmin
   - Click on "New" in the left sidebar to create a new database.
   - Name the database "buttonDB" and click "Create".
   - ![image](https://github.com/user-attachments/assets/d7fd4660-7a27-4b1f-aa41-17aa29dbd5b7)

   - Select the "buttonDB" database from the left sidebar.
   - Click on the "Structure" tab at the top.
   - Create a new table with the name "buttonPresses" and 3 columns.
   - ![image](https://github.com/user-attachments/assets/9d8b8cbf-db76-4d47-8eec-b364d5f80a22)
   - make sure to have the same settings for all the columns as me otherwise it might not work.
   - ![image](https://github.com/user-attachments/assets/259d89be-f47a-4a24-9ba8-c03b85b91ec4)


5. Configure the WebSite:
   - Open `fetchLastInput.php` and `saveButtonPress.php` in a text editor.
   - If your XAMPP MySQL setup uses different credentials, update the following lines in both files:
     ```php
     $username = "root"; // change if different
     $password = ""; // change if different
     ```

## Running the WebSite

1. Ensure Apache and MySQL services are running in the XAMPP Control Panel.
2. ![image](https://github.com/user-attachments/assets/bbcd7bd9-fc6c-4007-95ad-da6ed2c1d795.
3.  Open your web browser and navigate to: http://localhost/index.html
4.  you should see something like this ![image](https://github.com/user-attachments/assets/86715929-9d82-40eb-a31d-4ca576590750)
5.  and that's it each time you click on a button it should update and show you what is the last button you clicked 
