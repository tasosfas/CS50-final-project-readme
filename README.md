﻿# CS50 Final Project
Hello,my name is Tasos Fasoulis, I live in Athens, Greece and this is my submission to the CS50 2021 final project. 
My project is called digital library and it is a web application where the users have the ability to donate a book to a library and also rent a book that another user has donated. It works like a lending library, but in digital format.

# Features
In order to implement this application I used python, SQL, flask, html and css.

# Description of files

 - application.py: a python script which runs the whole web application.
 - helpers.py: a python script with functions for apology messages and login (derived from CS50 finance project)
 - library.db: the database which stores all the data needed for the application in order to run. It contains five tables: 
	 1. users: contains all the information abou the registered users.
	 2. books: contains all the information about the books that are available.
	 3. donations: contains all the information about the book donations that the users have made.
	 4. rents: contains all the informations about the rents that the users have made.
	 5. returns: contains all the informations about the book returns that the users have made.
 - README.md: this file, which explains how the application works. 
 - requirements. txt: the file that contains the python libraries that are required for this application.
 - style.css (in static folder):  A css script which controls the style of the html pages.
 - the templates folder, which contains these html files:
	 - layout.html: the file which contains the basic elements for each page.
	 -  index.html: the file that creates the introduction (index) page.
	 - register.html: the file that creates the page for user registration (derived from CS50 finance project).
	 - login.html: the script that creates the log in page (derived from the CS50 finance project).
	 - apology.html: the script that creaters the pages shown when an error is occured (derived from the CS50 finance project).
	 - donate.html: the script that creates the page where the user can donate a book to the library.
	 - rent.html: the script that creates the page where the user can rent a book.
	 - return_book.html: the script that creates the page where the user can return a book which has already rented.
	 - history.html: the script that creates the page where the user can see all the actions that he/she has made.
	
# Application description
	This application is a web page where the users can donate books in the library and also rent books, which other users have donated.
	First, the uses should register for the web page, by giving a username and a password, which must be at least 6 characters long. Then, the user can log in and navigate to the web page. The actions that the users can make are:
 - donate a book to the library.
 - rent a book from the library for a specific period.
 - return a book that they have rented.
 - see a history of their actions.
 Each page of the application is described analytically below.

# Registed and Log in
	In the register page, the user is asked to give a username and a passwword, which the user also has to confirm it.
	 
![Getting Started](./register.JPG)\

