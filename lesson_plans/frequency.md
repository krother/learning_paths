
# Frequency

## Lesson Goal:

Students create pivot tables and histograms.

## Time Frame:

180'

## Key Concepts:

* absolute frequency
* relative frequency
* pivot table
* histogram
* aggregate
* normalize

## Lesson Plan

| step |  activity                                          |  time   |
|------|----------------------------------------------------|---------|
|  1.  | warmup: Worlde: MEDIAN                             | 5'      |
|  2.  | hotseat coding: challenge exercise 1               | 25'     |
|  3.  | play 3 rounds of "My Gold Mine"                    | 30'     |
|  4.  | students work through exercises in teams           | 20'     |
|      | *break*                                            | 20'     |
|  5.  | discuss results and establish concepts             | 20'     |
|  6.  | calculate frequencies from the penguin table       | 60'     |
|  7.  | (optional): good and bad plots                     |  *      |
|  8.  | Wrap-up: collect pandas commands on the board      |  5'     |

6. Discuss that there are three ways to calculate percentages (by row, by col, globally), establish **normalization**
7. Discuss the anatomy of a histogram on the board and how **binning** is related to it.

## 1. Warmup Wordle

Use the HTML/JS Wordle tool

## 2. Hotseat coding: challenge exercise 1

Start a notebook or Python file that has the import section complete.

Randomly find a volunteer. Give them the keyboard. Let the others guide them to implement the 

The purpose of the 

## 3. Play "My Gold Mine"

See [https://www.academis.eu/probably_fun/articles/frequency/README.html](https://www.academis.eu/probably_fun/articles/frequency/README.html)

## 4. Students work through exercises

Examine the dungeon card pile:

- calculate the **absolute frequency** of each card type (the number of times it occurs)
- calculate the **relativve frequency** of each card type (the percentage)
- draw the absolute frequencies as a bar chart
- add reflection questions 2-4, 7

## 5. Discuss results and establish concepts

Have students draw on the board:

- a column with **absolute frequencies**
- a column with **relative frequencies**
- a bar chart
- introduce the word **probability mass function** (will be needed in session 3+4)

Follow up with a student exercise to create pivots and draw a histogram.

## 6. Calculate frequencies from the penguin table

1. Continue with the penguin table
2. Count penguins by one category using **abolute frequency**.
3. Calculate percentages using **relative frequency**
4. Introduce the `pd.pivot_table()` function
5. Create bar charts from the pivot table
6. Normalize the pivot table in 3 different ways.

## 7. Good and bad plots

this is to fill time, look at 3-6 plots together and discuss them.

### Extras:

* vary the aggregation function
* draw a bar chart
* draw a heat map of the normalized frequencies

## TODO:

adapt the material from
[https://github.com/krother/datenvisualisierung/tree/main/pivot](https://github.com/krother/datenvisualisierung/tree/main/pivot)
