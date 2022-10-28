# No-Show-Appointment-Udacity-project
# Dataset
This dataset collects information from 110k medical appointments in Brazil and is focused on the question of whether or not patients show up for their appointment. A number of characteristics about the patient are included in each row. These include Patients ID, Age, Appointment Date, Whether or not patient received sms for appointment etc. The overall dataset has a structure of (110527, 14) that's 110527 rows of data with 14 columns that describe each patient.

# Data Wrangling
This data from kaggle though looks clean, a bit of data cleaning was done to fix both data quality and tidiness issue which includes:

* Dropping PatientID and AppointmentID columns
* Dropping rows of data for patients whose age were below 1year.
* Converting scheduledday and appointmentday columns from object to datetime data type
* Adding two new columns b extrracting day and month from the appointmentday column

# Key Insights for Presentation
1. Wednesdays is the day that patients show up for appointment the most. Of the three months analyzed, May is appears to be the favorable day for appointment show up and lastly, patients show up for appointment if their appointmnt date is within 30 days of their scheduled date.
2. Eventhough the number of patient that showed up without receiving sms were many, I feel that the percentage of people that received sms were very small and I would recommend measures are put in place to reach out to these patients to remind them of their appointments. Generally, People between the ages of 40-59 have a better show up rate as compared to the others.
