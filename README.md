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
- Total Orders: 72,314
- ASAP Orders: 57,742
- Scheduled Orders: 14,572.

Delivery Times (Minutes):
- Overall: Mean = 133.95 | Median = 60.72 | Mode = 47.54 | SD = 252.96 | Max = 1399.68
- ASAP Orders: Mean = 128.22 | Median = 58.28 | Mode = 53.42 | SD = 247.93 | Max = 1399.68
- Scheduled Orders: Mean = 156.66 | Median = 71.37 | Mode = 51.59 | SD = 270.78 | Max = 1398.87.

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
## Insights
1.	Revenue showed a steady upward trend from January to April, peaking in Week 17, closely followed by Week 16. The lowest revenue was recorded in Week 1, followed by Week 3, with Week 18 also ranking among the lowest four. This indicates consistent growth over the four-month period despite occasional dips
2.	Performance across the three similar. Revenue is $2.59M in Union City, $2.60M in Fremont, and $2.62M in Hayward, indicating no significant variation across locations.
3.	Order patterns show clear peaks in the mornings, accounting for 80% of all orders, followed by evenings (9%) and nights (8%). Across days, Wednesday records the highest orders, followed by Saturday, while Friday sees the lowest activity.
4.	Average delivery time is 134 minutes (≈2h 14m). Delivery was fastest in January (68 mins), worsened steadily to March (165 mins), but improved in April (143 mins). Across weekdays, Fridays (140 mins) and Mondays (139 mins) face the longest delays, while Wednesdays record the fastest deliveries (122 mins).


