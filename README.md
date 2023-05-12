SQL Integration

Why Databases:

Data will not be available in our local system but it will be available in databases for a real time project. In this class we will store data in databases (MySQL Database)

Without databases we will not be able to build any application

CAP Theorem: The CAP theorem states that a distributed database system has to make a tradeoff between Consistency and Availability when a Partition occurs. On the basis of this theorem, we use different databases.

We can easily connect different databases (postgresql, mssql, mysql, oracle, db2 etc.) with Python.

MySQL Workbench:

MySQL Workbench is a visual database design tool that integrates SQL development, administration, database design, creation and maintenance into a single integrated development environment for the MySQL database system.
# Pythyon-mysql-connectivity
import mysql.connector as conn
''' pip install mysql-connector-python'''
''' creating connection with sql  '''
mydb = conn.connect(host = "localhost" , user ="root" , passwd = "Ganpati@2022")
print(mydb)
'''connection established with sql '''
cursor=mydb.cursor()
cursor.execute("show databases") #same as show databses in sql
print(cursor.fetchall())#pulling all the tables in sql


