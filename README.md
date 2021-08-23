# Digital Lending Library
 #### Video Demo:  <
 #### Introduction
 Hello, World! my name is Tasos Fasoulis, I live in Athens, Greece and this is my submission to the CS50 2021 final project. 
 My project is called Digital Lending Library and it is a web application where the users have the ability to donate a book to a library and also rent a book that another user has donated. It works like a lending library, but in digital format. The idea is to create a place where all the book lovers can share their books and also find interesting books they have not read yet. Since we live in the COVID-19 era (this project was submitted in summer 2021) it would be better if this library was created in a digital form, so as to prevent overcrowding. Of course, the users should donate books they own legally, and do not violate any copyright law.

 #### Languages used
 In order to implement this application I used these programming languages: Python, SQL, HTML and CSS.

 #### Description of files
 - application.py: a python script which runs the whole web application.
 - helpers.py: a python script with functions for apology messages and login (derived from CS50 finance project)
 - library.db: the database which stores all the data needed for the application in order to run. It contains five tables: 
	 1. users: contains all the information about the registered users.
	 2. books: contains all the information about the books that are available.
	 3. donations: contains all the information about the book donations that the users have made.
	 4. rents: contains all the information about the rents that the users have made.
	 5. returns: contains all the information about the book returns that the users have made.
 - README.md: this file, which explains how the application works. 
 - requirements.txt: the file that contains the python libraries that are required for this application.
 - style.css (in static folder):  A css script which controls the style of the html pages.
 - the templates folder, which contains these html files:
	 - layout.html: the file which contains the basic elements for each page.
	 - index.html: the file that creates the introduction (index) page.
	 - register.html: the file that creates the page for user registration (derived from CS50 finance project).
	 - login.html: the script that creates the log in page (derived from the CS50 finance project).
	 - apology.html: the script that creates the pages shown when an error is occured (derived from the CS50 finance project).
	 - donate.html: the script that creates the page where the user can donate a book to the library.
	 - rent.html: the script that creates the page where the user can rent a book.
	 - return_book.html: the script that creates the page where the user can return a book which he/she has already rented.
	 - history.html: the script that creates the page where the user can see all the actions that he/she has made.
	
 #### Description of application
 First, the user should register for the web page, by giving a username and a password, which must be at least 6 characters long. Then, the user can log in and navigate to the web application. In this application, the user can donate a book he/she owns to the library, or rent a book for a specific number of days. The user should also return any book he/she has rented back to the libary. Finally, the user can also see a history of his/hers account. More specifically, the actions that the users can make are:
 - donate a book to the library.
 - rent a book from the library for a specific period.
 - return a book that he/she have rented.
 - see a history of his/hers actions.
 Each page of the application is described analytically below.

 #### Register and Log in
 In the register page, the user is asked to give a username and a password, which must be at least 6 characters long. Also, the user must confirm the password in order to successfully register to the application.
![register](https://github.com/tasosfas/test/blob/main/Register.JPG)

 Then, the user should log in using his/hers credentials.
![log in](https://github.com/tasosfas/test/blob/main/login.JPG)

 #### Index page
 After the user has logged in, he/she will be redirected to the index page, where the user is welcomed to the library and he/she can see a shortly description about the actions that are available in this web application.
![index](https://github.com/tasosfas/test/blob/main/index.JPG)

 #### Donate a book
 In this page, the user can donate a book to the library. The user should specify the title of the book and the quantity he/she wants to donate (in case someone wants to donate more than one copy of the same book). After the donation has been done successfully, the user is redirected to the index page.
![donate](https://github.com/tasosfas/test/blob/main/donate.JPG)

 #### Rent a book
 In this page, the user can enter the title of the book which he/she wants to rent and the number of days he/she wants to hold it. The user can only rent books which have been donated to the database, so if a book is not in the library the user will see an error message. After the rent has been done successfully, the user is redirected to the index page.
 ![rent](https://github.com/tasosfas/test/blob/main/rent.JPG)
 
 #### Return a book
 In this page the user can return a book which he/she has previously rented, so this book will become again available for renting by other users. In the form, the user enters the title of the book he/she wants to return. If the user types a book that he/she has not rented previously, he/she will see an error message. After the return has been done successfully the user is redirected to the index page.
 ![return](https://github.com/tasosfas/test/blob/main/return.JPG)
 
 #### History
 In this page the user can see all the actions of his/hers account. This page includes these tables
 - Rents: The books that the user currently holds. The table shows the title of the book, the date that has been rented, the number of days that the book has been rented and the date that the user must return the book.
 - Donations: The books that the user has donated to the library. The table shows the title of the book, the quantity and the date of the donation.
 - Returns: The books that the user has returned to the library. The table shows the title of the book and the date that it was returned.
 ![history](https://github.com/tasosfas/test/blob/main/history.JPG)
