# CSC 174  Final Project

*Due: Monday, May 13, 2019 (last day of exams)*

The point of this take-home exam is to work independently and demonstrate your understanding of the concepts and technologies we've covered all semester in CSC 174.

Although the nature of web development is collaborative, the intent for this exam is to demonstrate *your* abilities to build a website independently.  Still however, you may "get inspiration" and even help from other websites and other students, but be very careful.  

- Copying someone else's code in large quantities without attribution is considered plagiarism. 
- Having someone else write your code is considered cheating.

Instances of plagiarism or cheating will be treated as such and submitted to the University's Board on Academic Honesty.  So be good!

## Requirements

From a very high level, you need to: create a **small website** that demonstrates your understanding of:

- The role of an **Information Architect**
- The role of a **Website Designer**
- The role of a **Front- and Back-end Website Developer** (technical coder)

*Note: the number of pages in the website is up to you; that's one of the things you have to decide as IA*

## Step 1: Domain

The professor will assign a domain (a topic) to you, and give you specific instructions regarding the primary and secondary goals of the website.

- [ ] The professor will confirm your choice of a domain (topic) that is unique to everyone else in CSC 174; you are required to use the domain the professor approved to build your architecture.  

*Note: the intent of the is assignment is to have you gather content from multiple sources and "architect" it - not just scrape content from a single source, like Wikipedia.  You can use Wikipedia, but not exclusively.*

##  Step 2: Gather Content

Note: as you gather content, keep in mind you may have to edit it to meet the requirements below.  It's okay if you take content from Wikipedia and manipulate it within reason.  As always, remember to cite your sources in a logical place in the content.

- [ ] Within the domain assigned by the professor, you choose the **ontology** (the limits of the domain) and compile content: text and images you want to use
    - At least four images (JPGs, PNGs, or GIFs only)
    - Text: at least 900 words

*Think ahead as you gather content.  You will need to "chunk" the content as described below.  Also, the images must relate to the content in some way.*

- [ ] Create a document outline (recommended: do this in a word processor first instead of going direct to HTML); use lots of headings to divide the content into sections.
- [ ] There must be a clear and consistent **taxonomy**, typically seen in the headings, throughout the content
- [ ] There must be a **choreography** (logical order) to the way you arrange the content.  

### Architecture of Behaviors

- [ ] The website must contain a **JavaScript-powered slideshow** (or gallery ...something that presents images to the user, using JavaScript)
  - Remember: where and what the slideshow presents must make sense from an architecture standpoint

- [ ] Add a **contact form** into the architecture
    - Remember: the content (fields) of the the form, as well as the location must makes sense in terms of the ontology, taxonomy, and choreography.
    - Suggestion: just don't dump the contact form in front of the user.  Be sure to use content to entice the user to fill it out - give them a reason.
    - Remember to include in the choreography, what happens after the user clicks the submit button.

## Step 3: Structure the Content

*You may have done the following when you did Step 2*

- [ ] Create your HTML document(s) website using the HTML5 document template.
- [ ] Add your textual content from Step 2 and apply the appropriate HTML5 tags, ensuring all content and document structure is clean and semantically tagged.

*Note: overuse of DIV tags when there are better, more semantically relevant HTML tags to use, will lose points*

## Step 4: Create the Presentation Layer

- [ ] You need to create a design (layout and embellishments) that supports the information architecture, i.e. you cannot make random choices.  You need to demonstrate your **use of styles in support of an information architecture**.

    - [ ] The layout needs to promote **the intended choreography**

    - [ ] The typography, color pallets and general embellishments must **support the intended "mood"** of the website as determined by the subject matter

- [ ] The design must demonstrate your understanding of:

  - **Z- *or* F-Patterns** (layout) ...you need to properly use at least one of the major design patterns somewhere in the website
  - **C.R.A.P. Principles** (styling) ...you need to demonstrate at least three of the four

  Note: use of a **CSS Framework** is *optional* (not graded)

- [ ] Install **two well-paired fonts** and demonstrate your understanding of: Typography, in terms of **readability** and **legibility**

- [ ] Arrange your custom CSS code using any **CSS Architecture** (any standard CSS architecture or one of your own variations)

      - Note: if you use a CSS Framework, you still need to demonstrate your understanding of CSS Architecture

## Step 5: Install the Behavior Layer

- [ ] Choose and install a slideshow (or gallery) solution as architected in Step 2, above
- [ ] Using your localhost, (not the class web server!) create a **MySQL database** to capture the data from the HTML form using **PHP**
  - The data from the form needs to be captured in the database, but that is all.  You do not have to demonstrate the four database functions
- [ ] Ensure that the entire website meets **web standards** and follows **best practices**

## Step 6: Turn it in

Do **not** upload your files to the class webserver or share your files in any way

- Export your MySQL database on your localhost to a file named **export.sql**
- [ ] Compress (ZIP) all your files including the .sql file into a single ZIP file
- [ ] Upload your compressed file to the assignment in Blackboard titled: **Final Project** on or before the due date.

*Note: <u>no</u> readme.md file is required for this project unless you think some of your design choices need to be explained.  If so, create a readme.md file and write a short explanation.*

