# 📘 Assignment: Building REST APIs with FastAPI

## 🎯 Objective

Build a small REST API with FastAPI that manages a list of books. You will create endpoints for each HTTP method, validate request data with Pydantic models, and return the correct status codes and error responses.

## 📝 Tasks

### 🛠️ Create Your First Endpoint

#### Description
Install FastAPI and Uvicorn, create a FastAPI application, and add a `GET /` endpoint that returns a welcome message. Start the server and open the interactive docs at `/docs` to confirm your endpoint works.

Install the packages with:

```bash
pip install fastapi uvicorn
```

Run your app with:

```bash
uvicorn main:app --reload
```

#### Requirements
Completed program should:

- Create a FastAPI app object named `app` in a file named `main.py`.
- Define a `GET /` endpoint that returns JSON with a `message` key, for example `{"message": "Welcome to the Book API"}`.
- Start the server with Uvicorn and confirm the endpoint works in a browser or at `/docs`.


### 🛠️ Build Book Routes

#### Description
Store books in a Python list of dictionaries. Add routes that let a client list all books, get one book by its ID, and add a new book.

Each book should have an `id`, a `title`, an `author`, and a `year`.

#### Requirements
Completed program should:

- Include a `GET /books` endpoint that returns all books in the list.
- Include a `GET /books/{book_id}` endpoint that returns the book with the matching `id`.
- Include a `POST /books` endpoint that adds a new book to the list and returns it with status code `201`.
- Assign a new, unique `id` to each book you add.

Example request body for `POST /books`:

```json
{
  "title": "Dune",
  "author": "Frank Herbert",
  "year": 1965
}
```


### 🛠️ Validate Data and Handle Errors

#### Description
Use Pydantic models to describe the data your API accepts and returns. Return a clear error when a client asks for a book that does not exist.

#### Requirements
Completed program should:

- Define a Pydantic `BookCreate` model with `title` (string), `author` (string), and `year` (integer) fields used for `POST /books` requests.
- Define a `Book` model that adds the `id` field and is used for responses.
- Return status code `404` with a helpful message when `GET /books/{book_id}` is called with an ID that does not exist.
- Return status code `422` automatically when a `POST /books` request is missing a field or has a `year` that is not an integer. Confirm this in the `/docs` page.
