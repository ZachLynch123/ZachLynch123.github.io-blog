---
layout: post
title:      "Sinatra Dungeons and Dragons Project"
date:       2020-08-23 20:12:07 +0000
permalink:  sinatra_dungeons_and_dragons_project
---


This is my Sinatra MVC project where users can sign in to and also create, read update and delete character sheets for their Dungeons and Dragons runs.

For this project I created two models. One for the user which have secure passwords as well as a "has_many" attribute, since every user can have many character sheets. The other model is for the Characters themselves. Which they have an attribute called "belongs_to" because each character is going to belong to a user. 

Each model has their own database table associated with them, user has their username and password. Whereas the Charater has name, class, race, and stats. As well as a user_id column, which is a foreign key to link each user with their respective characters.

I also made sure to make separate view folders and controllers for the specific models in order to maintain the idea of seperation of concerns. Allowing the application to handle logins, logouts, and sign ups, where as the users controller handled the users page and the characters controller handled the creation, updating, and deletion of any character sheet. 

All in all, a great project to test knowledge of the MVC framework.
