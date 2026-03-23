
# Backpropagation

Backpropagation is difficult. Very difficult. You can spend 3 hours on the differential equations. I strongly advise against that unless you know what you are doing and have an idea to make it interesting.

## Warmup

If you haven't done so yet, have the students solve the "checker" problem on [playground.tensorflow.org](playground.tensorflow.org). This is an example of a nonlinear problem, the XOR problem is very similar.

Ask students what is happening. This is a good recap.

Then let us consider a different nonlinear problem: You have a single feature x1 and want to classify points as 'X' and 'O':

X X O O O O X X

---------------> x1

It should be clear that you cannot separate the points by a straight line. Now imagine that you create a second feature x2 so that:

x2
^
| X X         X X
|   
|     O O O O 
|
------------------> x1

The separation by a single line suddenly works. This is more or less what a NLP does. The question is: where do its parameters come from (repeat the model equation at this point):

y = sigmoid(w2 @ sigmoid(w1 @ X))

 X: input matrix
w1: parameters of hidden layer (including bias)
w2: parameters of output layer (including bias)
 @: matrix multiplication

## Content

You have several options how to approach this. Pick one:

### 1. Backpropagation by Kagan:

A guided step-by-step tutorial that is not too difficult: [https://burakkagann.github.io/Pixels2GenAI/content/Module_09_intro_neural_networks/9.1_neural_network_fundamentals/9.1.2_backpropagation_visualization/README.html](https://burakkagann.github.io/Pixels2GenAI/content/Module_09_intro_neural_networks/9.1_neural_network_fundamentals/9.1.2_backpropagation_visualization/README.html)

The main exercise would be to play with the learning rate and see what happens.

### 2. Gradient Descent

If students had no prior exposure to GD, you can skip the hidden layer and train a single neuron instead. You can cover the fundamentals from [https://www.academis.eu/machine_learning/supervised/linear_regression/gradient_descent.html](https://www.academis.eu/machine_learning/supervised/linear_regression/gradient_descent.html)

It is still a longer coding exercise. Multiple solutions are on [https://github.com/krother/machine_learning/tree/main/solutions](https://github.com/krother/machine_learning/tree/main/solutions)

### 3. Backpropagation from scratch

This is the most challenging. First, go through the chain rule and deduce the partial derivative of the log-loss function. 
Then guide the students through the implementation starting from an emptied version of one of the **neural_network_from_scratch** notebooks on https://github.com/krother/machine_learning/tree/main/solutions/neural_networks .  

Do not do this if you teach the subject for the first time. I had instances of spending 1.5 days on this subject to do it properly. It can be very draining for the students.
