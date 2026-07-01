# Library API - Postman Collection & API Documentation

## Overview

This repository contains a **Postman collection** and API documentation for the **Library API**.

The collection is designed to support API testing and request workflow validation for book management and skill-check operations. It includes endpoints for retrieving books, filtering fiction books, creating new books, checking out books, deleting books, and performing skill checks.

## Repository Contents

```text
Postman_Course/
├── Postman Library API v2.postman_collection.json   # Postman collection
└── README.md                                       # API documentation
```

## Tech Stack

* Postman
* REST API
* JSON
* HTTP Methods
* API Testing

## Prerequisites

Before using this project, make sure you have the following installed:

* Postman
* Git

## Installation

Clone the repository:

```bash
git clone https://github.com/Alez-Estacio/Postman_Course.git
```

Navigate to the project folder:

```bash
cd Postman_Course
```

## Importing the Collection in Postman

To use the API collection:

1. Open Postman.
2. Click **Import**.
3. Select the file:

```text
Postman Library API v2.postman_collection.json
```

4. Import the collection into your workspace.
5. Configure the API host or base URL according to the target environment.
6. Start sending requests from the imported collection.

## Available Endpoints

| Method | Endpoint              | Description                                           |
| ------ | --------------------- | ----------------------------------------------------- |
| GET    | `/books`              | Retrieves all available books in the library.         |
| GET    | `/fiction-books`      | Retrieves all fiction books available in the library. |
| GET    | `/books/:id`          | Retrieves a specific book by its ID.                  |
| POST   | `/books`              | Adds a new book to the library.                       |
| PATCH  | `/books/:id/checkout` | Updates a book status to checked out.                 |
| DELETE | `/books/:id`          | Deletes a book from the library.                      |
| POST   | `/skill-check`        | Performs a skill-check request.                       |

## Endpoint Details

### Get All Books

```http
GET /books
```

Returns the full list of books available in the library.

### Get Fiction Books

```http
GET /fiction-books
```

Returns the list of fiction books available in the library.

### Get Book by ID

```http
GET /books/:id
```

Returns the details of a specific book using its unique ID.

### Add a Book

```http
POST /books
```

Creates a new book record in the library.

The request must include the required book information in the request body according to the API specification.

### Check Out a Book

```http
PATCH /books/:id/checkout
```

Updates the status of a book to indicate that it has been checked out or borrowed.

### Delete a Book

```http
DELETE /books/:id
```

Deletes a specific book from the library using its unique ID.

### Perform a Skill Check

```http
POST /skill-check
```

Executes a skill-check request.

## Usage

You can use this API documentation and Postman collection to:

* Validate Library API endpoints.
* Execute manual API tests.
* Review request and response workflows.
* Practice REST API testing with Postman.
* Document API behavior in a structured way.

## Notes

* Make sure the API base URL is correctly configured before sending requests.
* Requests that require a book ID must use a valid existing ID.
* Requests that create or update data must include the required request body.
* The Postman collection can be extended with test scripts, environment variables, and automated assertions.

## Author

**Alezander Estacio**

QA Automation Engineer
