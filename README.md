# Blog It!

Deployment link: (https://blog-it-app-f2464249567c.herokuapp.com/)

Github Repository: (https://github.com/henrybennett94/Blog-It)

Welcome to Blog It! Whether you're a seasoned collector or simply curious about the charm of vintage finds, join us as we explore the world of antiques, share tips for restoration and care, and connect with fellow enthusiasts who appreciate the artistry and nostalgia of yesteryear. Let’s uncover the past together!

## Table of Contents

- [Introduction](#introduction)
- [UX Design](#ux-design)
- [Development](#development)
- [Technology Used](#technology-used)
- [Deployment](#deployment)
- [Credits](#credits) 

## Introduction

Blog It! is a Django web application, intended to give users a streamlined platform for making, updating and managing posts that celebrate the beauty and history of treasured relics from the past! The intended audience is for people with an interest in historical antiques and artifacts, from any period, so that they have a dedicated online space to celebrate this passion by reading and/or posting about. In this way, the application is intended to have full CRUD functionality and user authentication, meaning users of the service can create their own account on the application, on which they have the agency to create, update, and delete posts and comments as logged-in users.

------

## UX Design

This application was designed using Balsamiq to create wireframes. The method of the design was to conform to user stories.

### MVP

The MVP provides users with an interest in the subject, though anyone is welcome to join, with an application they can quickly sign up with, and then use to create and read about interesting facts and stories related to different historical antiques, with the option to comment on other account-holders' posts, and delete and edit these posts.


### User Stories for Blog It!:

- As a site user I can view a paginated list of posts so that I can select which post I want to view.
- As a site user I can access my user account through a login form requiring a password so that my account's security is maintained.
- As a site user I can create a user account with a username and password so that access to how I use the site is private to me and protected.
- As a site user I can get asked to confirm that I wish to delete a feature, after selecting a delete option so that the risk of accidentally deleting something is minimised.
- As a site user I can leave comments on a post so that I can be involved in the conversation
- As a site admin I can approve or disapprove comments so that I can filter out objectionable comments
- As a site user or admin I can view comments on an individual post so that I can read the conversation
- As a site user or admin I can view comments on an individual post so that I can read the conversation
- As a site user I can have the option to delete my posts and comments that I no longer need there so that I can keep my user space organised, updated and relevant.
- As a site user I can click on a post so that I can read the full text
- As a site admin I can create draft posts so that I can finish writing the content later
- As a site admin I can create, read, update and delete posts so that I can manage my blog content
- As a site user I can like others' posts so that I can show appreciation for other site users' content.


------

## Development

The project was developed using Agile Methodology. User stories were mapped to a Github Projects project board to chart development progress, with three sections: 'To Do'- the backlog, 'In Progress', and 'Done'. 

### Link to Project Board

https://github.com/users/henrybennett94/projects/7

------

## Technology used
Blog It! leverages several modern web development technologies, with the intention to create an engaging and interactive user experience. The key technologies used are Python, HTML CSS, JavaScript, Django, and Cloudinary.

### Python
Python is an object-oriented general purpose programming language used popularly in supporting web development. Using Python in a Django project enables the creation of powerful web applications by leveraging Django's high-level framework for clean, scalable, and maintainable code.
### HTML
HTML (HyperText Markup Language) is the standard markup language used to create the structure of the web pages in this application. It provides the skeleton for the app's interface, defining elements such as buttons, images, and text content.
### CSS
CSS (Cascading Style Sheets) is used for styling the HTML elements. It enhances the visual presentation of the app by controlling the layout, colors, fonts, and overall look and feel.
### JavaScript
JavaScript enhances a Django application by enabling dynamic, interactive user interfaces, streamlining the development process.
### Django
Django is a Python web framework ideal for projects due to its robust scalability, offering rapid development, built-in security features, and a clean, pragmatic design. Its capabilities facilitate a well-structured development environment and enable a straightforward interface between application and database. 
### Cloudinary
Cloudinary is a cloud-based service that provides powerful tools for managing, optimizing, and delivering images and videos in web and mobile applications. Offering seamless media management and optimized delivery, it is an expedient tool for storing media in a Django application.

---
## Deployment

- The site was deployed to Heroku. The steps to deploy are as follows: 
  - Log in to herokuapp.com
  - From the Heroku dashboard, navigate to "New", and from the dropdown select "Create new app"
  - Choose a unique app name and select region, create app ("blog-it-app")
  - In the Heroku my-shopping-app go to the Settings tab, reveal Config Vars and set the necessary keys and        values
  - Go to the Deploy tab, go to "Deployment Method" section and select Github
  - Search for and then select the relevant Github repository (https://github.com/henrybennett94/Blog-It), to connect it with the Heroku app
  - Navigate to the "Manual deploy" section, ensure the main branch is selected for deployment, and then select "Deploy"
  - Wait for the app to build in Heroku
  - Select "View" on completion of build
  - The deployed link can be found at: (https://blog-it-app-f2464249567c.herokuapp.com/)

---
## Features
### Features implemented:
- Overview of posts
  user is redirected to a display of all posts with previews of content, paginated by six posts per page.
- Viewing posts in detail
  Site user selects a post title to open a display of the post with any comments.
- Create an account to comment on posts
- Authenticated users can comment on posts, and have full CRUD management of their own comments
  Only logged in users can Submit, Edit, and Delete comments on posts. In case of non-authenticated site visitor 
  browsing a post, 'Log in to leave a comment' message displays above the page footer, in place of 'Leave a 
  Comment' form.
  Any site user who has posted a comment has the option to edit that comment, by selecting 'Edit' under the 
  comment in the comment section.
  Any site user who has posted a comment has the option to delete that comment, by selecting 'Delete' under the 
  comment in the comment section.
- Comment approval required from site admin to publish comment
  Site admin can approve comments submitted from logged-in users, so the comment becomes visible to all site     
  visitors.
- Datetime for posts, comments and all updates
  Datetime is displayed for each post and comment on site: datetime of either the original posting or, if 
  updated, datetime of the update.
- Creating and saving of drafts (for superusers)
  From the admin panel, admin can add a new post but not publish it, with the option to amend the content again 
  before publishing by saving as a draft.
- 'About' page
- Defensive building
  When selecting delete (of a comment, or post if admin), options are presented to confirm deletion action, or to 
  cancel action.

### Features to implement for future iterations:
- 'Like' button
### Possible revisions
- Comment approval required
  Implement logic to remove requirement for admin approval for all users posting comments.

#### Create drafts
- Expected: From the admin panel, admin can add a new post but not publish it, with the option to amend the content again before publishing by saving as a draft.
- Testing: From the admin  panel, navigate to /blog/posts section, and select '+Add'. Fill in form fields to create a post. Check value for 'Status:' field is set to 'Draft'. Select SAVE.
- Result: Redirected to /admin/blog/post, where 'Test draft post' is listed first, with status of 'Draft'.
- Result: On returning to Home page, 'Test draft post' is not listed among the published posts accessible from Home. But 'Draft' status means it can be accessed from Admin panel to be amended at a later date.

#### Manage posts
- Expected: Site admin can, in the admin panel, create, update, read and delete posts, with changes reflected in the public website.
- Testing: Create: From the admin  panel, navigate to /blog/posts section, and select '+Add'. Fill in form fields to create a post. Check value for 'Status:' field is set to 'Published'. Select SAVE.
- Result: Create: New post is displayed on Home page.
- Testing: Read: From Home, click new post to open it. 
- Result: Read: Redirected to /newpost/, with all published content of the post displayed to user.
- Testing: Update: From admin panel, navigate to /admin/blog/post/. Select a published post to open it. In all fields, change values to modify the data, then click 'SAVE'.
- Result: Update: On opening the modified post from the Home page next, the associated data has changed.
- Testing: Delete: From admin panel, navigate to /admin/blog/post/. Select a published post to open it. With the post open for editing as per previous step, scroll down to 'Delete' button and select.
- Result: Delete: Redirected to /delete/ to confirm deletion action with 'Yes, I'm sure', or cancel action with 'No, take me back'.

---
## Testing

### Manual Testing

#### Navigation Links
- Expected: Link to separate pages of website anchored in the navigation menu, so user is redirected to each page on selecting the title.
- Testing: Move cursor over the titles ('Home', 'About', 'Register', 'Login'), which transition from grey to bold when hovered on (excepting current page which is always bold). Selecting title redirects page.
- Result: User redirected to urls:
  - https://blog-it-app-f2464249567c.herokuapp.com/ 'Home'
  - https://blog-it-app-f2464249567c.herokuapp.com/about/ 'About'
  - https://blog-it-app-f2464249567c.herokuapp.com/accounts/signup/ 'Register'
  - https://blog-it-app-f2464249567c.herokuapp.com/accounts/login/ 'Login'
  on completing above action.

#### Hover Functionality (text highlighting)
- Expected: Hovering cursor over post titles and preview text highlights all content to indicate an anchored link to the full content for user.
- Testing: Hover cursor over posts.
- Result: Text highlights to indicate link.
#### Links to posts
- Expected: Selecting posts titles and previews from list on homepage redirects to full content of post.
- Testing: Hover cursor over post title and select.
- Result: User redirected to page of full content for post (url- https://blog-it-app-f2464249567c.herokuapp.com/ [post-title]).
  
#### Datetime functionality of posts/updates
- Expected: Datetime is displayed for each post and comment on site: datetime of either the original posting or, if updated, datetime of the update.
- Testing: Datetime of original:
  - For a post- navigate to admin panel and create a new post (https://blog-it-app-f2464249567c.herokuapp.com/admin/blog/post/add/), fill in form fields and publish.
  - Navigate to 'VIEW SITE' to return to Home page.
- Result: New post created with timestamp dsiplayed, both on Home page and on 'post-detail' page.
  - To test the same functionality for comments- fill in the comment form on post detail page and select 'Submit'. Approve comment from the admin panel (in keeping with User Story #6). Refresh 'post-detail' and see timestamp of comment displayed.
- Testing: Datetime of update:
  - Either update a comment by opening a post, navigate to comment section and select 'Edit' underneath a comment, or update a post by navigating to admin panel and
    
#### Next/Previous and pagination
- Expected: Homepage url- always displays a maximum of 6 posts per page- click 'NEXT'/'PREVIOUS buttons to move through posts and access posts that don't fit on the primary display. Functionality in place that only 'NEXT' button for displaying of  6 most recent posts, only 'PREV' button for displaying of <7 earliest posts, and both 'NEXT'/'PREV' options for all intermediate displays.
- Testing:
  (I) Open Homepage (https://blog-it-app-f2464249567c.herokuapp.com/?page=1), most recent 6 posts displayed first. Select 'NEXT >>' button at bottom of page.
  (II) If on url https://blog-it-app-f2464249567c.herokuapp.com/?page=2 - select 'NEXT >>' button at bottom of page.
  (III)  If on url https://blog-it-app-f2464249567c.herokuapp.com/?page=2 - select '<< PREV' button at bottom of page.
  (IV) If on url https://blog-it-app-f2464249567c.herokuapp.com/?page=3 - select '<< PREV' button at bottom of page.

- Result:
  (I) Redirected to url https://blog-it-app-f2464249567c.herokuapp.com/?page=2 - as expected
  (II) Redirected to url https://blog-it-app-f2464249567c.herokuapp.com/?page=3 - as expected
  (III) Redirected to url https://blog-it-app-f2464249567c.herokuapp.com/?page=1 - as expected
  (IV) Redirected to url https://blog-it-app-f2464249567c.herokuapp.com/?page=2 - as expected
  
#### Sign Up/Sign In buttons and Success messages/failure prompts
- Expected: On clicking 'Sign In' (Login page) or 'Sign Up >>' (Register page) after filling in the required forms correctly, user is redirected to homepage where success messages are displayed.
- Testing:
  (I) Register- Fill in all required form fields conforming to specifications given on page (ie., password instructions), and select 'Sign Up>>'
  (II) Login- Fill in all required form fields, and select 'Sign In'.
- Result: For both cases (I) and (II), user is, after completing form action, redirected to Homepage where success messages 'Successfully signed in as [username].' and 'You are logged in as [username]' are displayed.

#### Defensive functionality- Sign Out and Deletion
(I) Deletion
- Expected: When selecting delete (of a comment, or post if admin), options are presented to confirm deletion action, or to cancel action.
- Testing: Comments: Click 'Delete' button to prompt 'Delete comment?' modal. In modal, select 'Close' to cancel action.
- Result: Comments: Action is canceled, user returns to post page with their comment still there, unmodified.
- Testing: Posts: Logged in as admin, go to admin/blog/post/ and open a post. Scroll down and select 'Delete'. Redirected to blog/post/23/delete/, page which gives options 'Yes, I'm sure' or 'No, take me back'. Select 'No, take me back'.
- Result: Posts: Action is canceled, admin is returned to blog/post/23/change/. On viewing posts in admin panel, all posts are present with no change from the view before, and the same on viewing posts on Home page as any site user.
(II) Sign Out
- Expected: When logged in, selecting 'Logout' from navbar redirects to user to be prompted to confirm action.

#### Protection for authenticated users
- Expected: Only logged in users can Submit, Edit, and Delete comments on posts. In case of non-authenticated site visitor browsing a post, 'Log in to leave a comment' message displays above the page footer, in place of 'Leave a Comment' form.
- Testing: Log out and navigate to Homepage. Open a post.
- Result: No functionality to enable leaving a comment if not logged in. 'Log in to leave a comment' message displayed above footer and to right of list of comments. No Edit or Delet buttons for non-authenticated user to toggle.

#### Password requirements
- Expected: To complete sign up action successfully, user needs to fill in all required criteria on the sign-up form, including Username, Password, and Passowrd (again). The value for Password must conform to the specified password requirements and the value for Password (again) must be identical to Password. With all this having been met, the user successfully signs up and can continue browsing.
- Testing: (I) Tested filling in the fields on the sign-up form on the Register page. Username, Password, conforming to specified requirements, and Password (again), identical value to Password. (II) Also tested that specified requirements are upheld by the programming, by filling in intentionally invalid values to fields (e.g. password <8 characters, entirely numeric, entering value for Password (again) that is not equal to value entered in Password, left some required fields blank and tried to complete action).
- Result (I) User sign-up action successfully completed, redirect straight to Home page, with personalised success message ('Successfully signed in as [username]') displayed.
- Result (II) On attempting to complete sign-up by clicking 'Submit', 'Register' page refreshes prompt messages/information for user about invalid form values (e.g., 'Please fill in this field.', 'This password is too short. It must contain at least 8 characters.', 'This password is entirely numeric.').

#### Delete/Edit/Submit buttons
(I) Submit button
- Expected: To post a comment, user moves cursor to 'Submit' button under 'Leave a comment' section after filling in field. Button highlights purple and on selection page refreshes with comment posted beneath 'Comments:' section on left.
- Testing: Input text into Body* of Comment Form. Hover cursor over Submit and select button.
- Result: 'Submit' button highlights purple and on selection, page refreshes with comment posted beneath 'Comments:' section on left.
(II) Delete button
- Expected: To delete a comment, user moves cursor to 'Delete' button underneath the comment. Button text changes colour to black on hover and, on selection, 'Delete comment?' modal is prompted.
- Testing: Select 'Delete' underneath a comment.
- Result: On hover, text changes to black, and on click, 'Delete comment?' modal is prompted.
(III) Delete comment modal
- Expected: Selecting either 'Close' or 'Delete' buttons in modal triggers action- 'Close' cancels the deletion process and refreshes page with no updates made, 'Delete' deletes the comment and refreshes page with this update shown.
- Testing: On generating modal, select 'Close', 'X', or 'Delete'.
- Result: 'Close' or 'X' refreshes page with no deletion update. 'Delete' removes the selected comment from the page, and also generates a success message at the top of page- 'Comment deleted!'.
(IV) Edit button
- Expected: To edit a comment, user moves cursor to 'Edit' button underneath the comment. Button text changes colour to black on hover and, on selection, refreshes whole page with the text of the comment selected for edit prepopulating the body field of the comment form, and 'Update' button in place of 'Submit' for the form.
- Testing: Hover cursor over 'Edit' button and select.
- Result: Button text changes colour to black on hover and, on selection, refreshes whole page with the text of the comment selected for edit prepopulating the body field of the comment form, and 'Update' button in place of 'Submit' for the form.
  [] Update button (in case of Comment edit): expected, tested and result exactly as for (I) Submit button. 

### Responsiveness

### Code Validation

### Features Testing

### Resolved Bugs

### Known Bugs
#### Paragraph tag bug
- HTML validation error in that, running HTML code through W3 Schools validator for post_detail.html from logged in view, a stray <p> opening tag is encided in the post content HTML body.
#### Comment Id bug
- Same HTML validator throwing error with 'comment-id' attribute of <button> element.
---
## Credits
