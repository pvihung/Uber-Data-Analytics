# Uber-Data-Analytics
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
1. 📊**Revenue & Ride Volume**:
* Total 2024 revenue: $52M from 93M completed rides and 9M incomplete rides.
* ~40% of rides are incomplete/cancelled (46.5M) → major red flag for platform efficiency.

2. ⏰ **Demand & Timing**:
* Peak booking demand: 17:00–20:00 hrs, lowest: 00:00–04:00 hrs (in line with Uber’s known trends).
* Customers are more likely to cancel if waiting > 12.5 minutes.
* Incomplete rides often happen when driver arrival time ≈ 20 minutes.

3. 💳 **Payments & Vehicles**:
* UPI is the dominant payment method.
* No clear Vehicle preference stands out among customers.
* UberXL did not attract the customers.

4. 🚗 **Rides**:
* The average length of rides is ~25km.
* Incomplete rides were usually stopped at 10km.
* Pickup and drop-off locations show a fairly balanced distribution of bookings.
* Drivers are more likely to cancel the rides compared to customers.
  
5. 👥 **Customer Behavior**:
* No strong loyalty, since the max rides per customer in a year =3.
* High spenders (>$4K) are mostly one-time customers.

6. ⭐ **Ratings**:
* Customers tend to rate drivers more harshly, while drivers rate customers more generously.

# Business Recommendation: 
1. Reduce Driver-Initiated Cancellations:
* **Issue**: High rate of driver cancellations reduces platform efficiency and customer trust
* **Recommendation**: Have strict penalties/warning for frequent cancellations, or incentivize drivers who consistenly accept or complete rides.
* **Impact**: Decrease cancellation rate and boost Uber's revenue

2. Optimize Customer Wait Times
* **Issue**: Cancellations spike when wat time ~12.5 minutes
* **Recommendation**: Provide driver time reminders or alert to reach customer within 10 minutes, or automatically send customer message that drivers are coming as soon as posisble
* **Impact**: Reduce the cancellation rate and boost Uber's revenue

3. Review Vehicle Type
* **Issue**: UberXL shows negligible contribution to revenue
* **Recommendation**: Consider reallocate resources to higher demanding vehicles
* **Impact**: Optimize resource

4. Prevent Incomplete Ride
* **Issue**: Many customers stop around 10km
* **Recommendation**: Add an app reminder/notification (for example: 'You are half way there'), or some offers when they finish the rides (for example: 2% cash back, Uber tokens)
* **Impact**: Increase Ride Completition and boost Uber's revenue

6. Strengthen Customer Loyalty
* **Issue**: The highest number of booking by Customer was 3
* **Recommendation**: Introduce more offers for coming back customers, send notification about events might happen hours later/day later to seek customer's attention
* **Impact**: Improve customer loytalty and boost revenue
