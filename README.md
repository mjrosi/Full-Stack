# SHOOD Blog

Live site available [here](https://blog-pp4.herokuapp.com/). 


## Table of Contents
--------------------------------------

- [Description](#description)
- [UX](#ux)
- [Agile Development](#agile-development)
- [Features](#features)
- [Testing](#testing)
- [Technologies](#technologies)
- [Deployment](#deployment)
- [Credits](#credits)

## Description
---------------------------------------

SHOOD Blog, the fourth project for the Code Institute Diploma in Software Development, is a website created using Django with Python, CSS/Bootstrap, and HTML. The site offers role-based permissions for users to access a central database, and it includes user authentication and full CRUD functionality for posts.


## UX
*  The blog about SHOOD - the search and comparison engine for grocery shopping and delivery. The blog is dedicated to providing users with all the information they need to know about SHOOD, including how it works, its features and benefits, and how it can help simplify grocery shopping and delivery experience.

### The Sites Ideal User

* The ideal usage of the SHOOD blog is for individuals who are interested in simplifying their grocery shopping and delivery experience. The blog provides valuable information on how to use SHOOD's search and comparison engine to find the best deals and place simultaneous orders from different stores.

### Site Goals

* Educate readers about SHOOD's search and comparison engine for grocery shopping and delivery.
* Provide helpful tips and tricks for optimizing the grocery shopping experience with SHOOD.
* Share news and updates about SHOOD, including new features and partnerships with grocery stores.



## Agile Development

The plan for this project was carried out using the Agile Methodology in Github. User Stories were created using issues on git hub. Each user story explicitly explains the purpose of the issues. Each user story is segmented into acceptance criteria and tasks.


### User Stories
- View post list:
    * As a Site User, I can view a list of posts to select one to read.
- Open a post:
    * As a Site User, I can click on a post to read the full text.
- View likes:
    * As a Site User / Admin, I can view the number of likes on each post to see which is the most popular or viral.
- View comments:
    * As a Site User / Admin, I can view comments on an  individual post to read the conversation.
- Account registration:
    * As a Site User, I can register an account to comment and like.
- Comment on a post:
    * As a Site User, I can leave comments on a post to be involved in the conversation.
- Like / Unlike:
    * As a Site User, I can like or unlike a post to interact with the content.
- Manage posts:
    * As a Site Admin, I can create, read, update, and delete posts to manage my blog content.
- Create drafts:
    * As a Site Admin, I can create draft posts to finish writing the content later.
- Approve comments:
    * As a Site Admin, I can approve or disapprove comments to filter out objectionable comments.

Live to the project in Github [here](https://github.com/users/mjrosi/projects/1/views/1).

![User Story To DO](/media/images/user-story-to-do.png)
![User Story in Progress](/media/images/user-story-progress.png)
![User Story Done](/media/images/user-story-done.png)


## Features

**Features planned:**
* User account - Create, Read, Update and Delete posts.
* Blog posts - Users can comment and like posts
* Users can login to their account.
* Users can logout of their account.
* Users need to be registered and logged in order to comment or like any posts.
* Responsive Design - The site needs to be fully responsive to cover the wide variety of devices and browsers users may use to access the site.


#### Home page
The Front page asks a the visitor of the site to log into view their posts. If already logged in then it displays posts created by the user.

![Home Page](/media/images/home.png)

#### Navigation Bar
The main navigation bar appears at the top of the page, clearly displaying the main navigational links users would require. For sign in and sign up and log out for signed in users.

![Nav Bar](/media/images/header.png)
![Nav Bar](/media/images/header-auth.png)

#### Footer
A common footer is utilised throughout the site with the links to other SHOOD websites which are my other portfolio projects, about SHOOD Blog and link to social medias.

![footer](/media/images/footer.png)

##### View post detail
![Example Post Card](/media/images/postview.png)

#### Sign up
Users can sign up in order to like or comment any posts.
![Sign up](/media/images/signup.png)

#### Sign in
Users can sign in to their accounts.
![Sign up](/media/images/signin.png)

#### 

## Testing

### Testing Strategy
I utilised a manual testing strategy for the development of the site.

#### Testing Overview

Testing was divided into different sections to ensure everything was tested individually with test cases developed for each area.


#### Validator Testing
All code files were validated using suitable validators for the specific language.
HTML & CSS code passed the validation.
There is no JavaScript code to be validated.
Python meets with Pep8 standards except 
* There are some errors regarding line too long- by one character

#### Python Testing
All Custom Python code was manually tested multiple times during and after development.


## Testing User Stories

------
User Story:

> Create a User Account - As a User, I would like to be able to create an account, so that I can create and save posts

Acceptance Criteria:
* Given that I am an unregistered user, When I am on the homepage, Then I can see a button to sign up, And, When I click on the button, Then I am taken to the user registration page.
* Given that I am an unregistered user and I am on the user registration page, When I enter my username, email address and password, And, I click on the register button, Then The system creates me an account, And, signs me in.
* Given that I have an account and I am signed into the account, When I have an option to create a post, And, when I click on that option, Then I am taken to a page where I can provide the details of my post.

Implementation of tests:
* Check for clearly accessible call to action on homepage to register for an account and that it works as expected.
* Clearly accessible link to login or register within main navigation bar and that it functions correctly.
* Easy to use User registration process, user account and profile is created upon submission.
* Clear UX design, prevent unnecessary links to register as a user, if user is already logged in.

All Tests Passed.
---

-----

User Story:

> User Account Login / Logout - As a User, I would like to be able to login or logout of my account, so that I can keep my account secure.

Acceptance Criteria:
* Given that I am a registered user, who is not logged in when I navigate to the sign in page and I enter my credentials correctly and press sign in then I am signed into my account.
* Given that I am a registered user, who is currently logged in when I click on the sign out link then I am signed out of my account.
* Given that I am a registered user, who has signed out of my account when I use the browser navigation buttons such as back button then I can not access information which requires me to be signed in.

Implementation of tests:
* Provide login and logout functionality.
* Secure restricted pages from access when a user is not signed in.

All Tests Passed.
---

-----

User Story:

> Features restricted to Admin - As a Site admin, I would like to: 
* create, read, update, and delete posts to manage my blog content.
* approve or disapprove comments to filter out objectionable comments.

Implementation of tests:
* Site admin can create, read, update, and delete posts to manage my blog content in admin site.
* Site admin can approve or disapprove comments to filter out objectionable comments in admin site.

All Tests Passed.
---

-----

User Story:

> Create a post
 - As a User, I would like to be able to create a post to be able keep a log for future review.

Acceptance Criteria:
* Given that I am a logged in user when I navigate to the 'Add Expense Post' of the home page so I have the option to create a post.
* Given that I have created a post as a logged in user when I save the completed post then it is available to other users to view.

Implementation of tests:
* Provide authenticated users with a clear option to create a post.
* Make saved posts available to other users to view.

All Tests Passed &#x2611;
---

-----

User Story:

> View posts - As a Site User, I can view a list of posts to select one to read.

Acceptance Criteria:
* Given that I am a user on the site when I navigate to the home page then I am presented with a list of the posts i have previously created.
* Given that I am a user on the site when I navigate to the home page And When I click on a post then I am presented with the full post details.

Implementation of tests:
* Provide users of the site with the ability to access all userd posts.
* Provide users of the site with the ability to access the full post details from the post summary card.

All Tests Passed.
---


-----

User Story:

> View likes:
* As a Site User / Admin, I can view the number of likes on each post to see which is the most popular or viral.

Acceptance Criteria:
* Given that I am a user I can see the number of like for each post.

Implementation of tests:
* Provide UI for seeing the number of likes

All Tests Passed.
---



## Technologies

* Python
* Django
    * Django was used as the main python framework in the development of this project.
* Heroku
    * Was used as the cloud based platform to deploy the site on.
* Heroku PostgreSQL
    * Heroku PostgreSQL was used as the database for this project during development and in production.
* Bootstrap 5
    * Bootstrap was used for general layout and spacing requirements for the site.
* Font Awesome
    * Was used for access to the Navvar bars icon for the navigation bar menu.
* CSS
    * CSS was written for a large number of areas on the site to implement custom styling and escape a bootstrap look and feel to the site.
* HTML
    * HTML was used as the base language for the templates created for the site.

#### Packages Used

* Gitpod was used to develop the site
* Git was utilised for version control and transferring files between the code editor and the repository
* GitHub was utilised for storing the files for this project

#### Resources Used

* The Django and Bootstrap documentation was used extensively during development of this project
* The Code Institute reference material was used as a general reference for things that I had previously done during the course.
* Other Resourses we used to help debug and to learn new features not yet covered in the course - Youtube, StackOverflow, GeekForGeeks and Slack.


[Back to the Top](#table-of-contents)

----

## Deployment

The site was deployed via Heroku, and the live link can be found here - [Expensed](https://dashboard.heroku.com/apps/expensed)

### Project Deployment

To deploy the project through Heroku I followed these steps:
* Sign up / Log in to [Heroku](https://www.heroku.com/)
* From the main Heroku Dashboard page select 'New' and then 'Create New App'
* Give the project a name - I entered The-Pantry and select a suitable region, then select create app. The name for the app must be unique.
* This will create the app within Heroku and bring you to the deploy tab. From the submenu at the top, navigate to the resources tab.
* Add the database to the app, in the add-ons section search for 'Heroku Postgres', select the package that appears and add 'Heroku Postgres' as the database
* Navigate to the setting tab, within the config vars section copy the DATABASE_URL to the clipboard for use in the Django configuration.
* Within the django app repository create a new file called env.py - within this file import the os library and set the environment variable for the DATABASE_URL pasting in the address copied from Heroku. The line should appear as os.environ["DATABASE_URL"]= "Paste the link in here"
* Add a secret key to the app using os.environ["SECRET_KEY"] = "your secret key goes here"
* Add the secret key just created to the Heroku Config Vars as SECRET_KEY for the KEY value and the secret key value you created as the VALUE
* In the settings.py file within the django app, import Path from pathlib, import os and import dj_database_url
* insert the line if os.path.isfile("env.py"): import env
* remove the insecure secret key that django has in the settings file by default and replace it with SECRET_KEY = os.environ.get('SECRET_KEY')
* replace the databases section with DATABASES = { 'default': dj_database_url.parse(os.environ.get("DATABASE_URL"))} ensure the correct indentation for python is used.
* In the terminal migrate the models over to the new database connection
* Navigate in a browser to cloudinary, log in, or create an account and log in. 
* From the dashboard - copy the CLOUDINARY_URL to the clipboard
* in the env.py file created earlier - add os.environ["CLOUDINARY_URL"] = "paste in the Url copied to the clipboard here"
* In Heroku, add the CLOUDINARY_URL and value copied to the clipboard to the config vars
* Also add the KEY - DISABLE_COLLECTSTATIC with the Value - 1 to the config vars
* this key value pair must be removed prior to final deployment
* Add the cloudinary libraries to the list of installed apps, the order they are inserted is important, 'cloudinary_storage' goes above 'django.contrib.staitcfiles' and 'cloudinary' goes below it.
* in the Settings.py file - add the STATIC files settings - the url, storage path, directory path, root path, media url and default file storage path.
* Link the file to the templates directory in Heroku TEMPLATES_DIR = os.path.join(BASE_DIR, 'templates')
* Change the templates directory to TEMPLATES_DIR - 'DIRS': [TEMPLATES_DIR]
* Add Heroku to the ALLOWED_HOSTS list the format will be the app name given in Heroku when creating the app followed by .herokuapp.com
* In your code editor, create three new top level folders, media, static, templates
* Create a new file on the top level directory - Procfile
* Within the Procfile add the code - web: guincorn PROJECT_NAME.wsgi
* In the terminal, add the changed files, commit and push to GitHub
* In Heroku, navigate to the deployment tab and deploy the branch manually - watch the build logs for any errors.
* Heroku will now build the app for you. Once it has completed the build process you will see a 'Your App Was Successfully Deployed' message and a link to the app to visit the live site.


[Back to the Top](#table-of-contents)

-----

## Credits

All Images used across the site were sourced from either freepik.com, freely available images.
The Navbar bars Icon was taken from font awesome.

I relied heavily on the Code institute course work, particularly the I Think Therefore I Blog walk through projects.

[Back to the Top](#table-of-contents)
