# Assignment 6: Simple Form and Database

*Due: Wednesday, April 3, 2019 (updated)* 

The goal of this assignment is to take an existing website with a simple, HTML form and power it with PHP so it writes to a MySQL database.

*By Wednesday, March 27...*

- [ ] Use [our shared Google Sheet, "CSC 174 City-Teams"](https://docs.google.com/spreadsheets/d/17nncaY3FWkgq2HEqK6IWAsyNsav34Jo4e-Vj1pwoXEQ/edit#gid=0) to establish your role in a city-team
- [ ] Working with your team, decide which Midterm Project you want to use as your starting place
  - See the [projects on our class web server](<http://csc174.org/midterm/>)
  - You can choose any Midterm Project; it doesn't matter if it was one of your own or not
  - Suggestion: read the requirements for this assignment, below and consider what will be required of each team member before selecting a Midterm Project
  - Note: you cannot *fork* the project files because repositories weren't required for the midterm; instead, the Technical Coder just needs to FTP-in to the web server and copy the files locally

## Requirements

Although you are using Midterm Projects for this assignment, you will not be graded on the particulars of the midterm except where specified in the instructions below.  I.e., there will be a different rubric.

### Technical Requirements (Role: Technical Coder), part 1

- [ ] The **technical coder** needs to start the assignment by setting up the repository, adding the team members as collaborators, and syncing the original set of files copied from someone's Midterm Project.
  - REQUIRED: this first step must be done **no later than Wednesday, March 27 by 10:25 AM** 
  - The coder needs to copy a link to the repository into [our shared Google Sheet, "CSC 174 City-Teams"](https://docs.google.com/spreadsheets/d/17nncaY3FWkgq2HEqK6IWAsyNsav34Jo4e-Vj1pwoXEQ/edit#gid=0) 
  - When CSC 174 meets again; the professor will do a live check in class!  Any coder who has not completed this first step will be booted off the city-team and replaced by someone else

*Note: there are more instructions for the Coder, further below*

### Information Architecture Requirements (Role: IA)

- [ ] The **information architect** must restructure the website
  - Set the **primary goal**  of the website to getting users to *sign-up for the newsletter*
  - The **secondary goal** of the website is to get users to read more about the website's topic

- [ ] The **information architect** must create a choreography for the newsletter sign-up
  - Specifically, what happens *after* the user fills out the form and submits it?

- [ ] The **information architect** must add a link to the original Midterm Project in an appropriate place in the Assignment 6 website

*Note: the IA will be graded on the LAYOUT of the website, specifically the positioning of elements within the Z-pattern on the homepage, however the Designer will be graded on their use of CSS to style it.  Let the professor know if you have questions or concerns about that.*

Also note: there is *no* requirement for a **readme.md** file for this assignment.  However, feel free to use one as a communication tool for your team.

Grading:

- The IA will be graded on the semantic naming of files and folders, and semantic usage of *all* HTML tags.
- In addition to the first-level tags that surround content (e.g. P tags, H tags, et cetera), all content must be positioned (nested) in structural elements (e.g. main, section, article, et cetera).
- Note: even though the Designer and Coder may change the tags used in the HTML documents while they work, the IA will be graded for the HTML structure in the final delivery.  So the IA must watch how the team members add or change their HTML documents!  If they make mistakes, the IA will lose points for it. 

### Visual Design Requirements (Role: Designer)

Note: the Designer needs to take direction from the IA, but only as it pertains to layout.  Other than that, the Designer must *make their own choices* for which they will be graded.  

For the most part, the designer can simply continue using the CSS as-is from its source, a Midterm Project.  But beware: the Designer will be graded against the requirements listed below.

*Note: given that the Midterm Projects haven't been graded yet, the designer must choose carefully!  Do you chose a Midterm Project that looks nice but may have technical problems?  Or do you chose one that's simple and has room for improvement?  Good luck choosing!  Let the professor know if you have questions or concerns about that.*

- [ ] The **Designer** must clearly demonstrate understanding of the **C.R.A.P. principles**
  - Design choices such color choices and use of the box model will determine the Designer's grade.
  - Design choices must reflect the content and add value to it.  Design choices must not be made randomly.
- [ ] The **Designer** must implement the **Gutenberg rule** on the home and sub-pages, specifically:  Z- and F-patterns, respectively 
- [ ] The **Designer** must implement a **CSS strategy** that is easily understood and obvious.  (Hint: write a comment-block at the top of your CSS file(s) that describes the architecture and where things can be found.)

And special attention, i.e. a lot of points, will be given to:

- [ ] The style and design of the **HTML form** - how it's positioned and how it integrates with the style of the overall website
- [ ] The style and design of the **post-form presentation** (what does the user see after the user clicks submit?)

### Technical Requirements (Role: Technical Coder), part 2

In parallel with the IA and Designer working on the website, the coder will be graded on the functionality of the simple HTML form and it's ability to write to a MySQL database.

- [ ] On the class webserver (not a localhost), the **Technical Coder** must create a dedicated table to capture input from the website's HTML form
  - Note: the website needs to use a "remote database" - <s>the professor will present instructions regarding how to set up a remote database and use it in the next CSC 174 class.</s> See the instructions in the **Installation** section, below.
- [ ] The **Technical Coder** must add the appropriate PHP code to the website to write HTML form data to the dedicated table in the database on the remote server
  - All industry standards and best practices as demonstrated in CSC 174 for using PHP to write to a MySQL database must be implemented

In addition to powering the website's HTML form to work with a MySQL database, the **Technical Coder** is still responsible for the usual requirements:

- [ ] All HTML and CSS must **validate within reason**; all PHP must work **without error**
  - On the class web server, PHP errors will automatically generate a `error_log` file to help you debug your PHP mistakes.  Be sure to delete any error log files off the server before your midterm is graded.
- [ ] File naming conventions and file sizes must follow **industry standards**
- [ ] Demonstrate your ability to use **PHP Includes** to factor out a reasonable amount of common-code across the webpages

#### Installation

The **Technical Coder** is responsible for the correct installation of the website on the class web server

- [ ] The website must be installed on the BLUEHOST class web server in the folder named: **assignment06** (…which already exists); then create a folder with a name based on the team city that you're in.  
- [ ] The website must use a database and table installed on the BLUEHOST class webserver.  
  - <s>Instructions on how to do that will be forthcoming</s> See below...

### Database Installation on the Production Web Server

The **Technical Coder** is responsible for creating and using the remote database on the class web server

#### Step 1: Login to Bluehost

- [ ] Login to our CSC 174 account on Bluehost
  - Refer to the instructions from *In-class Lab 7: Remote Databases* (<a href="https://docs.csc174.org/lab07-remote-database/instructions.html#step-2-login-to-bluehost" target="_blank">link here</a>)
- [ ] Click the submenu: **database** to get to the **MySQL Databases** page

#### Step 2: Create a new database

- [ ] On the MySQL Database page, under the **Create a New Database** section, enter a database name based on your city-team's name
  - Note: you can create a database name as long as you want, but when you create the user for the database (next step) it can only be seven characters long!  So truncate your database name to seven characters or less.  That way the database and user names can be the same.
- [ ] **Create a new MySQL User** for your database
  - Bluehost will limit you to seven characters
  - Pick an easy password; security is not a concern for what we're doing in CSC 174
- [ ] **Add the new User** to your new database
  - Use the pull-down selectors to select your database and user, then click the green **Add** button
- [ ] On the **MySQL Account Maintenance** page click the ALL PRIVILEDGES checkbox, then click the green **Make Changes** button

After you've done this part of the process, go back to the cpanel in Bluehost and put this browser window (tab) aside for now.  You may need to come back here shortly.

#### Step 3: Transfer the Database from your Localhost

- [ ] In your LOCAL phpMyAdmin, **click on your database** that you created for Assignment 6 in the left-side bar to make sure you’re in that database
- [ ] Click the **Export** tab above the main area, and then on the Exporting tables… page, click the Go button to create the an SQL file and save it somewhere.  You’ll need it soon.
- [ ] Go back to the web browser tab with the **Bluehost cpanel**
- [ ] In the Bluehost cpanel, scroll down to click the **phpMyAdmin** chicklet (or you’ll probably find a link to it along the left-side, under “frequently used features”
- [ ] In Bluehost's phpMyAdmin, in the left-side bar, **click the name of the database** you created in Step 2 (above)
- [ ] Click the **Import** tab in the top area
- [ ] Click the **Choose File** button and select the SQL file you created above
- [ ] Scroll down and click the **Go** button

Hopefully, you’ll see a long list of green messages. If so, proceed to the next step.

#### Step 4: Change the Connection Information

Go back to your localhost files for Assignment 6

- [ ] Open your **connection file** in your code editor ("config.php" ...? or whatever you called it)
- [ ] Update the database login information
  - change the server information from **localhost** to **66.147.242.186**
  - change the user, password, and database information to:<br>database user: **urcscon3** ...followed by the database user name you created in Bluehost<br>user password: ...whatever you used in Bluehost for your database user<br>database name: **urcscon3** ...followed by the database name you created in Bluehost 

- [ ] Save and close the connection file and re-sync it with your GitHub repository
  - Then inform the other developers in your city-team that you've changed the connection information and they need to re-sync with the repo to get it
  - Note: EVERYONE has to test their connection information to see if their current computer's IP is registered with Bluehost so they can use the new database remotely
  - Direct your team members to the following instructions (below); EVERYONE needs to do STEP 5...

#### Step 5: Test the Remote Connection to the Database

Everyone in each city-team needs to test the web application (the HTML form) to see if it still works with the remote database (assuming it worked with your local database before)

Because you're using local files that connect to a database on the Bluehost servers, Bluehost requires that you register your computer's IP number or Class C with them.

Refer to the instructions from *In-class Lab 7: Remote Databases*, specifically steps 3 and 3a and make changes as follows:

- [ ] After you get, unzip, and edit the **testmysql-remote.php** file, change the **database user**, **password**, and **database name** to the new database connection credentials (created by the Coder); then save and close the file
- [ ] With the **testmysql-remote.php** file in your localhost (anywhere) run it in a web browser; depending on the results you get, you may need to do **Step 3a** in the *In-class Lab 7: Remote Databases* instructions

The Coder needs to confirm that all the developers in the city-team are able to use the remote database.  If not, contact the professor for help using the #help channel in Slack.

### Web Server Credentials

The **Coder** on each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: assignment06@csc174.org
FTP Password: [same as before - ask if you need to be reminded]
```

- [ ] When installing the website on the web server, the **Technical Coder** needs to change the connection information for the database in the **config.php** file (or whatever you called it).  The database host needs to be changed *back to* **"localhost"**
  - That sounds unintuitive - changing the hostname back to *localhost* - but the professor will explain in the next CSC 174 class

## Submit the Assignment

Note: even though you worked as a team, everyone will be graded as an individual based on the work you did. To get credit for your work:

- <u>Everyone</u> on the team must make a submission in Blackboard, in the assignment:<br> **Assignment 6: Simple Form and Database**

- In the submission you must provide the following information:

  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own) **and their role** (IA, designer, or coder)
  - A link to the **website**
  - A link to the **repository**

  *NOTE: do not write this information (above) in the comments section in Blackboard.  Use the "Write Submission" area*

