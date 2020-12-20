# Library Management System using Django

The project aims at giving the learner a hands-on experience on the implementation of backend development using Django.

## Project Specifications
The finished project should be able to fulfill the following requirements:
- Maintain a database of books in a library
- Store multiple entities for a book like title, author, genre, ISBN, cover image, user ratings/reviews etc.
- Ability to sort books based on author, genre, average user rating
- Implement CRUD (Create, Read, Update and Delete) functionality from the admin panel
- Allow non-admin users to sign-up/login and add a book to their favorites and upload a rating/review

## Prerequisites
- **Python**<br>
  As Django framework uses Python, a fair understanding of the language would be required to successfully do the project.<br>
  Yet to study Python? No worries, you can view our content from [CodeInQuarantine, Week 1](https://github.com/wncc/CodeInQuarantine/tree/master/Week_1_Python).
  
- **Front-End Web Development (HTML/CSS/JS)**<br>
  This isn't as important as learning Python, but atleast a basic knowledge will be necessary to understand Backend Development.<br>
  Want to learn Frontend Development? Take a look at our Learners' Space course on [Web Deveopment](), Weeks 1-3.<br>
  
- **Django**<br>
  Django is the what you will actually be using to implement the project.<br>
  Here is a [link](https://github.com/wncc/learners-space/blob/master/Web%20Development/Week%205/README.md) for a detailed guide to study Django.<br>
  Just ensure that you have an overall idea of how it works and you can build upon that while doing the project.
  
Now that we understand what it takes to get started, let's cut to the chase and start building our project!
  
## Pathway
- Very first thing is to install Python. Download it from the [official downloads page](https://wiki.python.org/moin/BeginnersGuide/Download)
- Next is to set up a virtual environment. You can follow the steps [here](https://github.com/wncc/learners-space/blob/master/Web%20Development/Week%205/supplements/virtualenv.md).
- Within the virtual environment, install Django using `python -m pip install Django`
- Now create a directory for your project and in the folder run `django-admin startproject <project_name>`
- Ensure that everthing has been correct so far by running your server using `python manage.py runserver`. 
Navigate to localhost:8000 from the browser to check if the server is running fine.

This ends the setup part; now onto the actual project

- Now go on to create the library app and add models for the required feilds.
- Add a superuser account to access the Django admin panel
- Make CRUD models available from the admin interface
- Add a user registration form and create a user's page for registered users
- Add the rest of the functionality as per the specifications

**Note:** The steps mentioned above are just an overview guide for making the project. 
We encourage the learners to figure out the specifics themselves through discussions and self-learning. 
Coming up with more ideas to improve upon the project and implementing them by oneself is highly recommended and will help enhance learning further.

That's it!<br>
You have successfully implemented a Library Management System using Backend Development with Django. <br>
We hope that this project has been helpful in your journey towards becoming a Backend Developer!

<p align="center">Created with :heart: by <a href="https://www.wncc-iitb.org/">WnCC</a></p>
