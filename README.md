# Digital Lending Library
 #### Video Demo:  <
 #### Introduction
 Hello,my name is Tasos Fasoulis, I live in Athens, Greece and this is my submission to the CS50 2021 final project. 
 My project is called digital library and it is a web application where the users have the ability to donate a book to a library and also rent a book that another user has donated. It works like a lending library, but in digital format.

 #### Features
 In order to implement this application I used python, SQL, flask, html and css.

 #### Description of files
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
	
 #### Descritpion of application
 First, the user should register for the web page, by giving a username and a password, which must be at least 6 characters long. Then, the user can log in and navigate to the web page. The actions that the users can make are:
 - donate a book to the library.
 - rent a book from the library for a specific period.
 - return a book that they have rented.
 - see a history of their actions.
 Each page of the application is described analytically below.

 #### Register and Log in
 In the register page, the user is asked to give a username and a passwword, which the user must confirm in also to succesfully register to the page.
![register](https://github.com/tasosfas/test/blob/main/Register.JPG)

 Then, the user should log in using his/hers credentials.
![log in](https://github.com/tasosfas/test/blob/main/login.JPG)

 #### Index page
 After the user has loged in, he/she will be redictered to the index page, where the user is welcomed to the library and can see a shortly documentation about the actions that are available in this web application.
![index](https://github.com/tasosfas/test/blob/main/index.JPG)


 #### Donate a book
 In this page, the user can donate a book to the library. The user should specify the name of the book and the quantity he/she wants to donate (in case someone has many copies of a book and wants to donate more than one copy to the library).
![donate](https://github.com/tasosfas/test/blob/main/donate.JPG)

 #### Rent a book
 In this page, the user can select the title of the book which he/she wants to rent and the number of days he/she wants to hold it. The user can only rent books which have been donated by other users, so if a book is not in the library the user will see an error message.
 ![rent](https://github.com/tasosfas/test/blob/main/rent.JPG)
 
 #### Return a book
 In this page the user can return a book which has previously rented, so this book will become again available for the other users. In the form, the user enters the title of the book he/she wants to return. If the user types a book that has not rented previously, he/she will see an error message.\
 ![return](https://github.com/tasosfas/test/blob/main/return.JPG)
