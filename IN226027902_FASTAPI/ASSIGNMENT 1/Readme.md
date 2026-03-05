### FastAPI Assignment – Endpoint Creation and Testing

In this assignment, I learned how to create API endpoints using **FastAPI** and tested them using the built-in **Swagger UI**.

I implemented multiple endpoints in the `main.py` file to manage product-related data. The API returns structured JSON responses and demonstrates how to handle requests, responses, and basic data structures in FastAPI.

#### Key Concepts Practiced

* Creating API endpoints using FastAPI
* Structuring product data using Python dictionaries and lists
* Returning JSON responses from endpoints
* Testing endpoints using Swagger UI (`/docs`)
* Understanding how REST APIs work in a simple product management example

#### Implementation

All the endpoints were implemented inside the `main.py` file. The API includes a products list containing details such as:

* `id`
* `name`
* `price`
* `category`
* `in_stock`

Additional products were added to demonstrate how APIs dynamically return updated data.

#### Testing

All endpoints were successfully tested using **Swagger UI** available at:

`http://127.0.0.1:8000/docs`

Swagger provides an interactive interface where each endpoint can be executed directly from the browser to verify the API responses.

#### Repository Contents

* `main.py` – Contains the FastAPI application and endpoints
* Assignment screenshots – Demonstrating endpoint execution and responses
* API testing via Swagger UI

This assignment helped me understand the fundamentals of building and testing APIs using FastAPI, which is an essential skill for modern backend and AI-powered applications.
