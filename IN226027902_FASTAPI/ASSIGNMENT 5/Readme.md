# FastAPI Day 6 – Search, Sort, and Pagination

## Overview

This assignment focuses on implementing three essential features commonly used in real-world APIs: **search**, **sorting**, and **pagination**. These capabilities allow users to efficiently explore large datasets by filtering results, organizing them in a specific order, and navigating them in smaller pages.

The project builds on the previous FastAPI exercises and expands the product management API by adding endpoints that simulate how real e-commerce platforms manage product browsing and order management.

## Features Implemented

### Product Search

Implemented a search endpoint that allows users to find products by providing a keyword. The search is **case-insensitive** and returns all products whose names contain the given keyword.

**Endpoint**

```
GET /products/search?keyword=<text>
```

**Example**

```
GET /products/search?keyword=mouse
```

Returns matching products along with the total number of results.

---

### Product Sorting

Implemented sorting functionality that allows products to be sorted based on specific fields.

Supported sorting options:

* Sort by **price** (ascending or descending)
* Sort by **name** (alphabetical order)

**Endpoint**

```
GET /products/sort?sort_by=<field>&order=<asc|desc>
```

**Example**

```
GET /products/sort?sort_by=price&order=asc
```

Default values:

* `sort_by = price`
* `order = asc`

Invalid sorting fields are handled with proper error responses.

---

### Product Pagination

Pagination allows users to retrieve products in smaller sets instead of receiving the entire dataset at once.

**Endpoint**

```
GET /products/page?page=<number>&limit=<items_per_page>
```

**Example**

```
GET /products/page?page=1&limit=2
```

The response includes:

* Current page
* Number of items per page
* Total number of pages
* Products for that page

---

### Order Search

Added functionality to search orders by customer name. This helps administrators quickly locate orders associated with a specific customer.

**Endpoint**

```
GET /orders/search?customer_name=<name>
```

The search is case-insensitive and returns all matching orders.

---

### Sort Products by Category and Price

Created an endpoint that organizes products by **category first** and then sorts them by **price within each category**.

**Endpoint**

```
GET /products/sort-by-category
```

This produces grouped results such as:

* Electronics → sorted by price
* Stationery → sorted by price

---

### Combined Browse Endpoint

Built a powerful endpoint that combines **search, sorting, and pagination in a single request**.

**Endpoint**

```
GET /products/browse
```

Supported optional parameters:

* `keyword` – search filter
* `sort_by` – sorting field
* `order` – sorting direction
* `page` – page number
* `limit` – number of items per page

Processing order:

1. Filter products using the search keyword
2. Sort the filtered results
3. Apply pagination to the sorted results

This mimics how real online shopping APIs work.

---

## Technologies Used

* **Python**
* **FastAPI**
* **Pydantic**
* **Swagger UI** for API testing

---

## Running the Project

1. Rename the main file if required:

```
main_day6.py → main.py
```

2. Start the server:

```
uvicorn main:app --reload
```

3. Open Swagger documentation in your browser:

```
http://127.0.0.1:8000/docs
```

From here you can test all endpoints interactively.

---

## Learning Outcomes

Through this assignment, I learned how to:

* Implement **search functionality** in APIs
* Apply **sorting algorithms** to API responses
* Build **pagination systems** for large datasets
* Combine multiple query features into a single endpoint
* Design APIs that resemble **real production systems**

These concepts are critical for building scalable backend systems used in modern web applications and data-driven pla
