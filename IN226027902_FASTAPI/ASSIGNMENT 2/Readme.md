## FastAPI Day 2 – Advanced Endpoint Practice

In this assignment, I practiced building more advanced API endpoints using **FastAPI**. The tasks focused on combining multiple backend concepts such as **query parameters, path parameters, POST requests, Pydantic validation, and business logic**.

The assignment simulates a small **product management backend** where users can filter products, retrieve specific information, submit feedback, generate product analytics, and place bulk orders.

### Key Concepts Practiced

* Creating **GET endpoints** with path parameters
* Using **query parameters** for filtering data
* Building **POST endpoints** for submitting data
* Validating request bodies using **Pydantic models**
* Implementing **business logic** inside API routes
* Returning structured **JSON responses**
* Testing endpoints using **Swagger UI**

### Implementation

All endpoints were implemented inside the `main.py` file. The API works with a products list containing details such as:

* `id`
* `name`
* `price`
* `category`
* `in_stock`

Several new endpoints were added to extend the functionality of the API:

* **Product Filtering Endpoint** – Allows filtering products using parameters like `min_price`, `max_price`, and `category`.
* **Product Price Endpoint** – Returns only the `name` and `price` of a product using its `product_id`.
* **Customer Feedback Endpoint** – Accepts validated feedback using a Pydantic model and stores it in a feedback list.
* **Product Summary Endpoint** – Generates statistics about products such as total products, stock counts, cheapest product, most expensive product, and available categories.
* **Bulk Order Endpoint** – Accepts multiple order items, validates them, checks stock availability, calculates totals, and returns confirmed and failed items.

### Testing

All endpoints were tested using **Swagger UI**, which FastAPI automatically provides.

Swagger documentation can be accessed at:

```
http://127.0.0.1:8000/docs
```

The interactive interface allows sending requests directly from the browser and verifying JSON responses returned by the API.

### Repository Contents

* `main.py` – Contains the FastAPI application and all implemented endpoints
* Assignment screenshots – Showing endpoint execution and responses
* Swagger UI testing results

### Learning Outcome

This assignment strengthened my understanding of building **structured and validated REST APIs using FastAPI**. It also helped me practice implementing backend logic such as filtering data, validating requests, handling errors, and processing bulk operations.

These skills are essential for building scalable backend systems and **AI-powered applications that rely on APIs**.
