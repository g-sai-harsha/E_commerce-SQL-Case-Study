## E_commerce-SQL-Case-Study

#**Context:**
This business case focuses on the operations of Target in Brazil. Target is a premier U.S. retailer, focuses on delivering value, innovation, and an unmatched guest experience. This case study explores Target's e-commerce performance in Brazil, using a dataset of over 100,000 orders from 2016 to 2018, uncovering insights into:

  1. Order status & delivery time
  
  2. Payment trends & freight value
  
  3. Customer behavior & geographic distribution
  
  4. Product performance & customer satisfaction

📦 Dataset Exploration
Basic Understanding:

Identify data types of all columns in the customers table.

Determine the time range during which the orders were placed.

Count the unique cities and states from which customers placed orders.

📈 Order Trend Analysis
Growth & Seasonality:

Is there a growing trend in the number of orders placed over the years?

Can we detect monthly seasonality in order volume?

Time of Day Analysis:

Determine at what time of day Brazilian customers mostly place their orders:

00:00 - 06:00 → 🌅 Dawn

07:00 - 12:00 → 🌄 Morning

13:00 - 18:00 → 🌞 Afternoon

19:00 - 23:59 → 🌃 Night

🌍 Regional and Economic Impact
Regional Distribution:

Calculate month-over-month number of orders by state.

Visualize the distribution of customers across all Brazilian states.

Economic Flow:

Analyze money movement through:

payment_value for order cost

freight_value for shipping impact

2017–2018 Cost Increase (Jan–Aug only):

Compute % increase in total payment values between Jan–Aug 2017 and Jan–Aug 2018.

State-Level Metrics:

Calculate total & average order price by state.

Calculate total & average freight value by state.

🚚 Logistics and Delivery Performance
Delivery Timing Analysis:

Calculate:

time_to_deliver = order_delivered_customer_date - order_purchase_timestamp

diff_estimated_delivery = order_delivered_customer_date - order_estimated_delivery_date

Perform this in a single query.

Delivery Performance by State:

Top 5 states with:

⬆️ Highest average freight

⬇️ Lowest average freight

⏱️ Longest average delivery times

⚡ Fastest deliveries

📉 Most delayed deliveries (vs estimated)

💳 Payment Behavior Analysis
Payment Type Trends:

Month-over-month breakdown of orders by payment type.

Installment Usage:

Count of orders based on number of payment installments.

