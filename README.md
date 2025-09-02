# Dilex Food Delivery Analysis
## Induction
Dilex, a food delivery company, has seen steady sales movement but limited growth in profitability, efficiency, and overall performance. To understand why sales are not improving, they want to analyze 5 months of data and uncover insights to optimize operations, boost profitability, and enhance customer satisfaction.
##Dataset Overview 
The dataset contains 72,314 records of food delivery transactions with the following fields:
Date: The day the order was placed.
Time customer placed order: When the customer submitted their order.
Time order placed at restaurant: When the restaurant received the order.
Time driver arrived at restaurant: When the delivery driver reached the restaurant.
Delivery time: Time taken to complete the delivery.
Driver ID: Unique identifier for each driver.
Driver Name: Name of the delivery driver.
Restaurant ID: Unique identifier for each restaurant.
Customer ID: Unique identifier for each customer.
Delivery Area: The area/zone where the delivery was made.
ASAP: Whether the order was marked for immediate delivery or scheduled.
Sub Total: Cost of food items before fees, discounts, or tips.
Delivery Fee: Charge for delivery service.
Service Fee: Platform or restaurant service charge.
Discount: Any discount applied to the order.
Tip: Extra amount given by the customer to the driver.
Refunded amount: Amount returned to the customer in case of issues.
## Data Preparation
I checked the data to ensure it was clean,then turned it to table and standardized fields whose data were not well represented. I.e I changed columns storing numbers(currency) as textbook to numbers.
I created "Delivery duration column. to do this;
I merge dates inside date column with timestamps in order time and delivery time, then subtract former from latter. to get delivery time,i changed results from time and date to numbers.
## Exploratory Data Analysis
trying to understand the data better, I look at it well(dimensions and measure). They, I performed summary statistics to understand it greatly. The results are:
Total Orders: 72314
ASAP Orders: 57742
Scheduled Orders: 14572
Mean Delivery Time (min): 33.95
Median Delivery Time (min): 60.72
Mode Delivery Time (min): 47.54
SD Delivery Time (min): 252.96
Skewness: 3.68
Kurtosis: 12.60
Max Delivery Time (min): 1399.68
ASAP Mean (min): 128.22
ASAP Median (min): 58.28
ASAP Mode (min): 53.42
ASAP SD (min): 247.93
ASAP Max (min): 1399.68
Scheduled Mean (min): 156.66
Scheduled Median (min): 71.37
Scheduled Mode (min): 51.59
Scheduled SD (min): 270.78
Scheduled Max (min): 1398.87
  I then prepared pre- Analysis questions, as listed below:
- How is revenue trend (by week)
- When are Orders placed? (time cycle like mornings,..., weekday)
- Revenue by area and day type
- avg delivery by day of week(acrothe week)
- tip by day of week
- order completion rate
- driver efficiency.




