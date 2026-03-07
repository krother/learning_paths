
# Convolutional Networks

## Lesson Goal:

Participants train a CNN on Fashion-Mnist data

## Time Frame:

120'

## Key Concepts:

- convolutional kernel
- feature map
- maxpool
- flatten

## Warmup:

Play 6 rounds of *Pictionary*:

Split the class in three teams. One team sends a volunteer to the board to draw something. The other teams guess. Whoever guesses first, gets a point. If there is a tie, the teacher draws one more object.

## Content Delivery:

### Part 1: Convolution on the board

Build the convolution mechanic on the board step by step.
I recommend using a 6x6 pixel face and a 3x3 kernel for eye recognition. Calculate the feature map, decide on a bias and apply a 2x2 max pool.
Let student parametrize a mouth detector. Let them calculate the result as well. 
You should end up with 8 numbers that you can flatten into a vector. Stop there.
(ask Kristian for example slides)

### Part 2: 

Train CNN on the Fashion MNIST data in Jupyter.

If the students already have a MLP they can use it as a starting point.
Otherwise you need to plan some more time, especially for the TF installation.
You need to provide the basic structure:

- preprocessing (different shape of data required)
- input layer
- conv2D layer
- maxpool2D
- activation (relu, can be built into conv2D)
- flatten, followed by Dense

Task them to vary the following hyperparameters:

- size of kernels
- number of conv2D layers
- number of filters

use model.summary() to see how the number of trainable parameters changes.

For faster training, start with a smaller sample of training data points (1000) - the model should overfit, providing a motivation for discussing regularization.

## Material:

see sample notebook solution

## Comments:

If you have time for a smaller teaching unit after this one, it is a good opportunity to add regularization methods and use them to optimize them mnist training. Pick from the following methods:

- EarlyStopping (easy)
- L2 (easy, add to layer)
- Dropout (tricky to implement but easy to explain)
- BatchNorm (hard to explain)

If things go well, explain the bias-variance tradeoff as well.
