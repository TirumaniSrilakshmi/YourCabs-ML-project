YourCabs
YourCabs Capstone project

The business problem tackled here is trying to improve customer service for YourCabs.com, a cab company in Bangalore. The problem of interest is booking cancellations by the company due to unavailability of a car. The challenge is that cancellations can occur very close to the trip start time,thereby causing passengers inconvenience.

Objective
The goal of the competition is to create a predictive model for classifying new bookings as to whether they will eventually gets cancelled due to car unavailability

Number of columns :
id - booking ID
user_id - the ID of the customer (based on mobile number)
vehicle_model_id - vehicle model type.
package_id - type of package (1=4hrs & 40kms, 2=8hrs & 80kms, 3=6hrs & 60kms, 4= 10hrs & 100kms, 5=5hrs & 50kms, 6=3hrs & 30kms, 7=12hrs & 120kms)
travel_type_id - type of travel (1=long distance, 2= point to point, 3= hourly rental).
from_area_id - unique identifier of area. Applicable only for point-to-point travel and packages
to_area_id - unique identifier of area. Applicable only for point-to-point travel
from_city_id - unique identifier of city
to_city_id - unique identifier of city (only for intercity)
from_date - time stamp of requested trip start
online_booking - if booking was done on desktop website
mobile_site_booking - if booking was done on mobile website
booking_created - time stamp of booking
from_lat - latitude of from area
from_long - longitude of from area
to_lat - latitude of to area
to_long - longitude of to area
Car_Cancellation - whether the booking was cancelled (1) or not (0) due to unavailability of a car
Solution
In this project, EDA analysis for entire dataset is performed and 3 different datasets are categorized based on travel_type_id as different traveltypeid's have unique flows. As its a classification analysis, revelant classification algorithms mentioned below are applied on datasets and finak prediction is made based on model with high accuracy and good precision and recall scores.

Classification algorithms -
Logistic Regression
Decision Tree
Random Forest Classifier
AdaBoost Classifier
GradientBoost Classifier
SVM
Naive Bayes
KNN
As input 3 datasets are used, and each dataset are trained for 8 classification models therefore, for 1 dataset 24 models , and for 3 datasets 72 models (total) Finally commiting for 3 final models for each dataset
