# Assignment 3: Smash Website
*Due: Monday, February 11, 2019*

**The goal** of this assignment is to get a little more experience building a website as a team.  This is an activity you need to perfect because all team assignments for the rest of the semester require you to be very comfortable working with tools like this:

- Slack - to communicate with each other remotely
- Localhost - to work independently
- GitHub - to sync your independent work

The content for this website will come from your *In-Class Lab 3: Information Architecture and Markdown* exercise.

Note for the **IA**: you do NOT have to apply the rules of Information Architecture in this assignment.  Just smash the content together so it's coherent.  

Also note: the quality of this website only needs to rise to the standard of CSC 170 quality, i.e. the bar for the content and design is relatively low.  Still, you should try - you might want to include this as an example in your portfolio, right?  In any case, you won't lose points if you simply "smash" the content and styles together for this assignment.  (Hence the name, "Smash Website.")

## Suggested Steps

1. Everyone: refer to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/17nncaY3FWkgq2HEqK6IWAsyNsav34Jo4e-Vj1pwoXEQ/edit#gid=0) to confirm who's who on your team.  
   - Note: you do *not* have to continue doing the same role as before.  In fact, it'd be better if you swap each time you work together so everyone has experience doing everything.
2. Using your *private* team channel in Slack, confirm who's doing what.
   - Note: if you don't have a private team channel setup in Slack, do so.
   - Also note: the prof can't actually tell if you're using Slack or not.  Honestly, you can communicate with each other any way you want.  But you should use Slack to get the experience using it because that's what folks use in the industry these days.
3. The **Coder** should setup the repository and add the other team members as contributors, then the entire team should sync the repository to their localhosts
4. The **IA** should take a guess at the document structure based on how the content will *probably* need to flow, and then setup four HTML skeleton pages, maybe with some dummy content (lorem ipsum) as soon as possible and sync it with the repo.
5. As soon as the webpages are available, the **Designer** should start stitching together the CSS based on the structure.
6. The **IA** and the **Designer** continue to flesh out the content and design while the **Coder** installs the current page menu highlighter.
7. Late in the process, the **Coder** needs to frack the HTML into PHP includes where appropriate.  Be careful, changing files names will trip-up the other team members!  Have them stop and wait until the site is re-configured, then have everyone re-sync so they can continue work.  (Use Slack to coordinate this.)
8. Last step: the **Coder** needs to upload the finished website on the class web server (not Digital Scholar).
9. One of the team members (any) needs to create a submission in Blackboard on behalf of the team.
   - Note: refer to the instructions at the bottom for the requirements on submitting the assignment in Blackboard.  Follow the instructions else lose some points there!

## Requirements

The final product of this exercise must meet the following requirements:

- [ ] Three **readme.md** files from in-class Lab 3 (IA and Markdown) must be combined to create a **three page website plus an index page** (four web pages, total) 
  - [ ] NEW: don't cheap-out with the index page.  Make it functional and make it look like it's part of the website.  Add some content (e.g. snippets) from the subpages to the index page or something like that.
- [ ] There must be **PHP Includes** to factor-out common elements from each webpage to external "include" files


- [ ] The navigation element must **indicate which is the current page** (you'll have to use a PHP or JS solution to insert the a *class* on the appropriate menu item)
- [ ] The HTML, CSS and JS code, files and file system must be clean and follow **industry best practices and standards**

### Installation

- [ ] **The team must install the website** on the class web server (not Digital Scholar) using the following web server credentials, below.

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: assignment03@csc174.org
FTP Password: [ask the prof]
```
- [ ] When you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there
  - [ ] Note: do NOT put a **readme.md** file or any other file that's not actually used by the website, on the web server!
- [ ] NEW: make sure your website is in your city-team folder - NOT another subfolder inside it!
  - E.g. this is wrong:<br>
    `philadelphia/assignment3/index.php`
    ...it's supposed to be:<br>`philadelphia/index.php`

## Submit the Assignment

To get credit for your work:

- ONE of you must submit a link to your website in Blackboard, in the assignment: **Assignment 3: Smash Website**
- [ ] Along with your link write in the **Write Submission** area (*not* the comments box):
  - **Your city-team name**
  - A list of **everyone's name** in your team (including your own), and...
  - Next to everyone's name **indicate everyone's role on the team** (IA, designer, or coder)
  - A **link to your team's repository** (which should be set to public)
