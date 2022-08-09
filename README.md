#  Introduction
## 1.1 Brief Description of Project
The project is titled as “Gym Management App” in a quite apt manner since it does exactly that. This App enables its user/Administrator to maintain members, subscriptions and time schedules for gym sessions in a very efficient manner. This App is meant to create convenience and ease of operation for Fitness clubs/gyms. More on this in next section.
## 1.2 Utility of App
The Gym Management App focuses on creating ease and finesse of work for Administrator of a fitness club or gym. Here are the main utilities of the App
1.	Maintenance of active members of the gym.
2.	Preparing Fitness Plans and Packages with proper details and prices.
3.	Creating and maintaining concurrent fitness schedules for different gym members.
4.	Maintaining a trainer list for the gym.
5.	Creating a subscription plan network where payment status of every member is tracked.
6.	There can be multiple Admins on the same database.
7.	We can bundle features into “Packages” and assign trainers to them.


## 1.3 How to Run the App on Windows
Follow the steps below sequentially
1.	Firstly, Download the XAMPP control Panel from the link : Download XAMPP.
2.	After Installing the XAMPP Server on your local Machine, open the “XAMPP Control Panel” from the windows search.(Refer to Screen Shots Below If confused).
3.	Click on the “Start” buttons to fire up the Apache and SQL Servers. They will become Green when running.
4.	Download the App files in Zip format from the drive link given. UnZip these files and move them into the “C:/xampp/htdocs/” directory.
5.	Now, open browser and type in “localhost/phpmyadmin”. PhpMyAdmin portal will open now simply create a new database and name it “gym db” and then, import the gym db SQL file from
“database” folder from the project files.
6.	Finally, Go to browser and type in the search bar
“localhost/P rojectF olderName” and press enter. This Should Launch the App on your Machine and redirect you to a login page.
7.	The Username is “admin” and the Password is “123456”.

#  Tech Stack 
Here we have used the PHP and MySql Combination for our project.

•	Frontend: HTML, JavaScript, CSS, jQuery, Azax, etc.

•	Backend: PHP.

•	Database: mySql

•	Testing: PHP and Javascript.

# ER Model
In our App there is a central SQL database. We will represent that database in form of ER Diagram. There are several entities which are given below with their attributes:
1.	Members- id(PK), member id, name, gender, contact, address, email, date created, registration info id
2.	Schedules- id(PK), members id, date from, date to, time from, time to, members id
3.	Trainers- id(PK), name, contact, email, fees, registration info id
4.	Packages- id(PK), package, description, amount
5.	Plans- id(PK), plan, amount, packages id
6.	Registration info- id(Pk), member id, plan id, package id, start date, end date, trainer id, status, date created, package id.
7.	Payments- id(PK), registration id, amount, remarks, type, date created, registration info id.
8.	Admins- id(PK), name, username, password, type

![image](https://user-images.githubusercontent.com/83055678/183560188-1c50aca0-39f0-4769-bf7b-0d8dfc75c78b.png)

