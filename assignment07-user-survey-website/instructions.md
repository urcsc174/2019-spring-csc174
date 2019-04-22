# Assignment 7: User Survey Website

This is a complex assignment.  You will have two weeks to complete it.

*Due date for the final website: **Wednesday, May 1, 2019*** (the last class)

The goal of this assignment is to create a user survey that informs and gathers input from users, and also provides a back-end interface for administrators to access and edit the survey data.

This is a **team assignment**. Although you are graded as individuals (IA, Designer, Coder - front & back), you are expected to know who is responsible for which of the requirements listed below.  (This time, this instruction sheet does *not* say who does what.)

*By end-of-day today, Wednesday, April 17...*

- [ ] Everyone: use [our shared Google Sheet, "CSC 174 City-Teams"](https://docs.google.com/spreadsheets/d/17nncaY3FWkgq2HEqK6IWAsyNsav34Jo4e-Vj1pwoXEQ/edit#gid=0) to establish your role in a city-team
  - Remember: everyone has to have done each of the three roles at least once; if you want to increase your grade for one of the roles, you can do so.  The two (or more) grades will be averaged together.
  - Note: this is our last team assignment.

## Content

- [ ] For this assignment your city-team will build a **new website around a topic** of your city-team's choice.  
  - The appropriateness of the topic will impact your grade.
    - By "appropriate" I mean a topic that can be pulled-together in a coherent way that will be easy to understand.
    - Note: the topic can literally be about anything.  E.g. shoe strings, ...whatever, so long as the content is architected, designed, and coded properly.
  - You may reuse/repurpose any content from any CSC 174 assignment, or other websites including Wikipedia, but as always you have to cite your sources somewhere in your website.

- [ ] **The PRIMARY goal of the website** is to get website visitors (users) to **fill-out a survey** that is related to the topic.

- [ ] **The SECONDARY goal of the website** is to inform users about the topic so they develop an opinion that they will share in the survey.

- [ ] The **survey, its content, and the post-survey response** must also be architected, designed, and coded properly.

- [ ] NEW: you are required to **get as many people as possible** to go to your website to fill out the survey! 

  - Everyone on the top THREE city-teams who received the highest number of survey responses by end-of-day on Friday, May 10 - without any signs of cheating - will get **an extra one-third letter grade** added to their *FINAL* GRADE!!!  (Maximum grade: A)

  - Note: the grade-increase will be applied *after* you complete the Final Project.

  - Users who fill out the survey are required to identify themselves by entering the following in the survey:

    - Full name

    - A valid email

    - Their location (e.g. city, state)

    ...to ensure - somewhat - that they are real people going to the website and using it as designed, and not filling out the survey multiple times.  (Note: you are not required to automatically authenticate that users aren't filling out the survey multiple times, but if you suspect someone has done so, you need to find and delete those entries.)

  - You are also required to have the database auto-generate a date/time stamp for every record that gets created.

  - The professor will manually review all entries to gauge the data's authenticity.  Signs of cheating (database "stuffing") will result in disqualification for the entire city team.

## Survey Data and Access to the Database

- [ ] Results of the survey must be stored in a **MySQL database**.
  - The database and user credentials for this assignment will be the existing database/user created for your city-team on our shared Bluehost web server
  - Note: be careful to leave the table that's already in there undisturbed


- [ ] The users (people who submit the survey) need to **receive an email** that shows them their survey entries.  (This is like what we did in CSC 170, except instead of the email going to you, it must go to the user using their email address that they entered via the survey form.)
- [ ] The website will also provide a **login for administrators** so the administrators can access a private section of the website that is off-limits to non-logged-in visitors.  The login will be accessible from the public website but in an appropriate, non-conspicuous location.

  - In the login area, there must be *no* link to "Create an Account"
- [ ] The website will also provide **a place to create an account** to become an administrator, however that link must *not* appear anywhere on the website.  Instead, the URL to create an account must be `/register.php`
  - Granted, "hiding" the place to create an account to become an administrator isn't very secure, but it's good enough for CSC 174
- [ ] After the administrator logs-in (we'll call that "**the admin area**"), the administrator will be able to view, update, add, and delete records. (The four database functions)

*NOTE: there are many ways to accomplish the four functions.  You do not necessarily have to use AJAX, JSON or other advanced techniques we never covered in CSC 174.  You can do it "the old fashioned way" using four separate PHP scripts on four separate webpages ...it doesn't matter, so long as it works as part of the overall website.*

- [ ] The admin area must be styled using **Bootstrap** or another off-the-shelf CSS Framework
  - You can use the framework styles exclusively for the admin area but be advised: you still have to place key elements and controls in appropriate areas of each web page based on principles of page design and layout


## Other Notes About the Assignment

All standards that we've covered all semester long will be graded. For example:

- Information Architecture, in terms of:
  - a focused and clear ontology
  - a consistent taxonomy
  - a sensible choreography (which includes good use of Z- or F-patterns ...as you see fit)
  - good use of semantically clean HTML, logical document structure, and good file naming choices (all in support of *search engine optimization*)
- Visual Design, in terms of:
  - Page design, specifically good use of the C.R.A.P. principles
  - Page layout, specifically use of page layout patterns, not necessarily Z- or F- (but those are probably good choices)
  - Use of typography, specifically readability, legibility, and appropriateness of font choices
  - Use of a CSS architecture (any will do - but it must be apparent)
- Technical Coding Standards, in terms of
  - Good, clean, and valid code (within reason) that is optimized, and follows industry standards and best practices without error (that includes lack of error_log files on the server)
  - Everything works as expected

*NOTE: use of a **readme.md** file is <u>not</u> required for this assignment, but it is suggested for team communications only. Use it however you want - for whatever you want - it's up to you.*

### Extra Credit

- [ ] For extra credit, the **Visual Designer** can create **"design language" files** - a set of wireframes and a comp ("comp" is a marketing term, short for "comprehensive layout") 
  - To receive the extra credit, the files must be **submitted in Blackboard** before the website is coded, *and* before Wednesday, April 24 (the halfway point of the assignment)
  - The type of files you submit in Blackboard can be **any type - PSDs, PDFs, JPGs, whatever** - however, if you use some really esoteric application that the professor can't open, he may contact you to regarding exporting your drawings to a more common format.
  - Entries will not be graded until after the website is completed because the wireframes and comp will be **compared to the actual website**; although the actual website does not have to be pixel-perfect compared to the submitted files, it does have to generally represent the intent as shown by the submitted files
  - Also note, if you submit files to be graded, the professor may reply with feedback; if you do not implement the feedback, you will not get the extra points
  - Extra credit will be as much as **10 extra points** on top of the assignment grade for the Visual Designer *(I think Blackboard will allow you to get more than 100% so this could improve your overall grade for Visual Designer, but don't hold me to that)*
- [ ] For extra credit, the **Technical Coder** can implement an **Editable HTML Table** solution for the "Admin Area".  If successful, the user (an administrator) should be able to effect all four database functions without leaving the one webpage
  - Extra credit will be as much as **10 extra points** on top of the assignment grade for the Technical Coder *(I think Blackboard will allow you to get more than 100% so this could improve your overall grade for Technical Coder, but don't hold me to that)*
  - NOTE: whatever the Coder implements, the IA and Designer will also be graded on the placement and styles of all the elements, so be sure to communicate your plan and give the IA and Designer enough time to have you move components around (else they'll lose points for poor architecture or design!)

### Web Server Credentials

Each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: assignment07@csc174.org
FTP Password: [same as before - ask if you need to be reminded]
```

### Submit the Assignment

Note: even though you worked as a team, everyone will be graded as an individual based on the work you did. To get credit for your work:

- <u>Everyone</u> on the team must make a submission in Blackboard, in the assignment:<br> **Assignment 7: User Survey Website**

- In the submission you must provide the following information:

  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own) **and their role** (IA, designer, or coder)
  - A link to the **website**
  - A link to the **repository**

  *NOTE: do not write this information (above) in the comments section in Blackboard.  Use the "Write Submission" area*