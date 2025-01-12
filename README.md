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


# Database
Here,we used Mysql DB 
sql dump file:
- /src/main/resources/db_backup.sql
- db_backup.sql file is a mysql dump file.we have to import this dump to mysql db server
- > mysql -u <user_name> -p accounts < db_backup.sql


