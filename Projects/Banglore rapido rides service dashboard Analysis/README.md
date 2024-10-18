# Banglore rapido rides service dashboard Analysis

### Dashboard Link : [Dashboard]([https://app.powerbi.com/groups/me/reports/384d017e-e935-44dc-9e7d-1626c1a36de1/ReportSection](https://app.powerbi.com/reportEmbed?reportId=cb79784e-cf72-4064-8b0a-c1c6fed4cfc6&autoAuth=true&embeddedDemo=true))

<iframe title="rapido" width="1140" height="541.25" src="https://app.powerbi.com/reportEmbed?reportId=cb79784e-cf72-4064-8b0a-c1c6fed4cfc6&autoAuth=true&embeddedDemo=true" frameborder="0" allowFullScreen="true"></iframe>

## Problem Statement

Objective: To analyze and understand the transportation patterns, pricing dynamics, and user behavior related to various Rapido ride services in Bangalore. The aim is to identify key trends in service utilization, factors influencing ride cancellations, and fare structures across different service types, helping stakeholders make data-driven decisions to optimize operations and improve user satisfaction.

## Key Questions:

# Service Utilization Analysis:

1. What are the most and least popular Rapido services in Bangalore?
2. How does the distribution of ride types (bike, bike lite, cab economy, auto, parcel) vary across different areas of Bangalore?
   
# Pricing and Ride Economics:
1. What is the average ride duration and distance covered for each service type?
2. How do the base fares and additional charges vary across different services?
3. What factors impact the total fare, and how do they differ for each ride type?
   
Ride Cancellations:
1. What is the percentage of ride cancellations for each service type?
2. Are there specific times of day or locations where ride cancellations are more frequent?
3. What trends can be identified that might help reduce ride cancellations?
   
# Payment Method Preferences:
1. What are the most commonly used payment methods for completed rides?
2. How does the choice of payment method vary between different types of services?
3. Are there any correlations between payment methods and the likelihood of ride completion or cancellation?
   
# Expected Outcomes:
Insights into the demand for various Rapido services and opportunities to enhance service offerings.
A clear understanding of the pricing structures and factors influencing total fares.
Recommendations for reducing ride cancellations and improving the user experience.
Analysis of payment trends to help Rapido streamline payment processes and cater to user preferences.
This problem statement aims to leverage the dataset to generate actionable insights that can support Rapido's strategic decisions in Bangalore's competitive ride-hailing market.


## About Dataset
Dataset Title
Bangalore Rapido Ride Services Dataset [Dataset Link](https://www.kaggle.com/datasets/vishaldeoprasad/bangalore-rapido-ride-services-dataset)


# Subtitle
A Comprehensive Analysis of Ride Services in Bangalore

# Overview
This dataset contains comprehensive records of ride services offered by Rapido in Bangalore over a two-month period. It includes various service types such as bike, bike lite, cab economy, auto, and parcel services. Each record provides extensive details about the ride, including the journey from a source to a destination, duration, distance, charges, and payment methods. This dataset is ideal for analyzing transportation patterns, service utilization, and ride economics in Bangalore.

# Dataset Structure
The dataset is organized in a tabular format with 50,000 rows and 13 columns. Each row represents a unique ride, and the columns provide detailed information about each ride.

# Column Descriptions
services
           Description: Type of ride service offered by Rapido.
           Values:
           "bike": Standard bike ride service.
           "bike lite": Economical bike ride service.
           "cab economy": Standard cab ride service.
           "auto": Auto-rickshaw ride service.
           "parcel": Service for delivering parcels.
           Distribution:
           30% bike
           10% bike lite
           20% cab economy
           25% auto
           15% parcel
           
date
           Description: The date on which the ride was initiated.
           Values: Dates ranging from 60 days prior to the current date, covering approximately two months.
time
           Description: The time of day when the ride started.
           Values: Random times throughout the day, formatted as HH:MM:SS.
ride_status

           Description: The completion status of the ride.
Values:
           "completed": The ride was successfully completed.
           "cancelled": The ride was cancelled.
           Distribution:
           90% completed
           10% cancelled
source
           Description: The starting location of the ride.
           Values: Combinations of common Bangalore area names and suffixes (e.g., "Koramangala 1st Stage").
destination
           Description: The ending location of the ride.
           Values: Combinations of common Bangalore area names and suffixes, similar to the source.
duration
           Description: Duration of the ride in minutes.
           Values: Integer values ranging from 10 to 120 minutes.
ride_id
           Description: A unique identifier for each ride.
           Values: A string starting with "RD" followed by 16 random digits (e.g., "RD1234567890123456").
distance
           Description: The distance covered during the ride, in kilometers.
           Values: Floating-point numbers ranging from 1 to 50, rounded to two decimal places.
ride_charge
           Description: The base fare charged for the ride.
           Values: Floating-point numbers ranging from 50 to 1000, rounded to two decimal places. Null for cancelled rides.
misc_charge
           Description: Additional charges for the ride, such as tolls or surcharges.
           Values: Floating-point numbers ranging from 0 to 50, rounded to two decimal places. Null for cancelled rides.
total_fare
           Description: The total fare for the ride, including base fare and miscellaneous charges.
           Values: Calculated as the sum of ride_charge and misc_charge for completed rides. Null for cancelled rides.
payment_method
           Description: The method of payment used for the ride.
           Values:
           "Amazon Pay"
           "QR scan"
           "GPay"
           "Paytm"
Note: Null for cancelled rides.


