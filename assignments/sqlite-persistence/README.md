# 📘 Assignment: Adding SQLite Persistence to a FastAPI App

## 🎯 Objective

Extend the book API from the FastAPI assignment to store books in a SQLite database using Python's built-in `sqlite3` module. Practice creating a table and reading and changing records so that data remains available after the app restarts.

## 📝 Tasks

### 🛠️ Create the Books Database

#### Description
Replace the API's in-memory book collection with a SQLite database. Create the database and its `books` table when the application starts.

#### Requirements
Completed program should:

- Create a SQLite database file and a `books` table with `id`, `title`, and `author` columns.
- Keep the existing three example books available, adding them only when the table is empty.
- Use parameterized SQL statements when inserting or searching for book data.
- Use Python's `sqlite3` module; no third-party database library is required.


### 🛠️ Connect the API to SQLite

#### Description
Update the existing book endpoints to read and change records in SQLite rather than an in-memory list.

#### Requirements
Completed program should:

- Keep the existing list, retrieve, create, update, and delete endpoints working with database records.
- Preserve the existing response shapes and status codes, including `404 Not Found` for missing books, `201 Created` for a new book, and `204 No Content` for a deleted book.
- Keep author filtering available on `GET /books?author=<name>`.
- Return created and updated book details from the saved database record.


### 🛠️ Verify Data Persists

#### Description
Check that database-backed behavior works and that saved books remain after the API process is restarted.

#### Requirements
Completed program should:

- Add or update automated tests to cover listing, creating, filtering, updating, and deleting books.
- Verify that a created book is still available after restarting the application.
- Run the tests successfully and confirm that deleting a book removes it from subsequent API responses.
