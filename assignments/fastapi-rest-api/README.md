# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI to manage a collection of books. Practice defining HTTP endpoints, validating request data, returning appropriate status codes, and testing API behavior.

## 📝 Tasks

### 🛠️ Create the Book API

#### Description
Create a FastAPI application that serves a collection of books stored in memory. Each book should have an integer `id`, a `title`, and an `author`.

#### Requirements
Completed program should:

- Create a FastAPI application in `main.py` and run it locally with Uvicorn.
- Add `GET /books` to return all books as JSON.
- Add `GET /books/{book_id}` to return one book by its ID.
- Return an HTTP `404 Not Found` response when the requested book does not exist.
- Include at least three example books when the application starts.


### 🛠️ Add Book Management Endpoints

#### Description
Extend the API so clients can create, update, and delete books. Use Pydantic models to validate incoming request bodies.

#### Requirements
Completed program should:

- Define a Pydantic model for book data with required, non-empty `title` and `author` fields.
- Add `POST /books` to create a book, assign it a unique integer ID, and return the created book with HTTP `201 Created`.
- Add `PUT /books/{book_id}` to replace a book's title and author, returning `404 Not Found` if the ID does not exist.
- Add `DELETE /books/{book_id}` to remove a book, returning HTTP `204 No Content` on success and `404 Not Found` if the ID does not exist.
- Confirm invalid request data is rejected with HTTP `422 Unprocessable Entity`.


### 🛠️ Filter and Test the API

#### Description
Make it possible to search books by author and write automated tests for the API using FastAPI's `TestClient`.

#### Requirements
Completed program should:

- Allow `GET /books?author=<name>` to return books whose author matches the query, without changing the behavior of `GET /books` when no filter is provided.
- Add automated tests for listing books, retrieving a missing book, creating a book, and filtering by author.
- Run the tests successfully and verify the endpoints in FastAPI's interactive documentation at `/docs`.
