# Prerequisites
#
- JDK 11 
- Maven 3 
- MySQL 8

# Technologies 
Hypervisor – Oracle VM VirtualBox
Automation – Vagrant
CLI – Git Bash
IDE – Visual Studio Code
Architecture of Project Services:
NGINX, Tomcat, RabbitMQ, Memcached, MySQL
Architecture of Automated Setup:
Vagrant, Virtualbox, Git Bash

FLOW:
separate flow.doc
NGINX routes the request to the Tomcat server (Java web application service, since the app is written in Java)
NFS server if external storage is needed
Login details are stored in MySQL database
RabbitMQ – can be a message broker or a queuing agent, can be used to stream data
App running in Tomcat – user logs in – app will run an sql query to access the user info stored in sql database – before that it goes to Memcache (database caching service, connected to sql)
MySQL Server will store the user information when the first time the request comes to the database, from MySQL, it will be sent from the MySQL Server to the Tomcat and then it will be cached to the cache
server.


# Database
Here,we used Mysql DB 
sql dump file:
- /src/main/resources/db_backup.sql
- db_backup.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < db_backup.sql


