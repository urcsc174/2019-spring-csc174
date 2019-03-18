# CSC 174 Midterm Project

*Due: <s>Monday</s> Wednesday, March <s>18</s> 20, 2018*

The point of this take-home exam is to work independently and demonstrate your understanding of the concepts and technologies we've covered in CSC 174 so far.

Although the nature of web development is collaborative, the intent for this exam is to demonstrate *your* abilities to build a website independently.  Still however, you may "get inspiration" and even help from other websites and other students, but be very careful.  

- Copying someone else's code in large quantities without attribution is considered plagiarism. 
- Having someone else write your code is considered cheating.

Instances of plagiarism or cheating will be treated as such and submitted to the University's Board on Academic Honesty.  So be good!

## Requirements

From a very high level, you need to: create a **small website** (at least two pages, can be more) that demonstrates your understanding of:

- The role of an **Information Architect**
- The role of a **Website Designer**
- ...and all the **technical standards and best practices** that you learned in CSC 170.

### Information Architecture Requirements

*NOTE: the "goals" listed below are very important!  They inform you about how you should use the four corners of the Z-Pattern.*

- Pick a topic - any - and build a small, informational website
  - [ ] The **primary goal** of the website is to just *present information* about the topic, i.e., get the user to read more about it
  - [ ] The **secondary goal** of the website is to get users to *sign-up for a newsletter* 
    - Note: you need to *entice* users to sign-up
    - Also note: the newsletter sign-up is NOT the primary goal of the website!

*NOTE: you do not have to implement the newsletter sign-up with a PHP script or database.  (Actually, that'll be a future Lab Assignment.)  You only have to create an HTML form and embed it in your website.  (The "submit" button can be non-functional and you don't have to create a "thank you" page.)*

- [ ] Create your HTML pages using the HTML5 specification and demonstrate your understanding of good structure and semantic use of HTML tags
- [ ] Arrange the content to demonstrate your understanding of:
  - An **ontology** within a chosen domain
  - Implementation of a clear and consistent **taxonomy**
  - Creation of a logical and easy to follow **choreography**
- [ ] Write about (explain) your choices in the readme.md file (especially the choreography)

### Design Requirements

Create a design around your topic that demonstrates your understanding of:
- [ ] Use of the **C.R.A.P. principles** as needed to enforce the meaning of the content ...you need to demonstrate at least three of the four principles
- [ ] Implementation of webpage layouts using both a **Z- and an F-pattern** to help users understand and process information  ...you need to demonstrate both
  - *Note: use of a **CSS Framework** is optional (not graded)*
- [ ] Implementation of a **legible and readable** website design to increase the duration of user interaction and increase comprehension ...you need to install **two well-paired fonts** and demonstrate your understanding of typography

  - [ ] Arrange your custom CSS code using any **CSS Architecture** (a standard architecture or your own variation)
      - Note: if you use a CSS Framework, you still need to demonstrate your understanding of CSS Architecture in your customizations of the framework styles

- [ ] Write about (explain) your choices in the **readme.md** file

  - Explain your application of the Z-Pattern - why you put what you did in each quadrant
  - Explain your application of the F-Pattern - why you laid out what you did, from left-to-right
  - Describe the C.R.A.P. principles that exist in your website and explain what they achieve
  - Explain why you chose the fonts you did (and don't ever say, "because I like them.")
  - Explain the structure behind your CSS Architecture

## Technical Requirements

- [ ] All HTML and CSS must **validate within reason**; all PHP must work without error
  - On the class web server, PHP errors will automatically generate a `error_log` file to help you debug your PHP mistakes.  Be sure to delete any error log files off the server before your midterm is graded.
- [ ] File naming conventions and file sizes must follow **industry standards**
- [ ] Demonstrate your ability to use **PHP Includes** to factor out a reasonable amount of common-code across the webpages
- [ ] In your **readme.md** file - nothing is required from a technical aspect however:
  - You can describe any worthwhile or interesting technical aspects of your website and/or any technical difficulties that didn't work out (you *may* receive credit for things attempted but not achieved)

### readme Requirements

- [ ] You are also required to deliver a **readme.md** file that includes short descriptions of the rationale you used in the content and design of the website.
  - HINT: do not just describe the website!  Rather, describe the reasons and important aspects of your choices
  - Also, if you're particularly happy with some aspect of the website - some technical implementation or interesting arrangement of the content - write about it in the readme.  (Make sure I notice what's good about your website!)

*Note: use of a repository is not required for this assignment.  You'll **submit your readme.md file in Blackboard*** 

*Also note: do not install the readme.md file on the class webserver as it is **not** part of the website. (You would lose points for that!)*

### Other Requirements

Your midterm exam must be installed on the class webserver on or before the due date

- [ ] Upload your files into a directory using your regular, recognizable name (e.g. **rkostin**), using the following credentials

  ```
  FTP Server (a.k.a. Hostname): ftp.csc174.org
  FTP Port: 21
  FTP Username: midterm@csc174.org
  FTP Password: [search the #announcements channel in Slack]
  ```

  *As always, notice the username - that's the difference*

  *And as always, everyone will use the same FTP account so be careful when you're working on the web server!  Be careful not to disturb other students' files.*

- [ ] Create a submission in Blackboard

  - Upload your **readme.md** file to blackboard
  - Copy & paste a link to your website on the class webserver
