# FastAPI Assignment – 3

## Overview

This project demonstrates the creation of REST API endpoints using **FastAPI**. The assignment focuses on defining routes, handling requests, and returning structured responses using Python.

The application exposes multiple endpoints that can be tested through **Swagger UI**, which FastAPI automatically provides for API testing and documentation.

## Technologies Used

* Python
* FastAPI
* Uvicorn

## Key Concepts Practiced

* Creating API endpoints using FastAPI
* Handling HTTP requests and responses
* Using path and query parameters
* Returning JSON responses
* Testing endpoints using Swagger UI

## How to Run the Project

1. Install dependencies

```
pip install fastapi uvicorn
```

2. Run the FastAPI server

```
uvicorn main:app --reload
```

3. Open the browser and go to:

Swagger Documentation:

```
http://127.0.0.1:8000/docs
```

## Project Structure

```
project-folder
│
├── main.py
└── README.md
```

## Learning Outcome

Through this assignment, I learned how to build and test APIs using FastAPI, understand routing, and work with automatic documentation provided by Swagger UI.
