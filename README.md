# MSc Project: Develop A Waiting List Model for Elective Orthopaedic Knee Pathway
This repository contains the simulation model and analysis code for my MSc project at The University of Manchester.
The model simulates the journey of patients/referrals from GP referral to potential knee procedures, using fitted probability distributions based on real-world data.

## Requirements
```pip install -r requirements.txt```

## Project's Objective
To create 

## Data Structure
The structure of the dataset used to develop this simulation model consists of columns:
- Referral_ID: A unique identifier assigned to each patient referral.
\
- Event_Desc: The type of event recorded
\
- Event_Outcome: The result of status of the event/stage
\
- Event_Date: The date on which the event outcome occurred
\
- Event_Stage: A numeric code representing the sequence of event/stages in the pathway

## Simulation Model
### Routing
Stage 2 Outcome:
\
Conversion to Referral: 90.82%
\
Returned with Advice to Manage in Primary Care: 7.45%
\
Unknown Outcome: 1.73%

Stage 3 Outcome:
\
Follow-up but No Recorded Treatment: 43.70%
\
Discharged at 1st Outpatient Attendance: 28.22%
\
No Appointment Found: 14.30%
\
Follow-up with Recorded Treatment: 13.78%

### Fitted Distribution
Stage 1 to Stage 2:
\
Distribution: Exponential
\
Loc: 0.0
\
Scale: 10.145


Stage 2 to Stage 3:
\
Distribution: Weibull
\
Loc: -276.85
\
Scale: 525.05
\
Shape: 7.18

Stage 3 to Stage 4:
\
Distribution: Lognormal
\
Loc: -20.67
\
Scale: 490.37
\
Shape: 3.29

###

## Results
The simulated data

## Notes
For the reusability of the model, please ensure that the structure of the dataset used to run the model is the same.

