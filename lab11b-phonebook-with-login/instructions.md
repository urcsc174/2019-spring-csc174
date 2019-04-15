# Lab 11b: Phonebook Application with Login

*Due: Monday, April 15, 2019 (today)* 

The goal of this assignment is to install your completed *Lab 11a: Phonebook Application with Login*, on the class web server.

**Overview...**

1. Open both phpMyAdmin locally and on Bluehost
2. Export local database to .sql file
3. change \`users\` table to \`flastname_users\` in **login.php** and **register.php**
4. Import .sql file to Bluehost database
5. FTP files to new folder in lab11
6. edit **connect-db.php** file to Bluehost database

## FTP Lab 11 to a new folder on the class web server

- [ ] The website must be installed on the class web server with a folder name in the pattern of first-initial, last name, e.g. **rkostin**, (or you can make it the same as your URID), and put your website files in there
  - Note: the root of the website needs to be the folder you create.  (e.g. **rkostin**)  Do *not* put the website within another sub-folder within the root.  I.e. do not create an "lab11" folder.

### Web Server Credentials

Everyone will use the same FTP account in this class so be careful when you're working on the web server!  Be careful *not* to disturb other students' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: lab11@csc174.org
FTP Password: [search the #help channel in Slack for Lab 11]
```

*Notice that the username is different from last time*

- [ ] Edit the **config.php** file to work with a database (already created) on the class web server

```sql
'localhost'
'urcscon3_lab11'
'coffee1N'
'urcscon3_lab11'
```

*...NOTE: the database server (the host) is still "localhost"*

## Test the Application

Open a web browser pointed to your application on the class web server: 

​	**csc174.org/lab11/*username***
​	(where *username* is the folder you created through FTP)

If everything works, you're good to go.  (No need to submit anything in Blackboard.)  The professor will check your handiwork on the class web server later and give you credit (pass/fail).