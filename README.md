# Python CRUD Application for Library Management System

A comprehensive Python application for managing [Data Entity] data with Create, Read, Update, and Delete (CRUD) operations.

## Business Understanding

This project caters to the library management industry, specifically addressing the need to manage book loan transactions efficiently. Book lending plays a crucial role in maintaining an organized and systematic borrowing process in libraries, ensuring users can access books while keeping track of their return deadlines.

**Benefits:**

- Improved book inventory tracking

- Automated borrowing and returning process

- Enhanced user experience with book search and loan extensions

- Secure access to administrative functionalities

- Historical tracking of book loans for analysis and audit purposes

**Target Users:**

This application is designed for librarians and library members to facilitate book borrowing, returning, and transaction management.

## Features

- **Create:**
  - Add new books to the library inventory.
  - Record book loans by associating books with borrowers.
- **Read:**
  - View the list of available books.
  - Search for books or borrowers based on ID or name.
  - Retrieve transaction history to track borrowed and returned books.
- **Update:**
  - Allow borrowers to extend the loan period once.
  - Modify the book status when borrowed or returned.
- **Delete:**
  - Admins can delete transaction history after authentication.
  - Deleted records are stored in a recycle_bin directory in a CSV file.
- **Security:**
  - Implement admin authentication and authorization mechanisms (if sensitive data is involved) to control access to different CRUD operations.
- **Reporting:**
  - Displays a summary of book borrowings and returns.
  - Saves deleted transaction history for record-keeping.

## Installation

1. **Prerequisites:**

   - Python 3.x

2. **Installation:**

   ```bash
   git clone https://github.com/fakhrimaulanaherza/Library_System_Administration.git
   cd Library_System_Administration
   ```

## Usage

1. **Run the application:**

   ```bash
   python main.py
   ```

2. **CRUD Operations:**
   - **Create:** Add a new book entry or borrow a book by specifying book ID, borrower name, and NIK.
   - **Read:** View available books and loan history.
   - **Update:** Extend a loan period if conditions are met.
   - **Delete:** Remove transaction history (admin access required).

## Data Model

This project utilizes a dictionary-based data structure to store book and transaction data. The following fields are used:

## Books Data:

- ID: (Integer) - Unique identifier for each book.
- Title: (String) - Name of the book.
- Status: (String) - Availability of the book (available or not available).

## Transactions Data:

- Book ID: (Integer) - References the borrowed book.
- NIK: (String) - Unique identification number of the borrower.
- Name: (String) - Name of the borrower.
- Borrow Date: (Datetime) - The date the book was borrowed.
- Return Date: (Datetime) - The date the book was returned (if applicable).
- Notes: (String) - Additional remarks on book condition.
- Extension Count: (Integer) - Number of times the loan has been extended.

## Future Enhancements:

- Integration with a database for persistent data storage.
- Web-based UI for better user interaction.
- Notification system for due dates and late returns.

## Contributing

We welcome contributions to this project! Please feel free to open a pull request, sent to [fakhrimaulanaherza@gmail.com] or submit an issue if you encounter any problems or have suggestions for improvements.
