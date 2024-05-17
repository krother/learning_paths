
# Linear Regression (ML)

## Lesson Goal:

Students train a linear regression model.

## Time Frame:

180'

## Key Concepts:

* line of best fit
* linear equation
* slope
* intercept
* mean absolute error
* mean squared error

## Warmup:

* The case is housing price prediction: Brainstorm factors that influence the house price. Discuss in which direction they would influence it. 

## Content Delivery:

The backbone of the lesson are 6 CSV files that contain linear data of increasing complexity.
Slowly work with the students through each file, first inspecting and plotting the data, designing a model and training it.

The implementation can be done in a Jupyter notebook.

### File 01:

The x/y data is a perfect straight line through the origin. Introduce the equation:

    y = ax

You need a single data point to calculate a slope.

### File 02:

The x/y data is still a straight line, but it does not go through the origin. Extend the equation to:

    y = ax + b

The slope can be calculated from two data points manually, then calculate the intercept.

### File 03:

Now the x/y data contains noise. You need a quality metric. 
I suggest introducing the MAE as a easily interpretable metric (and because of file 05).
To identify the line of best fit you can random-guess model parameters and take the best one after a number of iterations. This is a good example of a stripped-down optimization algorithm.
It should also become clear in the process that random-guessing has a lot of disadvantages.

### File 04:

A bigger data set, otherwise very similar to 03.
You could use this as an opportunity to refactor the code.

### File 05:

This is a tricky one. The x/y data contains four artificial discrete parallel lines.
If you have the correct slope, the intercept can shift arbitrarily.
This example is to demonstrate the shortcomings of the MAE.

Introduce the MSE.

### File 06:

The x/y data does not have a linear relationship.
Discuss how you could find out.
Introduce and calculate a correlation coefficient.

## Wrap-Up

* inspect the 7th CSV file that contains two independent variables.

## Material:

* files linear_01.csv .. linear_06.csv
* sample Jupyter notebook with solution

## Comments:

The lesson should be followed by a session on optimizing multiple parameters (Normal Equation vs. Gradient Descent)
