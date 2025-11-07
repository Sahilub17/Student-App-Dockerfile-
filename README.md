# 🧾 Student Registration Website.



## 🖥️ Frontend -
Node.js and npm must be installed.

## 🧠 Backend -
Java Development Kit (JDK 17 or higher) must be installed.

Maven must be installed.

## 🗄️ Database -
Install MariaDB.

## ⚙️ Before starting, make sure:-

✅ RDS (Relational Database Service) is created.

✅ EC2 Instance is launched.
 
✅ Docker is installed.
 
✅ MySQL Client is installed.

## 🪜 Steps and Commands:


## 1. RDS (Relational Database Service) -

. Create Database

. Standard create 

. MariaDB

. Username - (admin) - Ex.

. Password - (redhat123) - Ex.

. Create Database

## 2. EC2 (Elastic Compute Cloud) -

. Launch instance 

. Connect

```shell
## 1. Switch to root user
sudo -i

## 2. Update the instance
apt update

## 3. Install MySQL client
apt install mysql-client -y

## 4. Mysql
mysql -h (endpoint) -u (username) -p
Enter password (password)

# RDS Database Endpoint copy & paste
# Example: mysql -h database-1.ca9eie2mihs7.us-east-1.rds.amazonaws.com -u admin -p
# Example: redhat123

CREATE DATABASE student_db;
GRANT ALL PRIVILEGES ON springbackend.* TO 'username'@'localhost' IDENTIFIED BY 'password';
show databases;
exit;

# Example: GRANT ALL PRIVILEGES ON springbackend.* TO 'admin'@'localhost' IDENTIFIED BY 'redhat123';


## 5. Install Docker
apt install docker.io -y

## 6. Clone the GitHub Repository
git clone <GitHub_Repository_Link>

# Example: git clone https://github.com/username/student-registration.git

cd <GitHub_Repository_Name>/backend
cp src/main/resources/application.properties .
nano application.properties
    server.port=8080
    spring.datasource.url=jdbc:mariadb://(database endpoint paste):3306/student_db 
    spring.datasource.username=(database username)
    spring.datasource.password=(database password)
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=true
# Then ctrl s+x
```
