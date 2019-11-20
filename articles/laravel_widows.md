
# Laravel
Laravel, is one of the best PHP framework and it is getting more popular among developers all around the world. The Model-View-Controller architecture and blade templating engine made Laravel simple and powerful. Here are the steps of installing it on Windows 10 using XAMPP.


## 1. Install XAMPP
XAMPP is the most popular PHP development environment. XAMPP is a completely free and easy to install it contains Apache distribution with MariaDB, PHP, and Perl.

XAMPP can be easily installed using the link below.

> https://www.apachefriends.org/download.html


## 2. Start Apache and MySQL
So we have successfully installed Apache and MySQL. Now start the Apache and MySQL.

![](/images/articles/laravel/xampp_start.png)


## 3. Install Composer
The composer is an application-level package manager for the PHP programming language that provides a standard format for managing dependencies of PHP software and required libraries. So we need to install composer before installing Laravel. Just follow the below URL and download the Composer-Setup.exe file.

> https://getcomposer.org/download/



## 4. Install Laravel
Now its time to install Laravel on our system using composer. This can be done by running the below command in the Command prompt.

`composer global require "laravel/installer"`



## 6. Create a Database
Now we need to create a database for the project in MySQL server. This can be done using phpMyAdmin.

* Open the link below. http://localhost/phpmyadmin

* Now Enter username and password(As a default, the username will be root password will be empty).
* Click on the New tab
* Enter a database name
* Click on create

![](/images/articles/laravel/create_db.PNG)



## 7. Modify ENV File
We can see a .env file inside the root directory of our project. Add our database details in this file as below.

DB_DATABASE=(in our case app_database)
DB_USERNAME=(Mysql username. Default: root)
DB_PASSWORD=(Mysql password. As a default, blank)

![](/images/articles/laravel/db_config.PNG)

## 8. Migrate Database
Now we have to migrate the database to the local database we created earlier. This can be done using the command below.

> php artisan migrate


## 9. Running the Application
Our application can be run using the command below.

> php artisan serv

This will open up a new tab on our browser with the URL below. This is the home page of our Laravel application.

> http://localhost:8000

Our app can also be run on another port using the command below.

> php artisan serv --port=9000

This will open up our application in the port 9000

> http://localhost:9000
