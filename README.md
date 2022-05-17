# Case Study: A/B Testing for an eCommerce company

This is a final project of course "Data Wrangling, Analysis and AB Testing with SQL" by University of California, Davis Progress

## Assignment Task

We are running an experiment at an item-level, which means all users who visit will see the same page, but the layout of different item pages may differ. Please follow the steps below and good luck!

Compare the final_assignments_qa table to the assignment events we captured for ```user_level_testing```. Write an answer to the following question: Does this table have everything you need to compute metrics like 30-day view-binary?

Write a query and table creation statement to make ```final_assignments_qa``` look like the ```final_assignments table```. If you discovered something missing in part 1, you may fill in the value with a place holder of the appropriate data type. 

Use the final_assignments table to calculate the order binary for the 30 day window after the test assignment for ```item_test_2``` (You may include the day the test started)

Use the final_assignments table to calculate the view binary, and average views for the 30 day window after the test assignment for ```item_test_2```. (You may include the day the test started)

Use the [Abba](https://thumbtack.github.io/abba/demo/abba.html) to compute the lifts in metrics and the p-values for the binary metrics ( 30 day order binary and 30 day view binary) using a interval 95% confidence. 

Write up the test. Your write-up should include a title, a graph for each of the two binary metrics you’ve calculated. The lift and p-value (from the AB test calculator) for each of the two metrics, and a complete sentence to interpret the significance of each of the results.

## Results

* Order binary

We have not collected enough samples to be able to detect statistically significant lift of 1%. The p-value is 0.86 and the true mean is likely to be between -10% and 12%. This result is not statistically significant. There is a no substantial difference in the number of orders within 30days of the assigned treatment date betwee the two treatments.

* View Binary 

We have not collected enough samples to be able to detect statistically significant lift of 2,6%. The p-value is 0.2 and the true mean is likely to be between -1.4% to 6.5%. This result is statistically significant. However, there is still not a substantial difference in the number of views within 30days of the assigned treatment date between the two treatments.
