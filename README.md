# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG

![R_linear_model](https://user-images.githubusercontent.com/85756203/136996559-08459736-6e8f-4597-8e47-062f556fc449.png)


We need to examine the p-value of the variables to determine whether a variable may impact the MechaCar mpg. 
The ground_clearance and vehicle_length variables have p-values of less than 0.05. Those two variables appear to have an impact on the mpg of our MechaCar.

To find whether the slope of our linear model would be considered 0, we need to look at the p-value of our linear model. The p-value of our model is less than 0.05, which suggests there is a correlation happening from our data.
That means the slope of our line would be considered non-zero because a slope of zero would mean there is no correlation in the data.

The R-squared variable shows how consistent our model will be at accurately predicting results. The R-squared of our model is 0.7149. About 71-percent of the time, our model will predict the mpg of the MechaCar.

Because of the R-squared value, I do believe this is an effective linear model.

## Summary Statistics on Suspension Coils

![R_psi_summary](https://user-images.githubusercontent.com/85756203/136996616-55e7d081-5236-483b-b27a-8b556d71b101.png)

![R_lot_psi_summary](https://user-images.githubusercontent.com/85756203/136996633-bfefec04-6bd7-4265-96d9-386cd5e60a7a.png)

The current manufacturing data does not meet the requirements in total for the MechaCar suspension. Each of the manufacturing lots is required to have a variance of less than 100 psi. From our data, Lot 3 has a variance of 170 psi.
Lots 1 and 2 are both under the required level with a variance of 0.980 and 7.47, respectively.

## T-Tests on Suspension Coils

For this part of our assignment, we ran four different t-tests to see if there was any difference in the PSI of MechCar based on the manufacturing lot.

The base t-test produced the results below.

![R_coils_t-test](https://user-images.githubusercontent.com/85756203/136996672-a052c55b-d315-41ce-b578-c49a2369e6b9.png)

The p-value of 0.06028 is not low enough to reject the null hypothesis. Meaning, there is no evidence to show a statistical difference in the means of the PSI.

![R_lot_1_t-test](https://user-images.githubusercontent.com/85756203/136996697-829bcb25-213d-40f8-b862-22db7ac33729.png)
![R_lot_2_t-test](https://user-images.githubusercontent.com/85756203/136996706-5dd023e6-5665-4f68-83aa-6885fb118a64.png)

The tests for Lot1 and Lot2 also produced the same results.

![R_lot_3_t-test](https://user-images.githubusercontent.com/85756203/136996730-fd173459-1b78-4fae-9855-5de5d5a83973.png)

The Lot3 t-test had a resulting p-value of 0.04168.  That tells us a difference in the average PSI in cars produced from Lot3 compared to our base mean PSI (1500) exists.

## Study Design: MechaCar vs. Competition

I believe performing a study to test the fuel efficiency of the MechaCar compared to other vehicles is a solid indicator of the vehicle's performance for consumers.

Null Hypothesis: There is no difference between the average MPG of the MechaCars vs. the competitors.
Alternate Hypothesis: There is a difference in the average MPG of the MechaCar vs. the competitors.

The statistical test I would run for this study would be a  two-sample t-test. I would run a two-sample t-test because we are comparing two different sample averages.

The only data we need to collect is the average MPG from the MechaCars and competitors' vehicles.

We already have a sample of MechaCars that includes MPG, which we could use for this test. That data also includes ground_clearance and vehicle_length, and we already concluded those appear to impact the MPG of the MechaCar. It would be helpful to try and find competitors' vehicles that have similar measurements in those areas because that can improve the accuracy of our results.
