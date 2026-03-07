
# Gradient Descent

## Lesson Goal:

Students fit a linear model from scratch.

## Time Frame:

90'

## Key Concepts:

- gradient
- learning rate
- loss function
- learning curve

## Warmup:

Let participants work through the puzzle on https://www.academis.eu/machine_learning/supervised/linear_regression/gradient_descent.html

## Content Delivery:

Use one example for this lesson and stick to it. The content is very abstract and requires a lot of mental space. The example can be small, simple, artificial data.

Cover some theory in the beginning. The GD formula is absolutely necessary and needs to be explained no matter how much linear algebra the students had before.

It helps to disambiguate concepts like: partial derivative, parameter space, Jacobian. Students frequently don't know where to put them.

Drawing a topographic map of the parameter space also helps to understand what we are even trying to do.

implement the GD algorithm from scratch following the instructions in the material.
This is not too easy and requires some fluency in Numpy.

Alternatively, take the solution from https://github.com/krother/machine_learning/tree/main/solutions
You might share the notebook with a few gaps and fill it together.

Other things you can do:

- start with a stupid loop that rolls random parameters and checks if they are better, repeat
- tweak the learning rate and see what happens
- tweak the number of iterations
- check the effect of scaling (multiply x2 by 1000, it should slow down the training considerably)
- take the MSE formula, apply the chain rule and calculate the partial derivative


## Material:

https://www.academis.eu/machine_learning/supervised/linear_regression/gradient_descent.html

If you have this model:

    ŷ = a1 * x1 + a2 * x2 + b

The partial derivative of the MSE is:

    [
       2/n * sum(a1 * x1**2 + a2 * x1 * x2 + b * x1 - y * x1),
       2/n * sum(a2 * x2**2 + a1 * x1 * x2 + b * x2 - y * x2),
       2/n * sum(a1 * x1    + a2 * x2      + b      - y)
    ]

(x1, x2 and y are vectors of the training data points)

## Comments:

see above