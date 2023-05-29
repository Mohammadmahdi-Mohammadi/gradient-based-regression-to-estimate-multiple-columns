# gradient-based-regression-to-estimate-multiple-columns
One of the critical tasks in the industry is predicting environmental measures such as pressure or temperature. You are given a dataset for bias correction of next-day maximum and minimum air temperatures forecast of the LDAPS model operated by the Korea Meteorological Administration over Seoul, South Korea. This data consists of summer data from 2013 to 2017. The input data comprises the LDAPS model's next-day forecast data, in-situ maximum and minimum present-day temperatures, and auxiliary geographic variables. This data has two outputs (i.e., next-day maximum and minimum air temperatures). You will use 2013-2015 data for training and 2016-2017 for tests.

a) Load the dataset, apply the needed preprocessing steps(missing values, normalization, outlier detection using K-Means, removing unneeded columns, etc.), and split the dataset to train and test sets.

b) With reasonable logic, choose and train a regression model(gradient-based) to estimate the "Next_Tmax" column. Report the SSE metric, and plot the regression and truth lines in one graph. (the x-axis will be the "date" with station ID, and the y-axis will be Next_Tmax values[estimated and truth]). Explain the parameters and model complexity you used; How did you reach it?

c) Now, we want to estimate "Next_Tmax" and "Next_Tmin" at the same time. How can you address this problem? Describe your answer and strategy.

d) Based on your strategy in the previous part, implement a gradient-based regression function that takes feature vectors and training parameters(learning rate, etc.), and can estimate the two above columns. Evaluate your model, report the SSE metric, and plot the regression and truth lines in one graph(one graph for each column).

e) Compare results in parts (b) and (d). which one is better? is it suitable to train one model to estimate one column or train one model to multiple columns?

f) Try to implement, and report results if we use normal equation to estimate two columns as the same time.

g) How KNeighborsRegressor works? Implement and evaluate it. Compare the results.
