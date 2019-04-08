# Lab 9: Phonebook Application

*Due: Wednesday, April 10, 2019* 

In this exercise you will practice setting up a remote database and connecting to it from your localhost. This is an **individual assignment**.  You will not be working as a team, however you can help each other. 

Note: this lab assignment is counted toward your *participation* grade.

## Setup

- [ ] Re-download [four-functions.zip](../18-four-functions/four-functions.zip) and extract the folder
- [ ] Rename the extracted folder from **four-functions** to **phonebook**
- [ ] Move the **phonebook** folder to your localhost directory
- [ ] In the **phonebook** folder, edit the file: **create-table.sql**
- [ ] Completely delete the contents of **create-table.sql** and replace it with the following code:

```sql
/* replace the dashes on line 2 with your first initial, last name e.g. rkostin_phonebook */
CREATE TABLE `---------_phonebook` (
	`id` int(11) NOT NULL auto_increment,
	`firstname` varchar(32) NOT NULL,
	`lastname` varchar(32) NOT NULL,
	`phone` varchar(32) NOT NULL,
	`email` varchar(32) NOT NULL,
	PRIMARY KEY (`id`)
) ENGINE=MyISAM DEFAULT CHARSET=latin1;
```

- [ ] Edit the code as directed on **line 1**; be careful to not accidently disturb the tick-mark near the dashes on **line 2** when you replace the dashes with your **first initial and last name** (e.g. rkostin)
- [ ] Leave the **create-table.sql** file open; you'll need it shortly

## Create a New Database Connection and Table

- [ ] Edit the file, **connect-db.php**.  Change the database server information (the variables) to the following:


```php
66.147.242.186
urcscon3_lab09
coffee1N
urcscon3_lab09
```

- [ ] Save and close the **connect-db.php** file
- [ ] Login to Bluehost: 
   - www.bluehost.com
   - Username: **csc174.org**
   - Password: [**same Bluehost password as before**, check the #help channel in Slack]
- [ ] Go to the bluehost **cPanel**, and then into **phpMyAdmin**
- [ ] Click on the database, **urcscon3_lab09**
- [ ] Import the code from your edited **create-table.sql** file
  - Use the SQL tab in phpMyAdmin, then copy & paste your edited SQL code there, then run the query (click the GO button)
  - After your table in the database is created successfully, you can close and then delete the **create-table.sql** file, but take note: remember the table name and the exact column names (phone and email) that have been created!
- [ ] Open the phonebook application in a web browser on your localhost; you should see the database application.
  - If you see the empty table (just the table headings), then you're connected okay
  - If you get the "Connect Error (2002)" message, you need to re-register your computer with Bluehost.  (See [Step 3a in In-class Lab 7](https://docs.csc174.org/lab07-remote-database/instructions.html#step-3a-setup-remote-access-to-the-remote-database).)

## Edit the Application to Work with the New Table

Next, you need to hack some of the application files (the .php files) to work with the new database table

- [ ] Open the following PHP files in your code editor
   - **index.php**
   - **new.php**
   - **delete.php**
   - **edit.php**

- [ ] Search for every instance of “**mytable**” in those PHP files and replace them with the new table name (e.g. rkostin_phonebook)
    - In **index.php** there is **one** instance
    - In **new.php** there is **one** instance
    - In **delete.php** there is **one** instance
    - In **edit.php** there are **two** instances

- [ ] Save and close those files


Test the Phonebook application in your localhost again

- [ ] Make some additions, edits, deletions ...whatever, to make sure it's working.

## Edit the Application to Work with the New Table Columns

Notice in the phonebook application that there are only two fields being shown (besides ID): First Name and Last Name ...but the table you created in the database has *two more fields*: **phone** and **email**.  

The bulk of this lab is to hack the code you've been given to work with the new database columns (**phone** and **email**).  

*Note: for some CSC 174 students (especially those with no prior programming experience) this might be tricky, but not impossible! Carefully look at the lines of code indicated in the instructions below and make the changes as needed to get the application to work with the two new database fields.*

- Edit **renderform.php**
  - edit **line 3** to include the two other variables, **\$phone** and **\$email**, and be careful with the commas!
  - duplicate **lines 21** and **22** (create new lines 23 and 24) and edit the duplicates as needed

- Edit **index.php**
  - duplicate **lines 19** and **20** and edit the duplicates as needed
  - duplicate **lines 31** and **32 ** and edit the duplicates as needed

- Edit **new.php**:
  - duplicate and edit **lines 10** and **11**
  - edit **line 16**
  - edit **line 21**
  - edit **line 25** (be very careful with this one; very difficult with all the quotes and commas)
  - edit line **32** (add two more empty quotes with commas)

- Edit **edit.php**
  - duplicate and edit **lines 13** and **14**
  - edit **line 19** (be careful with the double-pipes ...means OR)
  - edit **line 24**
  - edit **line 28** (be very careful with this one; very difficult with all the quotes and commas)
  - duplicate and edit **lines 49** and **50**
  - edit **line 55**

- [ ] Then test all four functions in your web browser - make sure to leave at least one more record in the database that contains data in all four columns (it'll be graded)


NOTE: getting credit for this lab is automatic. When the professor sees your table in the **urcscon3_lab09** database, he’ll give you credit for this assignment in Blackboard.
