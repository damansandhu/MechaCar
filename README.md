# MechaCar
## Linear Regression to Predict MPG
* Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Vehicle weight, spoiler_angle & AWD provided a non-random amount of variance. The two variables that had the most amount of random variance are ground_clearance and vehicle_length.

* Is the slope of the linear model considered to be zero? Why or why not?
Our slope is not zero by looking at the p-value, 5.35e-11, which is less than 0.05 by a great margin.

* Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Our R-squared value is 0.7149, which means roughly ~71% of the time the model will predict mpg values correctly. There are probably other factors that were not captured in the datasaet that contribute to the mpg variability of the MechaCar prototypes.
![linear_regression](https://raw.githubusercontent.com/damansandhu/MechaCar/main/Images/Multiple_Linear_Regression.png)
![lot_summary](https://raw.githubusercontent.com/damansandhu/MechaCar/main/Images/lot_summary.png)
## Summary Statistics on Suspension Coils
* The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?

Lot 1 and Lot 2 are both within design specifications and have hnearly the same exact mean and median. Lot 3 shows the most variance and exceeds the manufacturers specs.
![total_summary](https://raw.githubusercontent.com/damansandhu/MechaCar/main/Images/total_summary.png)
## T-Tests on Suspension Coils
* In Lot 3 the PSI values are not different from the population mean. However lot 2 the p-value is 0.6072 which means there is evidence that the suspension coil is different from the population mean and in Lot 1 the p-value is 1, which is greatly over the mean.. All t-tests can be seen below:
![t.test1](https://raw.githubusercontent.com/damansandhu/MechaCar/main/Images/t.test.png)
![t.test2](https://raw.githubusercontent.com/damansandhu/MechaCar/main/Images/t.test_lots.png)
## Study Design: MechaCar vs Competition
Horsepower is something that car manufacturers advertise often, especially sports/muscle cars. I believe horsepower, mpg, and engine size are three factors that go into consumer decision making. We can use our tests to see if our MechaCar is much different from the competiton. We can make a null hypothesis stating that it is not different from the competition and our Alternative would be the opposite. To do this we will need to use our t-test after collecting data from different types of competitor vehicles. Our t-test will be comparing the population of all types of competitor vehicles.
