---
layout: post
title:      "CLI Final Project"
date:       2020-06-26 21:55:16 +0000
permalink:  cli_final_project
---





Hi my name is Zach and this is my CLI final project.

For the project I created a weather CLI tool to grab data from a weather API and display it to the user given the city they searched for. 



Main is the start of the program, or what file is intitially used to begin the program. I made sure that repeat is always true in order to make searching for multiple cities easier. The program runs until ctrl C is imputed to the CLI. 

There are two functions in main to note. Get city formats the city entered to make sure to omit any spaces like in las vegas or salt lake city, and get weather that initializes all the classes with the city entered. Lets take a look at the classes to see what’s goin on under the hood 

Weather data

This is where the weather API is called. I used string interpolation to make things a bit easier to understand. Here we have 3 method variables, the location or city, URL which is the api endpoint, and res, which saves the response, as well a class variable of all which is an array that saves every instance of the class. Get response uses the API endpoint to get the data and adds response to the response variable. Also adds the class instance to the all variable. Parse json is what gets called in main and returns the parsed data for easier access.

Display

Taking a look at display shows that it takes the data and oganizes it to be displayed to the screen. 
To run the program all you have to do is type "ruby main.rb" into the command line, enter a city and the data displays neatly for the user to see. 
