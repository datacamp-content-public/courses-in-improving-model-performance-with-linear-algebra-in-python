---
title: 'Chapter Title Here'
description: 'Chapter description goes here.'
free_preview: true
---

## Data Analysis Using Matrices

```yaml
type: NormalExercise
key: f6e7532727
xp: 100
```

This Exercise intends to use matrix concept to make some data modeling and  analysis.


This Exercise intends to use matrix concepts to make some data modeling and  analysis.
The objective of the exercise is to model and analyze the economy of the assumed country.
The data consist of quantities  of 35 different products recorded from Day 1 to Day 360 for two consecutive years. 
The data consists of four files and for two years. 

1. Year one: the data file for the first year are as follows:
	1. **Quantities1.csv: ** the data consisting of quantities  of 35 different products recorded from Day 1 to Day 360.  
     2. **Prices1.csv: ** the data consisting of the corresponding daily prices per unit of the 35 products. 
     
2. Year two: files **Quantities2.csv**  and **Prices2.csv** consisting of the quantities and prices for the same products within the second year.


# Question 1

1. Write a Scipy code to compute the double of each quantity exported in the first year
2. Write the command to compute the total daily exportation for each product within the two years.
3. Write  a code to computer the  per- product total income made for the first year. 
4. Write  a code to computer the  daily total income made for the second year. 
5. Compute the total amount of income for the period of the two years. 

# Question 2
Suppose the country want to double the daily total income of the second year,  for the next year (**Year 3**).
What is the total amount of each product required if the price matrix for the second year is kept for the third one? 

Hint: Formulate first the linear equation.

# Question 3

1. Consider the matrix consisting of the first 35 days lines of  ***Quantities1.csv**
2. Compute the Eigenvalues and Eigenvectors of this matrix.
3. What is its inverse?

# Question 4

Use the matrix obtained in Question 3 to study the independence of the daily amounts of quantities for the first 35 days and extend this ideal to the whole data set.

Hint: Use the determinant to make the decision.










`@instructions`
1.  Answer all question.
3. For each question, you may use some few steps before the final one. Explain your code with a simple justification.
2. Questions will be marked based on correctness and related justifications.

`@hint`
1.Basics on Scipy (Numpy) can be found  on this link https://www.tutorialspoint.com/scipy/scipy_basic_functionality.htm

`@pre_exercise_code`
```{python}
import scipy as s # importing scipy and nickname it as s

def Open_data(filename): # function to read files and group entries in a matrix excluding headings
    data =open(filename, "r") 
    for line in data:
        myentries.append(line.rstrip().split(","))
    data.close()
    Entries= s.matrix([[float(i) for i in row[1:]] for row in myentries[1:] ])  # deleting headings
    return Entries

Year1Quantities= Open_data("Quantities1.csv") # fist year quantities
Year2Quantities= Open_data("Quantities2.csv") # second year quantities
Year1Prices= Open_data("Prices1.csv") # first year unit prices
Year2Prices= Open_data("Prices2.csv") # second year unit prices










```

`@sample_code`
```{python}

```

`@solution`
```{python}

```

`@sct`
```{python}

```
