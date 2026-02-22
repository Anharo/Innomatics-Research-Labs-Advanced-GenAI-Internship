# Python Programming Assignment – Data Processing and Analysis

## Introduction

This assignment focuses on applying Python programming concepts to real-world scenarios involving data analysis, validation, and processing. Students will use Python data structures such as dictionaries, lists, strings, and tuples to solve practical problems commonly encountered in software development, data science, and business applications.

These exercises will help strengthen logical thinking, data handling skills, and the ability to extract meaningful insights from raw data.

---

## Problem 1: Employee Performance Bonus Eligibility

### Problem Statement

A company evaluates employee performance scores at the end of the year. You are given a dictionary containing employee names and their performance scores.

### Requirements

* Identify the highest performance score.
* Handle ties if multiple employees have the same highest score.
* Display all employees eligible for the top performance bonus.

### Hint

* Use the `max()` function to find the highest score.
* Use a loop or list comprehension to find employees with that score.

### Input

```python
employees = {
    "Ravi": 92,
    "Anita": 88,
    "Kiran": 92,
    "Suresh": 85
}
```

### Expected Output

```
Top Performers Eligible for Bonus: Ravi, Kiran (Score: 92)
```

### Real-Time Applications

* HR performance evaluation systems
* Employee reward programs
* Performance-based bonus automation

---

## Problem 2: Search Query Keyword Analysis

### Problem Statement

An e-commerce website stores customer search queries. You are given a search query sentence entered by a user.

### Requirements

* Convert the input to lowercase.
* Ignore common punctuation.
* Count the frequency of each keyword.
* Display only keywords searched more than once.

### Hint

* Use `lower()` to normalize text.
* Use `replace()` or `string.punctuation` to remove punctuation.
* Use a dictionary to count frequency.

### Input

```
"Buy mobile phone buy phone online"
```

### Expected Output

```
{'buy': 2, 'phone': 2}
```

### Real-Time Applications

* Search engine optimization (SEO)
* Keyword trend analysis
* Recommendation systems

---

## Problem 3: Sensor Data Validation

### Problem Statement

A factory collects sensor readings every hour. Each reading is stored in a list where the index represents the hour and the value represents the sensor reading.

### Requirements

* Identify readings that are even numbers (valid readings).
* Store them as `(hour_index, reading_value)` pairs.
* Ignore odd readings (invalid readings).

### Hint

* Use `enumerate()` to access index and value.
* Use the modulus operator `%` to check even numbers.

### Input

```python
sensor_readings = [3, 4, 7, 8, 10, 12, 5]
```

### Expected Output

```
Valid Sensor Readings (Hour, Value):
[(1, 4), (3, 8), (4, 10), (5, 12)]
```

### Real-Time Applications

* Industrial monitoring systems
* IoT sensor validation
* Fault detection systems

---

## Problem 4: Email Domain Usage Analysis

### Problem Statement

A company wants to analyze which email providers its users are using. You are given a list of employee email IDs.

### Requirements

* Count how many users belong to each email domain.
* Calculate the percentage usage of each domain.

### Hint

* Split email using `split('@')`.
* Use a dictionary to count domains.
* Calculate percentage using `(count / total) * 100`.

### Input

```python
emails = [
    "ravi@gmail.com",
    "anita@yahoo.com",
    "kiran@gmail.com",
    "suresh@gmail.com",
    "meena@yahoo.com"
]
```

### Expected Output

```
gmail.com: 60%
yahoo.com: 40%
```

### Real-Time Applications

* User analytics
* Email service usage tracking
* Customer segmentation

---

## Problem 5: Sales Spike Detection

### Problem Statement

A retail company tracks daily sales. Sudden spikes in sales may indicate promotions or unusual activity.

### Requirements

* Calculate the average daily sales.
* Detect days where sales are more than 30% above average.
* Display the day number and sale value.

### Hint

* Use `sum()` and `len()` to calculate average.
* Compare each sale with `average * 1.3`.
* Use `enumerate()` to get day numbers.

### Input

```python
sales = [1200, 1500, 900, 2200, 1400, 3000]
```

### Expected Output

```
Day 4: 2200
Day 6: 3000
```

### Real-Time Applications

* Fraud detection
* Business analytics
* Sales performance monitoring

---

## Problem 6: Duplicate User ID Detection

### Problem Statement

A system stores user IDs during registration. Duplicate IDs can cause data integrity issues.

### Requirements

* Identify duplicate user IDs.
* Display how many times each duplicate appears.

### Hint

* Use a dictionary to count occurrences.
* Display only IDs with count greater than 1.

### Input

```python
user_ids = ["user1", "user2", "user1", "user3", "user1", "user3"]
```

### Expected Output

```
user1 → 3 times
user3 → 2 times
```

### Real-Time Applications

* Database integrity validation
* User registration systems
* Security auditing

---

## Submission Instructions

* Write Python programs for all six problems.
* Ensure code is properly formatted and commented.
* Test your programs with the given sample inputs.
* Submit the assignment as a single `.py` file or GitHub repository as instructed.

---

## Learning Outcomes

By completing this assignment, students will learn:

* Data processing using Python
* Working with dictionaries, lists, and strings
* Real-world data analysis techniques
* Logical problem solving
* Writing clean and efficient Python code

---

**End of Document**

