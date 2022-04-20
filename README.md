# MechaCar_Statistical_Analysis

## Linear Regression to Predict MPG
![Deliverable 1](https://user-images.githubusercontent.com/90940985/164297572-ef80636a-be05-42e1-882b-4eae961571b6.jpg)

### Which variables/coefficients provided a non-random amount of variance to the mpg values in the dataset?
Based on the results, I would say the following provided a non-random amount of variance:
- vehicle weight (0.0776)
- spoiler angle (0.3069)
- AWD (0.1852)

### Is the slope of the linear model considered to be zero? Why or why not?
No, because the p-value is less than 0.05. According to our module 15.7.2, because the p-value of our linear regression analysis is 5.35e-11, which is much smaller than our assumed significance level of 0.05%. Therefore, we can state that there is sufficient evidence to reject our null hypothesis, which means that the slope of our linear model is not zero.

### Does this linear model predict mpg of MechaCar prototypes effectively? Why or why not?
Based on the summary output, the value of r-squared is 0.71. That means that approximately 71% of all mpg predictions will be correct when using this linear model.

## Summary of Statistics on Suspension Coils
![Deliverable 2](https://user-images.githubusercontent.com/90940985/164334476-28f478a2-4a1f-4c6b-9bcd-8300b1749ff2.jpg)

### The design specifications for the MechaCar suspension coils dictate that the variance of the suspension coils must not exceed 100 pounds per square inch. Does the current manufacturing data meet this design specification for all manufacturing lots in total and each lot individually? Why or why not?
According to the total_summary table for all 3 lots, the mean is consistent at 1498.7. The variance is 62.293 and the StdDev is 7.892. The median value varies between 1452 and 1542. The variance and std dev are within the design specifications do not exceed 100 pounds per square inch for any of the 3 lots.

![Deliverable 2 1](https://user-images.githubusercontent.com/90940985/164335102-523f0fc7-850f-40f1-ad65-5ba67dc5c28c.jpg)

![Deliverable 2 2](https://user-images.githubusercontent.com/90940985/164335373-ce27011e-459a-428e-ae43-7006170a868d.jpg)

![Deliverable 2 3](https://user-images.githubusercontent.com/90940985/164335388-25571658-982e-459a-a3ef-e55686a953ae.jpg)

Looking at each lot individually, Lot 1 and Lot 2 are well below the 100 PSI design specification, but Lot 3 has a variance of 170.286 and st dev of 13.05 which puts it above the design specification.

## T-Tests on Suspension Coils

![Deliverable 3 1](https://user-images.githubusercontent.com/90940985/164335563-6c4aaa6d-c99b-4d18-bf4b-1ef9fdefe213.jpg)

![Deliverable 3 2](https://user-images.githubusercontent.com/90940985/164335582-12b54da4-e36a-4f54-b4ce-3aa30b8de01b.jpg)

Based on the t-tests performed, the p-value for all three lots is 0.06028 which is outside the signifigance level of 0.05. This puts our confidence interval at 93.972%. Which means there is not enough evidence to reject the null hypothesis. 
## Study Design: Mechacar vs Competition
To compare the Mechacar to other cars, I would look at fuel efficiency. I would use the 6 variables already in the data set and I would include things such as fuel tank size to see how it compared to short and long trips compared to competition. I would compare it to a data set of cars with similar price and size.

### What Metrics are you going to test?
I would test all numerical data and use very large samples. The data samples will be randomly selected with similar variance.

### What is the null hypothesis or alternative hypothesis?
HO: The Mechacar mpg data set has no statistical difference from the competitions mpg data set.
Ha: The true mean of the Mechacar's mpg is greater than that of the competitors.

### What statistical test would you use to test the hypothesis? And why?
I would run more t-tests to compare the data sets. The t-test gave us the necessary information to make a reasonable prediction so I think we could use it for this as well.

### What data is needed to run the statistical test?
We would need the data from the variables listed above. We would need a p-value set at 0.05 so that we can have 95% accuracy of our alternative hypothesis.
