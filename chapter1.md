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
3. Write the a code to computer the  per- product total income made for the first year. 
4. Write the a code to computer the  daily total income made for the second year. 
5. Compute the total amount of income for the period of each income. 

# Question 2

# Question 3

# Question 4

# Question 5

# Question 6

# Question 7

# Question 8

# Question 9

# Question 10






`@instructions`
1.  Answer all question.
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
