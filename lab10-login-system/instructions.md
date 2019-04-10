# Lab 10: Login System

*Due: Wednesday, April 10, 2019 (today - in-class)* 

The purpose of this lab assignment is to practice building a PHP/MySQL login system for a website.

- Start your MAMP or WAMP server
- [ ] In phpMyAdmin on your localhost, create a database named **sessions_demo**, and a database user by the same name with all privileges assigned.


## Follow online tutorial to build the system

The goal here is to *not* blindly copy and paste the code from the tutorial, but actually read and understand how the pieces and parts work together.  You don't have to know exactly what each line of code does (most of it is error handling) but you do need to know what each snippet does from a high level.

- Go to: the [Tutorial Republic: PHP MySQL Login System tutorial](https://www.tutorialrepublic.com/php-tutorial/php-mysql-login-system.php) and follow the instructions
  - Note: you are expected to know where and how to change the demo code to work with your own development environment (the author assumes you can do that!)
- Test your login system. 

## Add a new webpage to your demo

When your login system works as-is from the tutorial, make these changes to prove you understand the system well enough to hack it a little bit.

- [ ] **Rename welcome.php** to **index.php**.  (You'll also need to find any reference to "welcome.php" in the code and change that as well.)
- [ ] **Create a new webpage** in your login system website - add some content, any content, just so it looks different than the Index page.
- [ ] **Link the new webpage** to the index.php page and vice versa so you can go back and forth between the two pages (in effect, a simple navigation menu)
- [ ] **Make the new webpage inaccessible** unless the user is logged-in
  - If the user goes to the new page directly (by URL) it should automatically re-route the user to the login page
- [ ] **Add a button, "Sign Out of Your Account"** to the the new webpage - same as the button on the index.php page

## Prepare for the Next Assignment

Hold on to your Lab 10 files and database.  The next assignment will involve you merging the login system with your Phonebook Application (Lab 9), and then installing it on the class web server.