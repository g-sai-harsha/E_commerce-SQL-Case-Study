### E_commerce-SQL-Case-Study

# **Context:**
This business case focuses on the operations of Target in Brazil. Target is a premier U.S. retailer, focuses on delivering value, innovation, and an unmatched guest experience. This case study explores Target's e-commerce performance in Brazil, using a dataset of over 100,000 orders from 2016 to 2018, uncovering insights into:

  1. Order status & delivery time
  2. Payment trends & freight value
  3. Customer behavior & geographic distribution
  4. Product performance & customer satisfaction

## **Problem Statement:**
    Our objective is to analyze the provided dataset to uncover meaningful insights and deliver actionable 
    business recommendations. 
    The following steps outline the approach used to extract meaningful insights from the     
    dataset:
  **Usual exploratory analysis steps:**
        1. Data type of all columns in the "customers" table.
        2. Get the time range between which the orders were placed.
        3. Count the Cities & States of customers who ordered during the given period.
    **In-depth Exploration:**
        1. Is there a growing trend in the no. of orders placed over the past years?
        2. Can we see some kind of monthly seasonality in terms of the no. of orders being placed?
        3. During what time of the day, do the Brazilian customers mostly place their orders? (Dawn, Morning,     
           Afternoon or Night)
                0-6 hrs : Dawn
                7-12 hrs : Mornings
                13-18 hrs : Afternoon
                19-23 hrs : Night
    **Evolution of E-commerce orders in the Brazil region:**
        1. Get the month on month no. of orders placed in each state.
        2. How are the customers distributed across all the states?
    **Impact on Economy: Analyze the money movement by e-commerce by looking at order prices, freight and 
      others.**
        1. Get the % increase in the cost of orders from year 2017 to 2018 (include months between Jan to Aug   
           only).
           You can use the "payment_value" column in the payments table to get the cost of orders.
        2. Calculate the Total & Average value of order price for each state.
        3. Calculate the Total & Average value of order freight for each state.
    **Analysis based on sales, freight and delivery time.**
        1. Find the no. of days taken to deliver each order from the order’s purchase date as delivery time.
           Also, calculate the difference (in days) between the estimated & actual delivery date of an order.
           Do this in a single query.
    
          (You can calculate the delivery time and the difference between the estimated & actual delivery date 
          using the given formula:
               a. time_to_deliver = order_delivered_customer_date - order_purchase_timestamp
               b.  diff_estimated_delivery = order_delivered_customer_date - order_estimated_delivery_date)
        2. Find out the top 5 states with the highest & lowest average freight value.
        3. Find out the top 5 states with the highest & lowest average delivery time.
        4. Find out the top 5 states where the order delivery is really fast as compared to the estimated date 
           of delivery.
           (You can use the difference between the averages of actual & estimated delivery date to figure out 
           how fast the delivery was for each state.)
  **Analysis based on the payments:**
        1. Find the month on month no. of orders placed using different payment types.
        2. Find the no. of orders placed on the basis of the payment installments that have been paid.
# **Tools and Databases used:**
    Google BigQuery
# **Insights and Business Recommendations Summary:**
  1. **Expand Logistics Infrastructure in Remote States:**
       States like RR, AC, and PB experience high freight costs and long delivery times.
       Investing in local warehouses or distribution hubs can reduce shipping costs and improve
       customer satisfaction.
  2. **Leverage SP as a Strategic Fulfillment Hub:**
       SP has high order density and the lowest average freight costs. Enhancing warehousing
       and fulfillment capabilities in this region can optimize nationwide logistics.
  3. **Optimize Delivery Promises Using Data:**
       States like AL consistently deliver ahead of estimated dates. Update estimated delivery
       algorithms to reflect actual performance for improved transparency and trust.
  4. **Incentivize High-Value Regions with Targeted Promotions:**
       States with high average order prices but fewer customers (e.g., PB, AL, AC) show
       potential for premium product targeting and personalized marketing strategies.
  5. **Promote Afternoon Deals or Campaigns:**
       Since the peak ordering window is in the afternoon, scheduling flash sales or marketing
       pushes during this time can capitalize on user behavior.
  6.** Encourage Full Upfront Payments:**
       Over 52,000 customers prefer one-time payments. Reinforcing this behavior with small
       incentives (e.g., cashback for full payment) can reduce transaction processing costs.
  7. **Monitor and Enhance UPI Adoption:**
       UPI usage is rising steadily. Ensure seamless UPI integration and provide incentives for
       its use to align with Brazil’s digital payment evolution.
