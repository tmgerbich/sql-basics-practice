<!-- # sql-basics-practice

Steps:

1. Created a database in github repo in VSC using:

touch BookStore.db

2. Then opened a new terminal initialize the db using:

sqlite3 BookStore.db

3. Ran the following commands in the sqlite terminal and/or sqlite gui:

CREATE TABLE Books (
BookID int,
Title varchar(255),
Author varchar(255),
PublicationYear int,
Price float,
PRIMARY KEY (BookID)
);

INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES (1, 'Green Eggs and Ham', 'Dr Seuss', 1960, 5.25);
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES (2, 'Where the Wild Things Are', 'Maurice Sendak', 1963, 6.75);
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES (3, 'Each Peach Pear Plum', 'Janet Alhberg', 1955, 4.00);
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES (4, 'Jamberry', 'Bruce Degen', 1995, 5.00);
INSERT INTO Books (BookID, Title, Author, PublicationYear, Price) VALUES (5, 'The Rainbow Fish', 'Marcus Pfister', 1993, 4.50);

SELECT * FROM Books;
SELECT * FROM Books WHERE PublicationYear>2000;
SELECT * FROM Books Where Author = 'Maurice Sendak';
UPDATE Books SET Price = 6 WHERE BookID = 1;
DELETE FROM Books WHERE BookID = 5;

Reflection:
The most challenging part of this assignment was setting up SQLite3 and creating the databbase. The installation instructions were a bit confusing and at I was swapping back and forth between doing things in the command line, VSC, and the GUI. Once I had a handle on the tools, the actual assignment to add and manipulate the data was quite straightforward. None of the operations were particularly complex and the language used by SQL is very straightforward and intuitive. I imagine though that working with real data that is much larger and more complex than these simple examples would be challenging, particularly when getting to the point where one cannot easily confirm that the code is doing the expected things with simple visual checks of the table. -->
