---
layout: post
title:      "Rails Project"
date:       2020-10-25 19:52:31 +0000
permalink:  rails_project
---


This is my rails project I named Rubrary. It's a website built in the MVC framework that allows users to log in using the standard login route, or using their github account. The user can then add books to the website by giving the book a name an a description. The book will then be posted for all users to see, and they can comment on said books. 

The models have validation to prevent any invalid data going into database. I also made sure to include association between all the models by using has many through and belongs to. Each book has many comments, and has many users through the comments. Each user has many comments, and has many books through their comments. 

Each View with a form has error handling using pluralize. If there is an error submitting the form, the user will be alerted to the error and shown the message as to why the form didn't submit. Each form I created I used the form_with helper method because I thought it looked super clean, as well as seeing form_for was "soft deprecated" on the rails website. 


The controllers are where the magic happens. The application controller has many methods that check and make sure a user is logged in. Users controller is used for the standard way users sign up. Sessions controlls creating the session and handling any OAuth logins. Which to be honest was probably the hardest part of this project. I made sure to use a .where ActiveRecord Query method on my comment model to find all the comments where the book id was the same as the book id in the params.

Overall this project was fun to build and has a lot of different, seperate components working together to make one cohesive website. Interesting to see that our favorite websites we use everyday impliment these sorts of practices and we didn't even realize it until now. 


