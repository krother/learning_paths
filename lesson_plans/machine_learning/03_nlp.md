
# Lesson 3 - NLP

## Goal

- Students train a classification model on a bag of words
- Students compare word vectors
- Students find similar documents using Cosine similarity

## Suggested Actions

**Part 1: Warming up**

1. Wordle: WORDS
2. NumPy warmup exercise
3. Recap: Learning curves exercise
4. Follow up with any leftovers from session 2, even if that takes longer

**Part 2: Bag of Words**

5. Bag of words
6. Example: vader sentiment
7. Prediction with bag of words

BREAK

**Part 3: Embeddings**

8. Spacer: Word guessing Game
9. Theory on Embeddings
10. Spacy Exercise
11. Cosine Similarity Exercise
12. Recap Questions

## 3. Learning curves exercise

Show the images in https://github.com/krother/machine_learning/tree/main/classroom_exercises/learning_curves
and interpret them together (solution in README.md)

## 5. Bag of Words:

Start with a rhetoric question: How to convert words to numbers?

Develop the bag of words approach on the board:

- Write a sentence on the board, e.g. "the answer to life, the universe and everything else is 42".

- count each word, make a table with all unique words and their count
- remove stop words -> edit the table to make it simpler
- replace the number by [NUM]
- apply stemming (is -> be)

Discuss pros and cons. Students might come up with:

- good: fast
- good: easy to explain
- bad: similar words are not recognized
- bad: drops word order completely

### 6. Application example: vader

Show an application example: The vader sentiment library.

Run the code in `vader.py` on
https://github.com/krother/python_library_examples/tree/master/vader

Exercise: run the code and calculate sentiment scores for a couple of sentences.

### 7. Prediction with bag of words

For the practical application you need the file `lyrics.json`. If you don't have it look up the newsgroup dataset in scikit-learn.

Slowly go through the notebook:
https://github.com/krother/machine_learning/blob/main/solutions/neural_networks/bag_of_words.py

Point out that the CountVectorizer produces a *sparse matrix* (lots of zeros).


### 8. Spacer: Word guessing Game

At this point you may want to do a word-guessing game:

- find two volunteers
- show a word to the others (table, bar, python)
- ask the others to give hints that consist of a single word
- play 3 rounds with different people.

## 9. Theory on Embeddings

Claim: we want something that takes the similarity of words into account.

Find some similar words on https://projector.tensorflow.org/
Let students find some as well.

Then take apart the theory:

Draw the KING - MAN + WOMAN = QUEEN diagram (there are 1M copies of it on the web).

Explain:
- we want to represent words by vectors
- vectors allows additions / subtractions
- vectors allow calculating similarity (by cosine similarity)
- word vectors can be used to calculate document vectors (sum of all word vectors divided by their count)
- vectors can have different numbers of dimensions, between 50 (GloVe) and 12000+ (GPT)

### 10. Exercise:
calculate word similarities with Spacy:
https://github.com/krother/machine_learning/blob/main/solutions/neural_networks/word_similarity.py

### 11. Exercise:
Use a bot to implement a Cosine Similarity function. Explain what Cosine Similarity does.

Explain that it is super fast compared to the alternatives, once the 

### Recap questions

Present and ask prepared MC-questions (sent separately).
