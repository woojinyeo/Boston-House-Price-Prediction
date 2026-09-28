# FoodHub Order Analysis

## Project Overview

This project analyzes customer order data from FoodHub, an online food delivery platform that connects customers with restaurants in New York.

The objective of the analysis was to understand restaurant demand, customer ordering behavior, delivery performance, and customer ratings. The findings were used to identify opportunities for improving the customer experience and overall business performance.

The project demonstrates exploratory data analysis, data visualization, and business insight generation using Python.

## Dataset

The dataset contains 1,898 food orders and 9 variables.

The variables include:

- `order_id` – Unique identifier for each order
- `customer_id` – Unique identifier for each customer
- `restaurant_name` – Restaurant from which the order was placed
- `cuisine_type` – Type of cuisine ordered
- `cost_of_the_order` – Cost of the order
- `day_of_the_week` – Whether the order was placed on a weekday or weekend
- `rating` – Customer rating of the order
- `food_preparation_time` – Time taken by the restaurant to prepare the food
- `delivery_time` – Time taken to deliver the order to the customer

## Data Exploration and Preparation

The dataset was examined to understand its structure and ensure it was suitable for analysis.

Key steps included:

- Examined the shape and structure of the dataset
- Reviewed column data types
- Checked for missing values
- Generated descriptive statistics for numerical variables
- Examined order costs, ratings, preparation times, and delivery times
- Analyzed categorical variables such as restaurant, cuisine type, and day of the week
- Used univariate and multivariate visualizations to identify patterns and relationships

No missing values were identified in the dataset.

## Exploratory Data Analysis

The analysis investigated several areas of FoodHub's business, including:

- Most frequently ordered restaurants
- Most popular cuisine types
- Customer ordering frequency
- Distribution of order costs
- Customer rating patterns
- Food preparation times
- Delivery times
- Differences between weekday and weekend orders
- Relationships between ratings, cost, preparation time, and delivery time

## Key Findings

### Restaurant Demand

The five restaurants receiving the highest number of orders were:

1. Shake Shack
2. The Meatball Shop
3. Blue Ribbon Sushi
4. Blue Ribbon Fried Chicken
5. Parm

Shake Shack received the highest number of orders in the dataset.

### Cuisine Preferences

American cuisine was the most frequently ordered cuisine and was also the most popular cuisine on weekends.

Japanese, Italian, and Chinese cuisine were also among the most frequently ordered cuisine types.

### Order Costs

Approximately **29.24% of orders cost more than $20**.

The average order cost was approximately **$16.50**.

### Customer Ratings

A significant portion of orders did not receive customer ratings:

- 588 orders received a rating of 5
- 386 orders received a rating of 4
- 188 orders received a rating of 3
- 736 orders were not rated

The large number of unrated orders indicates an opportunity to encourage additional customer feedback.

### Delivery Performance

The average delivery time across all orders was approximately **24.16 minutes**.

Delivery performance differed considerably between weekdays and weekends:

- **Weekday average:** approximately 28.34 minutes
- **Weekend average:** approximately 22.47 minutes

Despite having fewer orders, weekday deliveries took longer on average.

Approximately **10.54% of orders required more than 60 minutes** from preparation through delivery.

### Restaurant Promotion Analysis

Restaurants with more than 50 ratings and an average rating above 4 were identified as candidates for promotional opportunities:

- Blue Ribbon Fried Chicken
- Blue Ribbon Sushi
- Shake Shack
- The Meatball Shop

### Revenue Analysis

Using FoodHub's commission structure for qualifying orders, the estimated revenue generated from the orders in the dataset was approximately **$6,166.30**.

## Business Recommendations

Based on the analysis:

- Investigate the causes of longer weekday delivery times and consider adjusting driver availability or delivery coverage during weekdays.
- Encourage customers to leave ratings through incentives such as reward points or promotional offers to improve the amount of customer feedback available for analysis.
- Monitor restaurants with lower ratings and investigate whether inconsistent food preparation or delivery times are affecting customer satisfaction.
- Investigate preparation-time outliers among Korean cuisine restaurants to determine the operational causes of unusually long preparation times.
- Continue leveraging highly rated and frequently ordered restaurants in promotional campaigns.

## Visualizations

The project uses several visualizations to explore customer behavior and operational performance, including:

- Histograms
- Box plots
- Count plots
- Cuisine comparisons
- Rating comparisons
- Weekday vs. weekend delivery-time comparisons
- Correlation heatmap

### Featured Analysis

![Visualization 1](images/visualization1.png)

![Visualization 2](images/visualization2.png)

![Visualization 3](images/visualization3.png)

## Tools and Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data inspection and validation
- Descriptive statistics
- Data visualization
- Univariate analysis
- Multivariate analysis
- Customer behavior analysis
- Operational performance analysis
- Business insight generation
- Translating analytical findings into recommendations

## Project Files

- FoodHub analysis notebook – Complete Python analysis
- `foodhub_order.csv` – Dataset used for the analysis
- `README.md` – Project documentation
- `images/` – Selected project visualizations
