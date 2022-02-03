# Pokemon API v1.0

Spring Boot + Groovy example for Dev.to

## Requirements

* Java 8 or greater
* MySQL
* Gradle
##Updates to run on Java 11
Gradle 7.3.3 will only run on Java 11 later versions do not work 
Update spring boot to version 2.1.9
## Setup MySQL on Docker
* Pull docker image
docker pull mysql
* Create Docker Volume
docker volume create mysql-data
* Run Docker image
docker run -d --name=mysql-server -p 3306:3306 -v mysql-data:/var/lib/mysql -e MYSQL_ROOT_PASSWORD=your_password mysql
* Reference

 https://linuxiac.com/mysql-docker-container/
## Configuration

Edit the file `application.properties` and change **your-username**, **your-password** and **your-database** values.

Running the project will create the database, tables and inserting example data automatically.

## Running the project

In terminal type the command `gradle bootRun`.
