
# Lesson 1 - Machine Learning Fundamentals

## Goals

- Students identify use cases for supervised and unsupervised learning.
- Students train a tree-based model with scikit

## Suggested Actions

**Part 1: ML**

1. Wordle `MODEL`
2. introduce yourself
3. discuss administrative matters
4. brainstorming on Machine Learning
5. theory: what are models?
6. exercise: identify classification/regression/unsupervised

BREAK

7. warmup: tree puzzle
8. decision tree worksheet
9. evaluation of the trees
10. theory: random forest

BREAK

11. install required packages
12. practical exercise with scikit [SKIP THIS IF IT IS LATE AND DO IT NEXT CLASS]
13. wrap-up quiz questions

### 3. administrative matters

- we are two teachers
- teaching approch: theory + practical exercises
- show lecture dates + topics
- attendance (not required)
- exam (project: extract images from PDF
  (instead of https://www.academis.eu/machine_learning/project.html)
  *has to be done in groups of 3-4*
- Teams channel for general communication
- how to reach us; Kristian (kristian.rother@posteo.de)

### 4. Brainstorming

Ask: "what Machine learning systems have you used recently?".
Collect as many answers as possible.

(possible answers include: Deep Seek app, Spam filter, Netflix recommendations, Google Search, ...)

### 5. Theory "what is ML"?

Discuss the image on the fundamentals page or draw it on the board step by step. 
Use one example to explain all the concepts (e.g. a spam filter).

Make sure to cover the following concepts:

- model
- input data (X)
- prediction (y)
- model parameter
- hyperparameter
- fit

Conclude with the definition of ML by Tom Mitchell.
Then distinguish supervised and unsupervised learning.

- supervised learning:
  - classification
  - regression
- unsupervised learning

### 6. Exercise

Give students 10' to read the use cases on the fundamentals page and decide which is classification, regression and unsupervised.
After time runs out, have them vote:

- draw a legend on the board:

   "rock": unsupervised
   "paper": regression
   "scissors": classification


### 7. warmup: tree puzzle

Give students 2' to calm down after the break while they think about the puzzle on https://www.academis.eu/machine_learning/supervised/decision_trees/README.html

Ask them for answers and move on.

### 8. decision tree worksheet

Same as during the conference. Depending on the number of students in groups of 2-3 so that you have 6-8 groups.

Pay attention that the students are predicting the animals on the sheet, that was not 100% clear in the Pydata tutorial.

### 9. evaluation of the trees

go through the six animals (show them to), ask the students to predict using their trees. Build a table (a confusion matrix) with correct animal x predicted animal groups containing the count of predictions. It may take some time to collect all the outcomes but it helps to make sure the students understood what they are doing.

Ask how you could create a better predicition -> consensus

### 10. theory: random forest

http://www.r2d3.us/visual-intro-to-machine-learning-part-1/

briefly cover some of the theory (e.g. the GINI score, the CART algorithm, bagging vs. boosting). If you have some spare content here, you can use it to manage time.

### 11. install required packages

Show which packages are rquired to work during the course. Make it clear that the installation is homework and that questions should be directed to the Teams channel. The following will be required:

- numpy
- scikit-learn
- pandas
- matplotlib
- seaborn
- tensorflow

#### Installation commands:
  
Try any of:

      pip install scikit-learn
      python -m pip install scikit-learn
      python3 -m pip install scikit-learn (Mac)
      pip3 install scikit-learn (Mac)
      Make sure Python is in your PATH variable (on Windows; edit environment variables and start new powershell)
      in VSCode, install Python and Jupyter plugins.
      in VSCode, install the Python plugin (does not install Python)
      .. also install Jupyter

      --> **troubleshooting in Teams Channel**

### 12. practical exercise with scikit

Find a notebook that goes through a straightforward end-to-end case where a Decision Tree and Random Forest are trained using scikit.
I recommend the penguins dataset because it is small and robust.

Make sure everything works before and you understand the code.

Go through the steps slowly, explain what you are doing. Take the time to change a few of the parameters together.
You should see that the Decision tree does overfit easily, but the Random Forest is less prone to it.
(you may need to explain overfitting at that point)

https://github.com/krother/machine_learning/blob/main/solutions/random_forest.ipynb

### 13. wrap-up quiz questions

Take the MC-questions in the fundamentals chapter.
We might want to complement them with 3-4 more about trees & forests.

## Material

- https://www.academis.eu/machine_learning/fundamentals/what_is_ml/README.html
- https://www.academis.eu/machine_learning/supervised/decision_trees/README.html
- https://www.academis.eu/machine_learning/supervised/random_forests/README.html
