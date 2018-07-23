# PODS_Assignment_5

Principle of Database System
 
This is an extension of the library database system we have worked in the previous assignments. Implement a Library Database 
Management system – Admin console using Oracle JDBC. Name your program as "LibraryAdminDb.java". 
 
The implementation is better explained using a screen capture of a sample run of the program given below. The user input is 
shown in bold. The MENU keeps on repeating until the user selects the choice 4 (Exit). At each step, where needed, comments 
are appropriately provided in the script file between /*..... */. However, such comments are provided for your understanding 
and should not appear in the file that you submit. 
 
We will use the library database schema available at library.sql (click to open the file). Use the borrower_seq object to 
generate unique sequence card no values for new borrowers. See the library.sql file.
 
Submission: Zip all your files and submit electronically using http://d2l.mu.edu. Also, submit sample execution screen 
shots/test case reports of running your program. Name the main program as LibraryAdminDb.java.
 
%java LibraryAdminDb
 
Enter your database username : <place holder for database user name>
Enter your database password : <database password>
 
Welcome to the Library Database Management System (Admin)
 
MENU
****************************************************
(1) Enter a new Borrower
(2) Check-out a Book for a Borrower
(3) Check-in a Book for a Borrower
(4) Exit
****************************************************
 
 
Please make your choice : 1
 
Please enter Borrower Name  (firstname lastname) : John Smith
Please enter Borrower Address : 678 Wisconsin Ave, Milwaukee, WI
Please enter Phone number (xxx-xxx-xxxx) : 123-789-7845
 
Borrower Record inserted successfully. The borrower’s card no is : 12003
 
 
MENU
****************************************************
(1) Enter a new Borrower
(2) Check-out a Book for a Borrower
(3) Check-in a Book for a Borrower
(4) Exit
****************************************************
 
Please make your choice: 2
 
Borrowers along with their card numbers are:
 
Davolio (1)
Fuller (2)
John Smith (12003)
Leverling (3)
 
Please enter the borrower card no: 1
Please enter the book id:  1035
Please enter the branch id: 6380
 
Successfully checked out the book - But Is It User Friendly? (1035) for Davolio(1). The book is due by : November, 26th, 2016.
 
/* When inserting the row into book_loans table, the date out should be defaulted to current date and time, and the due date 
should be one month from the date out. The date in and rating columns should be null. Also, meaningful error messages need to 
be displayed if any referential or primary constraints are violated. */
 
MENU
****************************************************
(1) Enter a new Borrower
(2) Check-out a Book for a Borrower
(3) Check-in a Book for a Borrower
(4) Exit
****************************************************
 
Please make your choice: 3
 
Borrowers along with their card numbers are:
 
Davolio (1)
Fuller (2)
John Smith (12003)
Leverling (3)
 
Please enter the borrower card no: 1
Please enter the book id:  1035
Please enter the branch id: 6380
 
Successfully checked in the book - But Is It User Friendly? (1035) for Davolio(1). The book has been returned by the due 
date. There is no late charge.
 
/* The datein column for the matching row in the book_loans table should be updated to the current date. Also, if the book is 
overdue, charge a late fee of 30cents for each late day after the due date.  Meaningful error messages need to be displayed if 
any referential or primary constraints are violated. */
 
MENU
****************************************************
(1) Enter a new Borrower
(2) Check-out a Book for a Borrower
(3) Check-in a Book for a Borrower
(4) Exit
****************************************************
 
Please make your choice: 4
 
%exit

