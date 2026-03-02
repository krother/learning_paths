
# Artificial Neural Networks

## Goals

- students manually set parameters of an ANN
- students train an ANN with Tensorflow

## Suggested Actions

(if not everything was completed in the first session,
go through the scikit notebook with Random Forest after 1.)

**Part 1: ANNs**

1. Wordle: BRAIN
2. history of ANNs
3. exercise: set parameters of an ANNs

BREAK

**Part 2: Training ANNs**

4. exercise: TF Playground
5. key concepts of ANN training
6. exercise: train a MLP with scikit   

BREAK

**Part 3: TensorFlow**

7. go through notebook that trains a model on Fashion data
   (move to next session if scikit notebook moved from session 1)
8. Networking tips
9. recap questions

### 1. Wordle: BRAIN

So students learn that each session starts in the same way.

### 2. history of ANNs

- cover a bit of history like the AI winter(s)
- noteworthy visuals incluse: the biological neuron, excerpt from Turings paper, Geoffrey Hinton (Noble Prize for Backpropagation 2024).

Key concepts:

- neuron
- weights
- bias (aka intercept)
- dot product
- activation function
- Multi-Layer Perceptron

Do an example calculation on the board.
Point out that the input of any neural network has to be numbers.

### 3. exercise: set parameters of an ANNs

Show the single neuron with missing parameters on academis.eu

- Explain the task: find *one* set of parameters for the neuron so that all four input/output pairs work.
- let students work on the first set for ~5 min. (logical AND)
- optionally the second set (OR)
- ask for solutions.

### 4. exercise: TF Playground

Ask students to spend 10 min. on playground.tensorflow.org and try to fit some of the datasets.

### 5. key concepts of ANN training

Go through 3 questions with the class (write them on the board in the meantime):

a) What does happen during the training?

Should result in 3 new concepts that you can explain briefly:

- epochs
- learning curve (top right)
- Gradient Descent with Backpropagation (the algorithm)

b) What hyperparameters does the model have?

Complete the students answers:

- activation function
- number of layers
- number of neurons
- number of epochs
- regularization
- learning rate
- input feature engineering

(you need definitions for each that are shared with students)

conclusion: ANNs have *a lot* of hyperparameters

c) What makes the training succeed?

possible answers:

- more neurons -> better fit
- transformed features -> trains faster
- ReLU works better than sigmoid

#### Variation

One could hand out the ~6 topics for research by students. Depends on how good your control of the group and topic is. If this is your first time I wouldn't do it.

### 6. exercise: train a MLP with scikit

The purpose of this section is to show how training an ANN looks like.
 
You can use the penguin notebook in solutions/MLP. It is almost the same as the random forest with scikit notebook. There is one important addition: data needs to be scaled for ANNs-> -3 .. +3 is a good range

- use a StandardScaler to scale the data.
- show the training with and without scaling.

This is also a good opportunity to answer questions about the workflow.

### 7. go through notebook that trains a model on Fashion data

You might ask who has installed TensorFlow.

Go through the Fashion MNIST notebook in solutions/fashion_mnist_mlp.ipynb
They should see:

- the sequence of layers in the model definition
- the shape of the input data
- the output of model.summary()
- the output of the .fit() call
- which loss function is used (you might want to explain the formula)
- which activation function is used (you might want to show and explain the activation plots for ReLU, sigmoid and softmax)
- the plotted learning curve

#### Challenge: 

Let the students train models on the Fashion data with tensorflow using the prepared notebook and optimize hyperparameters. You create an empty table on the board, where students can put in their results. Use the columns:

| initials | Layers + neurons | activation | epochs | train score | test score |

Collect 5-7 models in the table.

Recommended steps:

- start with a very small model
- make it bigger and see if accuracy goes up
- make it much bigger, should overfit
- make it a bit smaller
- add regularization

### 8. Networking opportunities

Mention places where you can network and learn what people do:

 * PyData meetups
 * PyLadies
 * Python Users Berlin
 * AI Guild
 * Ines Montani homepage / Meetup / Feminist AI LAN Party
 * conferences (calendar on https://pythondeadlin.es/)
 * Advent of Code (Kristian runs a support group Dec 1st-20th with daily meetings)

### 9. recap questions

Present and ask prepared MC-questions (sent separately).
