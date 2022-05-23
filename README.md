# Library-Management-System - with GUI Implementation
This is a group project, done in collaboration with team members Masroor Ahmed and Aftab Ali.
University: FAST - NUCES Islamabad
Course: Software Engineering (CS3009)


### The Library Management system provides following functionalities:

* Login
* Add a book
* Search a Book based on Book Title
* Search Books based on Category
* Search Books based on Author
* List All Books along with author information
* Issue Book to Student
* List Books issued to Student based on USN number 
* List books which are to be returned for current date

### Working

* A user can add book by providing the following information, title, ISBN (Book Number), category and Author information (Author Name and Phone Number).
* Book search can be based on book title, or category or Author, when a book is found, entire information has to be printed on the screen. Partial searches to be supported (for example, if user searches by ‘ja’, ‘Java Complete Reference’, ‘Head First Java’ books) should be displayed.
* A user can list all books present in the library and also the books issued to the students using their USN number.
* A book can be issued to a student by first selecting a book from list of books and then selecting the student from the list of partial or complete search result. Also the date of issue is saved while issuing and return date is calculated (i.e. 7 days from issue date).
* Also if the book is not in library, the user should be informed about the unavailability of the book.


### Database Design

Book Table  | -
----------- | ------------------
Book ISBN	| Primary key
Book Title	| Varchar
Category	| Varchar
No of Books	| int

</br>

Author Table	| -
------------ 	| ----------------------	 
Author Name	 	| Varchar
Author Mail Id	| Varchar
Book ISBN		| Foreign KEY, References Book

</br>

Student Table | -
------------- | --------------------
USN			  | Varchar, Primary Key
Name		  | Varchar

</br>

Book ISSUE Table | -
---------------	 | --------------------------------
Issue ID		 | Auto Increment, Primary Key
USN				 | Foreign Key, References Student
Issued Date		 | Date
Return Date		 | Date
Book ISBN		 | Foreign Key, References Book 

</br>

ADMIN Table		| -
--------------- | --------------------
Admin Id		| Varchar, Primary key
Password		| Varchar

</br>
</br>


### Screenshots

* Login Screen

![picture alt](https://github.com/Sourav-Malani/Library-Management-System/blob/main/Library-Management%20System/screenshots/login1.png)

</br>
</br>

* Add new Book

![picture alt](https://github.com/Sourav-Malani/Library-Management-System/blob/main/Library-Management%20System/screenshots/add_book.png)

</br>
</br>

* Search Book

![picture alt](https://github.com/Sourav-Malani/Library-Management-System/blob/main/Library-Management%20System/screenshots/search_book.png)

</br>
</br>

### Demo
* Install MariaDB and follow the steps given in [this](https://github.com/Sourav-Malani/Library-Management/blob/master/Database_Query/bookDB.txt) file.
* Now download this project and go to [dist folder](https://github.com/Sourav-Malani/Library-Management/tree/master/dist)
* Double click on LibraryManagement.jar and you are good to go:)
