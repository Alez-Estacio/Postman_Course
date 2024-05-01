# Library API - Documentation

This repository contains the documentation for the Library API, which provides endpoints for managing books and user skills.

## Available Endpoints

### Get all books

GET /books

This endpoint returns all the available books in the library.

### Get fiction books

GET /fiction-books

Returns all the fiction books available in the library.

### Get book by ID

GET /books/:id

Returns information about a specific book identified by its ID.

### Add a book

POST /books

Allows adding a new book to the library.

### Update book status

PATCH /books/:id/checkout

Marks a book as "checked out", indicating it has been borrowed.

### Delete a book

DELETE /books/:id

Deletes a book from the library.

### Perform a skill check

POST /skill-check

Allows performing a skill check.

## Usage

To use this API, you can send HTTP requests to the mentioned endpoints using any HTTP client or API testing tool like Postman.

Make sure to include necessary data in the requests, such as the request body for adding a book or the book ID in requests that require it.
