# Troubleshooting Servers:

# DB:
check mysql service is running or not
systemctl status mysqld
check port no 3306 is opened or not
netstat -lntp
check you are able to connect mysql or not
mysql -h db.daws78s.online -u root -pExpenseApp@1
How to check mysql process is running or not
ps -ef | grep mysql
How to check IP Address is accessible or not
$ping -c3 db.lingaiah.online

# Backend:
check backend service is running
systemctl status backend
check port no 8080 is running or not
netstat -lntp
check you are able to connect mysql or not
telnet db.daws78s.online 3306
How to check backend process is running or not
ps -ef | grep backend
How to check IP Address is accessible or not
$ping -c3 backend.lingaiah.online


Check MySQL data is imported
mysql -h db.daws78s.online -u root -pExpenseApp@1
show databases;
use transactions;
show tables;

How to check expense application is running or not
ps -ef | grep expense

# frontend:
check frontend service is running
systemctl status nginx
check port no 80 is running or not
netstat -lntp --> port no 80
check you are able to connect frontend or not
telnet backend.daws78s.online 80
How to check frontend process is running or not
ps -ef | grep frontend
How to check IP Address is accessible or not
$ping -c3 frontend.lingaiah.online
