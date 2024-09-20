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

-----


---
## Credits
