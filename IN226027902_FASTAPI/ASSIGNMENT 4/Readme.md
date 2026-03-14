## FastAPI Day 5 – Cart System API

In this assignment, I practiced building a **complete cart system backend using FastAPI**. The tasks focused on implementing multiple endpoints that work together to simulate a real **shopping cart workflow**.

The assignment demonstrates how APIs interact to support operations such as **adding products to a cart, viewing cart items, handling stock validation, updating quantities, removing products, and completing checkout**.

### Key Concepts Practiced

* Building **POST endpoints** to add items to a cart
* Creating **GET endpoints** to view cart contents
* Implementing **DELETE endpoints** to remove products
* Handling **error responses** such as out-of-stock products or invalid product IDs
* Updating existing cart items instead of creating duplicates
* Processing **checkout logic** and generating orders
* Returning structured **JSON responses**
* Testing APIs using **Swagger UI**

### Implementation

All endpoints were implemented in the `main.py` file and work together to simulate a basic **e-commerce cart system**.

The API manages several data structures including:

* **Products list** – Contains product details such as:

  * `product_id`
  * `name`
  * `price`
  * `in_stock`

* **Cart list** – Stores items added by the customer

* **Orders list** – Stores completed checkout orders

### Features Implemented

Several endpoints were created to support the full shopping cart flow:

* **Add to Cart Endpoint** – Allows users to add products to the cart with quantity and calculates subtotal automatically.

* **View Cart Endpoint** – Displays all items currently in the cart along with item count and grand total.

* **Stock Validation** – Prevents adding products that are out of stock and returns appropriate error responses.

* **Cart Update Logic** – If a product already exists in the cart, its quantity is updated instead of creating duplicate entries.

* **Remove Item Endpoint** – Allows users to delete a specific product from the cart.

* **Checkout Endpoint** – Processes the cart items, generates order entries, calculates totals, and clears the cart after checkout.

* **Orders Endpoint** – Returns all placed orders along with the total number of orders.

### Testing

All endpoints were tested using **Swagger UI**, which FastAPI automatically generates.

Swagger documentation can be accessed at:

```
http://127.0.0.1:8000/docs
```

Using Swagger UI, requests were executed directly from the browser to verify:

* Cart item additions
* Quantity updates
* Stock validation errors
* Cart totals and item counts
* Checkout operations
* Orders generated after checkout

Screenshots of these API responses were captured as part of the assignment submission.

### Repository Contents

* `main.py` – Contains the FastAPI cart system implementation
* Assignment screenshots – Showing API requests and responses
* Swagger UI test outputs

### Learning Outcome

This assignment helped strengthen my understanding of **designing interconnected REST API endpoints using FastAPI**. It also demonstrated how backend services manage application state such as cart items, product availability, and order creation.

Through this exercise, I gained practical experience implementing **business logic, error handling, and API workflows similar to real e-commerce backend systems**.

These skills are essential for building **scalable backend services and modern web applications that rely heavily on APIs**.
