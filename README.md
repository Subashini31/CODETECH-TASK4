# Linear Programming for Car Sales Optimization

This notebook demonstrates how Linear Programming (LP) can be applied to optimize car sales and maximize profit for an automotive dealership. We'll use the PuLP library to model and solve this optimization problem. 

#### Business Problem:
Given a dataset of car sales, we want to maximize the profit by optimizing the number of cars sold for each model, while adhering to certain constraints like inventory limits and regional demand.

#### Objective:
- Maximize the profit from car sales.
- Identify which car models should be prioritized to maximize profit.

---

### **2. Dataset Exploration**
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

# Problem Setup

The goal is to maximize the total profit by selecting the optimal number of cars to sell from each model, while adhering to certain constraints.

#### Objective Function:
We aim to maximize the total profit, which can be calculated as:

\[
\text{Total Profit} = \sum_{i=1}^{n} (\text{Profit}_i \times \text{Sales Quantity}_i)
\]

Where:
- `Profit_i` is the profit for car model \(i\) (calculated as `Price - Cost`).
- `Sales Quantity_i` is the number of units of car model \(i\) sold.

#### Constraints:
1. **Inventory Limits**: Each region has a limit on how many cars can be sold based on inventory.
2. **Non-Negativity**: The number of cars sold for each model must be non-negative.

---

### **4. Linear Programming Implementation**

# Linear Programming Model Implementation

We will now set up the LP problem using the PuLP library. The goal is to maximize profit while considering the constraints.

#### Steps:
1. **Define Decision Variables**: The number of cars to be sold for each model.
2. **Set Objective Function**: Maximize the total profit.
3. **Define Constraints**: Ensure sales don't exceed regional inventory limits.

We'll solve the LP problem and display the optimal solution.

