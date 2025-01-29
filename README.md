# Linear Programming for Car Sales Optimization

This notebook demonstrates how Linear Programming (LP) can be applied to optimize car sales and maximize profit for an automotive dealership. We'll use the PuLP library to model and solve this optimization problem. 

#### Business Problem:
Given a dataset of car sales, we want to maximize the profit by optimizing the number of cars sold for each model, while adhering to certain constraints like inventory limits and regional demand.

#### Objective:
- Maximize the profit from car sales.
- Identify which car models should be prioritized to maximize profit.

---

### **2. Dataset Exploration**

```markdown
# Dataset Overview

Let's first load the dataset and explore the data to understand its structure and key features.

### Data Columns:
- `Car_id`: Unique identifier for each car sale.
- `Date`: Date of sale transaction.
- `Customer Name`: Name of the customer.
- `Gender`: Gender of the customer.
- `Annual Income`: Annual income of the customer.
- `Dealer_Name`: Name of the car dealer.
- `Company`: Car manufacturer.
- `Model`: Model of the car sold.
- `Engine`: Type of engine in the car.
- `Transmission`: Transmission type.
- `Color`: Color of the car.
- `Price ($)`: Sale price of the car.
- `Dealer_No`: Dealer identification number.
- `Body Style`: Type of car (SUV, Hatchback, etc.).
- `Phone`: Customer phone number.
- `Dealer_Region`: Region of the dealer.

We will inspect the first few rows of the dataset to understand its structure and decide how to model the problem.
