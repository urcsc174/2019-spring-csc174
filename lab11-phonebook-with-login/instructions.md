# Lab 11a: Phonebook Application with Login

*Due: Monday, April 15, 2019* 

The goal of this assignment is to, in effect, merge your phonebook application (Lab 9) with the login system (Lab 10).

GOAL: let users see the phonebook table (index.php), but password-protect the ability to add a new record (add.php), edit a record (edit.php), or delete a record (delete.php).

## Export Your Lab 9 Data

- [ ] Login to **Bluehost** and navigate to the *cpanel* and then into *phpMyAdmin*

- [ ] Click on the database: **urcscon3_lab09**
- [ ] Click on your phonebook table
- [ ] Click the **Export** button (top tab bar)
- [ ] Click the **Go** button and save the .sql file somewhere handy (like your computer's desktop)
  - Take a look inside the .sql file; notice the SQL code contains all the instructions for the phonebook table _plus_ the actual data from that table

## Create a New Database

- [ ] Open your LOCAL *phpMyAdmin*
- [ ] Create a new User/Database/Permissions set; call the user and database **phonebook2**
  - remember: you can create all three at once by going into the User Accounts area of *phpMyAdmin*

- [ ] Click on your new database in the left-side panel
- [ ] Click the **Import** tab (top tab bar) and select the .sql file from the previous step, and click the **Go** button

- Check to make sure your database table and the data got setup correctly

## Create a New Set of Website Files

- [ ] Working in your *webroot* folder on your computer, copy your **phonebook** folder to a new folder called **phonebook2**

- [ ] In **phonebook2**, edit the **connect-db.php** file; edit the connection information to work with your local database
  - change the *server*, *user*, *pass*, and *db* appropriately

- Test the phonebook2 application in your web browser.  Make sure it continues to work using your local database

## Apply Styles

Apply basic design principles to the phonebook application (simply: make it look nice)

*NOTE: the following instructions are a bit of a cop-out, but since the focus of this lab assignment is on the application, not the design, it is appropriate to use a CSS Framework like Bootstrap.  Also, since the login system tutorial we did in the in-class lab uses Bootstrap, this will work nicely with that.*

Also note that this phonebook application only uses two files to display content in the user's viewport: *index.php* and *renderform.php* 

- Open **index.php** and **renderform.php** for editing

- [ ] In both files, install Bootstrap using the Bootstrap CDN in the normal place where you link CSS files:

```html
<link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.css">
```

- [ ] In both files, install a "container" in the BODY tags
  - See here for Bootstrap instructions on using a container: [https://getbootstrap.com/docs/4.3/layout/overview/](https://getbootstrap.com/docs/4.3/layout/overview/)
  - Suggestion: inside the BODY tags create the opening DIV with the container class directly above where the content starts (*below* the PHP block), and close the DIV directly above the closing BODY tags.

- [ ] In both files, embellish the bare-bone content with some more HTML and text.  See the examples below as minimums.

- [ ] In the **index.php** file, style the table by adding Bootstrap classes in the appropriate places

  - See here: [https://getbootstrap.com/docs/4.3/content/tables/](https://getbootstrap.com/docs/4.3/content/tables/) (feel free to do more styling than what's shown here)
    ![figure1](media\figure1.png)

- [ ] In the **renderform.php** file, you need to style the form

  Before adding Bootstrap classes to the form, you need to fix some of the HTML problems (non-standard HTML); notice there are no LABEL tags, and the use of BR tags is unprofessional ...you need to fix that first

  - You can leave the first INPUT (type="hidden") as-is, because it's hidden
  - [ ] Add an ID to each INPUT tag and give them a value that makes sense for each one
  - You can leave the STRONG tags around the ID as-is, but for the rest...
  - [ ] Change all those STRONG tags to LABEL tags and add a *for=""* attribute with the correct value for each
  - [ ] Delete those BR tags and instead, wrap each LABEL/INPUT pair in a DIV

  Then, with the HTML in the FORM standardized you can start to style it by applying Bootstrap classes.

  - [ ] Refer to the Bootstrap documentation for classes you can use to style the HTML FORM: [https://getbootstrap.com/docs/4.3/components/forms/](https://getbootstrap.com/docs/4.3/components/forms/) (again, feel free to do more styling than what's shown here)
  - [ ] Also, add more HTML content to make the webpage look a bit more normal/usable; here's an example with the bare minimum
    ![figure2](media\figure2.png)


Check to make sure the phonebook2 application continues to work correctly, reading and writing data to your local database, before moving on.

## Password Protect Part of the Application

Again, the goal of this assignment is to, in effect, merge your phonebook application (Lab 9) with the login system (Lab 10).  Specifically, you need to let users see the phonebook table (index.php), but password-protect the ability to add a new record (add.php), edit a record (edit.php), or delete a record (delete.php).  That means inserting two new pages into the websites Information Architecture: login and register (as well as their helper files and a new table in your database).

### Merge Some of the Files from Lab 10

- [ ] Create the **users** table (from Lab 10) in your local **phonebook2** database...
  - You can use the **users.sql** script from Lab 10; just go into phpMyAdmin and click on the **phonebook2** database, then IMPORT (or use the SQL tab to copy and paste the script) to setup the **users** table
  - The goal is to have two tables in your **phonebook2** database: one for the phonebook records, and another for the user accounts.
- [ ] Copy the **login.php** file, **register.php** file, and **styles.css** file from Lab 10 to your **phonebook2** folder

**Note: part of merging applications is dealing with inconsistencies between them.** 

- [ ] Edit the **login.php** and **register.php** files - notice that their first statement (line 3) refers to **config.php**.  Since the phonebook application uses a file named **connect-db.php** (instead of config.php) edit that line accordingly so the **connect-db.php** file is used

- Open Lab 10's **config.php** file and phonebook2's **connect-db.php** file.  Notice that, even though they do effectively the same thing, they're coded differently.  
- Generally that doesn't matter, but it just so happens that the Lab 10 connection file saves the database connection (in **config.php**) in a variable named **$link** (on line 9) and the phonebook2 connection file saves the database connection (in **connect-db.php**) in a variable named **$connection**.  
- That little inconsistency between applications is normal, and unfortunately must be fixed wherever those variables are used, or else the phonebook application won't work. So...

- [ ] Continue editing the **login.php** and **register.php** files in the phonebook2 application.  Find every instance of the variable **$link** and replace it with **$connection**
  - In **login.php** there are two instances
  - In **register.php** there are three instances

### Password Protect the Webpages that Should be Protected

- [ ] From the Lab 10 **index.php** file, copy-out the PHP block that sets and then checks the session variable (lines 1 - 10), and paste that PHP block at the top of phonebook2's **new.php**, **edit.php**, and **delete.php** files
  - That'll keep those three files from ever showing unless the user is logged-in
- [ ] Edit the **logout.php** file - change the redirection (the header() command on line 12); instead of redirecting the user to **login.php**, change that to **index.php**

### Add "States" to the Webpages for Logged-in vs. Logged-out

*Note: this is new in CSC 174.  I did not cover this technique in our last two classes on session variables.  But you've seen parts of this PHP code before.  This is the code that decides whether or not to do something based on whether or not the user is logged-in.*

- [ ] Add a session start command to the top of both the the **index.php** file and the **renderform.php** file like this:<br> `<?php session_start(); ?>`
  - This will allow us to show or hide content in the phonebook2 application based on whether the user is signed-in or not
- [ ] In the **index.php** file, add a *login* AND a *logout* link to the top-right of the webpage, just under the opening DIV with the *container* class, like this:

```php+HTML
<div style="float: right; margin-top: 30px;">
<?php if(isset($_SESSION['username'])) { ?>
  <a href="logout.php">Logout of your User Account</a>
<?php } else { ?>
  <a href="login.php">Login to your User Account</a>
<?php } ?>
</div>
```

  - This snipped of code will show *either* the link to *login* or the link to *logout* based on the "state" of the session variable (actually, the existence of the session's global variable "username" being set or not)

*NOTE: that snippet of code is shameful (using in-line styles, and a bastardized float used to position it).  Normally, you would be expected to write appropriate CSS in your external stylesheet, but this assignment is long enough.  Sad.*

Using the same IF statement to check whether the session is active or not, you can disable other features of the **index.php** webpage where it makes sense.

- [ ] In the **index.php** file, wrap the link to "Add a new record" with this PHP code:

```php+HTML
<?php if(isset($_SESSION['username'])) { ?>
  <a href="new.php">Add a new record</a>
<?php } ?>
```
That will keep that link from showing unless the user is logged-in.

- [ ] In the **index.php** file, wrap the table header that creates the "functions" header for the table using this PHP code:

```php+HTML
<?php if(isset($_SESSION['username'])) { ?>
    <th colspan="2"><em>functions</em></th>
<?php } ?>
```

- [ ] And finally, in the **index.php** file, wrap this part of the table using this PHP code:

```php+HTML
<?php if(isset($_SESSION['username'])) { ?>
    <td><a href="edit.php?id=<?php echo $row['id']; ?>">Edit</a></td>
    <td><a onclick="return confirm('Are you sure you want to delete ID: <?php echo $row["id"]; ?>?')" href="delete.php?id=<?php echo $row['id']; ?>">Delete</a></td>
<?php } ?>
```
Those two snippets of code above will keep the "functions" column from appearing in the table unless the user is logged-in.

With the code to control the HTML based on the "state" properly installed, the index page will appear in one of two ways:

1. This, when the user is *not* logged-in:

![figure3](media\figure3.png)

2. This, when the user *is* logged-in

![figure4](media\figure4.png)



This is the end of Lab 11a.  

Hold on to your files and database tables for now.  Later, Lab 11b will require you to move the application from your localhost to the class web server.  