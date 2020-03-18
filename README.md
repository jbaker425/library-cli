# library-cli
Library SQL Application

-The LibraryManagementApplication.doc file is the prompt we were given.

-Run librarySchema.sql then insertLibraryData.sql in MySQL Workbench to set up the tables and fill them with test data
(It connects with USER: root, PSWD: root)

Run the rest in Python 3:
  -Run the two helper files, first check.py, then librarysql.py (this file is where you can change your normal username, password, and connection IP)
  -Run the three files for the roles in any order: borrower.py, librarian.py, admin.py
  -Run the driver file to run the application: project.py
 
Known Bugs:
-When deleting a publisher, it will throw an error if there are books that use it as a foreign key, could be fixed with a cascade
-When overriding a due date, there is insufficient input checking when typing in the date, so the date must be typed correctly, or else it will throw an error.
