# SQL-Stored-Procedures-and-Functions
This repository contains examples of Stored Procedures and a Function for the Library Management System database.

## 📂 File Included
•⁠  ⁠⁠ library_reusable_blocks.sql ⁠
  - Stored Procedure: ⁠ GetBorrowingsByMemberName ⁠ – Returns borrowing details for a given member name.
  - Stored Procedure: ⁠ AddNewMember ⁠ – Adds a new member if they do not already exist.
  - Function: ⁠ GetAuthorBookCountByName ⁠ – Returns the total number of books written by a given author.

## 🗃️ Tables Used
•⁠  ⁠⁠ members ⁠
•⁠  ⁠⁠ borrowings ⁠
•⁠  ⁠⁠ books ⁠
•⁠  ⁠⁠ authors ⁠

## 💡 Usage
1.⁠ ⁠Ensure the ⁠ librarydb ⁠ schema and tables exist.
2.⁠ ⁠Run ⁠ library_reusable_blocks.sql ⁠ to create the procedures and function.
3.⁠ ⁠Call them using:
   ```sql
   CALL GetBorrowingsByMemberName('Alice Smith');
   CALL AddNewMember('Charlie Brown', '2025-08-14');
   SELECT GetAuthorBookCountByName('George Orwell') AS total_books;
