# British Airways Customer Review Analysis
## Objective: Analyze customer reviews to identify key drivers of passenger satisfaction and areas for improvement.
Key Insights:
•	Passenger Concerns: Frequent mentions of seating arrangements, class types, food quality, delays, and service management.
•	Recommendations: 
o	Enhance meal quality and maintain seating comfort standards across all classes.
o	Regularly review passenger feedback to address concerns proactively.
o	Minimize delays through operational efficiency and improve transparency by providing timely updates.

# Predictive Model for Understanding Buying Behavior
## Objective: Develop predictive models to identify factors influencing booking behavior and optimize revenue potential.
Key Insights:
•	Top Predictors: Purchase lead time, route, booking origin, flight hour, length of stay, and flight duration.
•	Model Performance: 
o	Gradient Boosting performed better on ROC-AUC (0.7871) but struggled with recall for completed bookings.
o	Random Forest effectively predicted non-booking events but also showed poor recall for completed bookings.
•	Challenges: 
o	Class imbalance biased predictions toward non-bookings (Class 0), reducing accuracy for completed bookings (Class 1).

# Recommendations: 
o	Target high-value routes and origins with promotions.
o	Implement early-bird discounts to encourage earlier bookings.
o	Retarget at-risk customers with personalized offers.
o	Address model imbalance with oversampling, class-weight adjustments, or ensemble techniques to improve recall.
