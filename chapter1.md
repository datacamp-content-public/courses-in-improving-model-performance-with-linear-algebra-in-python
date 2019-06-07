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

The objective of the exercise is to model and analyze the economy of the assumed country
based on the data.


The data consist of quantities  of 35 different products recorded from Day 1 to Day 360 for two consecutive years.

`@instructions`
1. Answer all questions.
3. For each question, you may use some few steps before the final one. Explain your code with a simple justification.
2. Questions will be marked based on correctness and related justifications.

`@hint`
Basics on Scipy (Numpy) can be found  on this link https://www.tutorialspoint.com/scipy/scipy_basic_functionality.htm

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
