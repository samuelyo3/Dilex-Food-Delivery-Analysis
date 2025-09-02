# Dilex Food Delivery Analysis
## Induction
Dilex, a food delivery company, has experienced steady sales growth but limited improvements in profitability, efficiency, and overall performance. To understand these challenges, the company commissioned an analysis of 5 months of delivery data. The goal is to uncover insights that can optimize operations, enhance customer satisfaction, and improve profitability.
## Dataset Overview 
The dataset contains 72,314 records of food delivery transactions with the following fields:
- Date: The day the order was placed.
- Time customer placed order: When the customer submitted their order.
- Time order placed at restaurant: When the restaurant received the order.
-Time driver arrived at restaurant: When the delivery driver reached the restaurant.
- Delivery time: Time taken to complete the delivery.
- Driver ID: Unique identifier for each driver.
- Driver Name: Name of the delivery driver.
- Restaurant ID: Unique identifier for each restaurant.
- Customer ID: Unique identifier for each customer.
- Delivery Area: The area/zone where the delivery was made.
- ASAP: Whether the order was marked for immediate delivery or scheduled.
- Sub Total: Cost of food items before fees, discounts, or tips.
- Delivery Fee: Charge for delivery service.
- Service Fee: Platform or restaurant service charge.
- Discount: Any discount applied to the order.
- Tip: Extra amount given by the customer to the driver.
- Refunded amount: Amount returned to the customer in case of issues.
## Data Preparation
- Checked the dataset for consistency and cleaned irregularities.
- Converted relevant fields (e.g., currency values) from text to numeric formats.
- Created a new Delivery Duration field by merging date and time columns, then subtracting order time from delivery completion time.
Converted the resulting values into minutes for easier analysis.
## Exploratory Data Analysis
To better understand the data, I explored both dimensions and measures using summary statistics.
Key Summary Statistics:

● Total Orders: 72,314
● ASAP Orders: 57,742
● Scheduled Orders: 14,572.
Delivery Times (Minutes):
● Overall: Mean = 133.95 | Median = 60.72 | Mode = 47.54 | SD = 252.96 | Max = 1399.68
● ASAP Orders: Mean = 128.22 | Median = 58.28 | Mode = 53.42 | SD = 247.93 | Max = 1399.68
● Scheduled Orders: Mean = 156.66 | Median = 71.37 | Mode = 51.59 | SD = 270.78 | Max = 1398.87.

Skewness: 3.68 (positively skewed)
Kurtosis: 12.60 (heavy-tailed distribution)
### Pre-Analysis Questions
To guide the analysis, the following questions were prepared:
- How is revenue trending over time (by week)?
- When are orders placed (time cycle: mornings, afternoons, evenings)?
- How does revenue vary by area and by day type (weekday vs weekend)?
- What is the average delivery time across days of the week?
- How do tips vary across days of the week?
- What is the order completion rate (delivered vs refunded)?
- How efficient are drivers in completing deliveries?



