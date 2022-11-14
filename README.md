# Cloud-Managed-SQL-ERDs-Dummy-Data
HHA 504 WEEK 7 Assignment 6 --  week 6


## Need to have a .env file in the root directory with following structure for Part5_Db:
```
AZURE_MYSQL_HOSTNAME = "inserthere"
AZURE_MYSQL_USER = "inserthere"
AZURE_MYSQL_PASSWORD = "inserthere"
AZURE_MYSQL_DATABASE = "inserthere"
```


## set up mySQL DB in AZURE/GCP -- used AZURE
1. go to https://azure.microsoft.com/en-us/pricing/details/mysql/flexible-server/
2. create an instance (504-db-server)
3. sudo apt-get update
4. sudo apt install mysql-server mysql-client
5. sudo nano /etc/mysql/mysql.conf.d/mysqld.cnf
6. change 'bind-address' to 0.0.0.0
7. in networking, add firewall rules -- clientIPAddress & allow all 0.0.0.0
8. under server parameters, turn off require_secure_transport

## in vscode, do the following
1. check for the correct python interpreter 
2. pip install python-dotenv
3. pip install faker
4. conda install -c anaconda pymysql

## in terminal
1. mysql -u jannatul -h 504-db-server.mysql.database.azure.com -p
2. show databases;
3. use patient_portal; (name of the database)

