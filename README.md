# Uber-Data-Analytics
---
## Introduction:
This project analyzes **Uber ride-sharing data (2024)** to generate actionable business insights that can help improve **revenue optimization, customer experience, and operational efficiency**. The dataset provides detailed information on bookings, cancellations, ratings, ride distances, payment methods, and more, allowing for a holistic view of Uber’s ecosystem.

### Data Schema:
- Date: Date of the booking
- Time: Time of the booking
- Booking ID: Unique identifier for each ride booking
- Booking : Status of booking (Completed, Cancelled by Customer, Cancelled by Driver, etc.)
- Customer ID: Unique identifier for customers
- Vehicle Type: Type of vehicle (Go Mini, Go Sedan, Auto, eBike/Bike, UberXL, Premier Sedan)
- Pickup Location: Starting location of the ride
- Drop Location: Destination location of the ride
- Avg VTAT: Average Vehicle Time at Arrival
- Avg CTAT: Average Customer Time at Arrival
- Cancelled Rides by Customer: Customer-initiated cancellation flag
- Reason for cancelling by Customer: Reason for customer cancellation
- Cancelled Rides by Driver: Driver-initiated cancellation flag
- Driver Cancellation Reason: Reason for driver cancellation
- Incomplete Rides: Incomplete ride flag
- Incomplete Rides Reason: Reason for incomplete rides
- Booking Value: Total fare amount for the ride
- Ride Distance: Distance covered during the ride (in km)
- Driver Ratings: Rating given to driver (1-5 scale)
- Customer Rating: Rating given by customer (1-5 scale)
- Payment Method: Method used for payment (UPI, Cash, Credit Card, Uber Wallet, Debit Card)

## Structures:
* UberAnalysis/ : Main notebooks (EDA, visualization, modeling)
* UberData/ : Raw dataset files
* Dashboard/ : Power BI dashboard showcasing key findings

## Tools & Technologies
* Language: Python
* Libraries: Pandas, Numpy, Matplotlib, Seaborn, Scikit-learn
* Visualization: Power BI, Matplotlib, Seaborn
* Analytics Approach: EDA, Data Cleaning, Statistical Analysis, Business Insights

## Analysis Highlights:
1. Revenue Analysis
- Revenue contribution by vehicle type (Go Mini, Go Sedan, UberXL, etc.)
- Revenue by payment method (UPI, Wallet, Credit/Debit Card, Cash)
- Peak revenue dates & times

2. Cancellation:
- Peak times & dates for cancellations
- Reasons for cancellations (customer vs. driver)
- Revenue lost from cancellations & incomplete rides
- Effect of VTAT & CTAT on cancellation likelihood

3. Location & Distance
- Top pickup & drop locations
- Average ride length by vehicle type
- Destinations with highest cancellation rates
  
4. Rating & Satisfaction:
- Driver vs. customer rating distribution
- Correlation of ratings with ride distance, booking value, cancellations
- Rating patterns across time of day & vehicle type

5. Customer Behavior
- Customers with highest number of cancellations
- Loyal customers & their booking patterns
- Top spenders & their contribution to total revenue

## Deliverables
* **Interactive Dashboard (Power BI)**: Visual summary of revenue, cancellations, and customer insights
* **EDA Notebook (Colab/Python)**: Detailed data cleaning, transformation, and statistical analysis
* **Key Recommendations Report**: Business insights with actionable strategies for Uber

## Key Takeaways: 
