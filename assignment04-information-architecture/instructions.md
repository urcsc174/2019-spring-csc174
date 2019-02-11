# Assignment 4: Information Architecture

*Due: Monday, February 18, 2019 (one week)* 

The goal of this assignment is to Fork another team's website and make it better.  

- The **IA** must make the website better by imposing a proper information architecture over the content (note: this is the most important part of this assignment)
- The **Designer** must make the website better by making visual improvements to the formatting and layout of the website
- The **Coder** must maintain or fix the quality of the website in terms of the file structure, optimization, and validation

For this assignment, you will work as a team again, however this time you will be graded as individuals for the work you did in the role you chose.

## Requirements

### DUE: TODAY, Monday, February 11

1. Everyone: go to [our shared Google Sheet](https://docs.google.com/spreadsheets/d/17nncaY3FWkgq2HEqK6IWAsyNsav34Jo4e-Vj1pwoXEQ/edit#gid=0) to choose a new team  
   - Everyone must chose a different role in a different city (COPY your name/email to a new column)
   - Note: you do not have to move as a group; suggestion - move to a ROLE you want to take-on next
   - If necessary setup a new private team channel in Slack
2. The team must choose their new city-team's Assignment 2 or Assignment 3 to "Fork"
   - The **IA** must consider with which assignment it would be easier to build a proper Information Architecture (assignment 2 or 3)
   - The **Designer** must consider with which assignment it would be easier to improve its visual appearance (assignment 2 or 3)
   - The **Coder** must consider which would be easier to setup and install on the website and ensure it runs technically well (assignment 2 or 3)
3. After the team comes to a consensus (assignment 2 or 3) the **Coder** must Fork the repo and setup the new repository, and the add the other team members as collaborators

### DUE: by end-of-day Wednesday, February 12

*Note: this is the trickiest, most important part of this assignment.*

Working alone (typically) the **IA** must make sense of the content as given.  Although it's best to use as much of the original content as possible, the **IA** *may* search across other teams' assignments to mix and match content as necessary to make it easier to make a coherent information architecture.

The goal of the IA is to *impose* an ontology, taxonomy and choreography on to the content.  That may mean getting/changing content including getting new images, altering or writing new headlines ...whatever it takes to FORCE the content into a proper information architecture.  

1. The **IA** must setup the HTML pages and structure the content into a coherent document outline using semantically correct HTML tags
   - Note: it can be rough at first, but good enough for the Designer and Coder to have something to work with when it's sync'd for the first time; remember, the content can be tweaked all the way until the assignment is turned-in next Monday
2. The **IA** must create a **readme.md** file that clearly explains: 
   - The **domain** (a simple line or two of text that describes the subject matter)
   - The **ontology** (a list of *triples* that describes all the content in the website)
   - The **taxonomy** (which will typically translate into headings in the HTML)
   - The **choreography** (which will typically translate into the order and/or navigation)

3. The **IA** must sync the initial content and readme to the team's repository no later than **end-of-day on Wednesday, February 12**
   - The **IA** must also paste a link to the team's repository in [our shared Google Sheet](https://docs.google.com/spreadsheets/d/17nncaY3FWkgq2HEqK6IWAsyNsav34Jo4e-Vj1pwoXEQ/edit#gid=0) 
   - IMPORTANT: if the **IA** has *not* made adequate progress with the HTML by Thursday morning, the professor will re-assign the job of IA to another student and the IA will get a zero for this assignment

### DUE: by Monday, February 18

- [ ] The **Designer** must use *some* of the design elements inherited from the Forked repository, and then make visual improvements
  - The designer will be graded by basic readability and clarity of the typography
  - There must be some logical use of a columnar layout (side-by-side content) on every webpage
- [ ] The **Coder** must ensure the new website meets all web standards and best practices, including but not limited to:
  - PHP Includes factor out redundant code (within reason)
  - The current page highlighter works
  - All HTML and CSS meet W3C standards (within reason)
  - The source code (HTML, CSS, JavaScript and/or PHP) is properly formatted with whitespace and readable
  - The website is mounted on the class webserver and works correctly
    - Only files that are part of the website exist on the web server (e.g. no readme.md on the server!)
    - All file and folder names follow industry standards (all lowercase and no spaces)
    - File sizes (especially image files) are appropriate for the web

## Installation

- [ ] The **Coder** must install the website on the class web server (not Digital Scholar) using the following web server credentials, below.

Note: each team will use the same FTP account. Be careful *not* to disturb other teams' files.

```
FTP Server (a.k.a. Hostname): ftp.csc174.org
FTP Port: 21
FTP Username: assignment04@csc174.org
FTP Password: [ask the prof]
```

- [ ] **Coder**: when you FTP-in to the account, create a folder using the name of your **city-team** and place your website in there
  - [ ] Do NOT put a **readme.md** file or any other file that's not actually used by the website, on the web server!
- [ ] Make sure your website is in your city-team folder - NOT another subfolder inside it!
  - E.g. this is wrong:<br>
    `philadelphia/assignment4/index.php`
    ...it's supposed to be:<br>`philadelphia/index.php`

## Submit the Assignment

*NOTICE: the instructions are different this time!* **EVERYONE** must make a submission in Blackboard

- In the "Assignments Turn-in" area in Blackboard, you'll see a folder titled: **Assignment 4: Information Architecture**
- Within the Assignment 4 folder you will find THREE assignments.  You **pick the one for your role**.  Ignore the others.

As you're making the submission in Blackboard, enter the following in the Write Submission area (*not* the Comments area)
- Click the `Write Submission` button
- In the Text Submission box:
  - Paste a **link to your website**
  - Write your **city-team name**
  - Write a list of **everyone's name** in your team (including your own), and...
  - Next to everyone's name **indicate everyone's role on the team** (IA, designer, or coder)
  - Paste A **link to your team's repository** (which should be set to public)
