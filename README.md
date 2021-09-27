# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

(Insert Deliverable 1 Summary)

### Questions to answer:

- Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?

The vehicle weight, spoiler angle, and AWD all showed non-random variance to MPG values.

- Is the slope of the linear model considered to be zero? Why or why not?
The P-value is 5.35e-11 which is less than our standard .05 so the Null hypothesis is rejected.

- Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Our predicted accuracy rate or R-squared value is 0.7149 meaning it has a 71.5% accuracy rate. So, it has merit but will still be incorrect approximately 28.5% of the time.

## Summary Statistics on Suspension Coils

The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?


Suspension Coil Summary
(Insert Deliverable 2 summary)


Suspension Coil Lot Summary
(Insert Deliverable 2 Lot Summary)


As seen in the variance in our summaries show that the PSI values in total as well as in Lots 1, and 2 are within the design specification of less than or equal to 100. However, the variance of Lot 3 approximately 170 exceeds the design specifications.

## T-Tests on Suspension Coils

T-Test Overall
(Deliverable 3 Overall)
Overall P-Score .06028 > Standard of .05
T-Test Lot 1
(T-Test Lot 1)
Lot 1 P-Score 1 > Standard of .05
T-Test Lot 2
(T-Test Lot 2)
Lot 2 P-Score .6072 > Standard of .05
T-Test Lot 3
(T-Test Lot 3)
Lot 1 P-value .04168 < Standard of .05

## Study Design: MechaCar vs Competition

When comparing cars most consumers are highly interested in the vehicles fuel efficiency (MPG), horsepower, and safety rating. In order to show how our car stands against the competition we can use t-tests with these factors included to see the difference between MechaCar and its competitors.  Our null hypothesis would be that MechaCar is the same as the competitors and our alternative hypothesis would be that MechaCar is different than the competitors. We would be able to run these numbers after collecting data the same data sets from all competitors' vehicles. The T-test will be comparing the overall population of all types of competitor vehicles to MechaCar.
