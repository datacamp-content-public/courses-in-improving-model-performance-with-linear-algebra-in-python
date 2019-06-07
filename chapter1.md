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


`@instructions`
1.  Answer all question.
2. Questions will be marked based on correctness and related justifications.

`@hint`
1.Basics on Scipy (Numpy) can be found  on this link https://www.tutorialspoint.com/scipy/scipy_basic_functionality.htm

`@pre_exercise_code`
```{python}
import scipy as s # importing scipy and nickname it as s

data1 =open("exported_quantinties.csv", "r") # reading and working on the Qunatities file
myprices=[]
for line in data1:
   myprices.append(line.rstrip().split(","))
data1.close()
data2 =open("exported_unit_prices.csv", "r") # reading and working on the prices file
myquantities=[]
for line in data2:
   myquantities.append(line.rstrip().split(","))
data2.close()
# The following are the matrices to be worked on
Prices= s.matrix([[float(i) for i in row[1:]] for row in myprices[1:] ])  # deleting headings
Quantities= s.matrix([[float(i) for i in row[1:]] for row in myquantities[1:] ]) # deleting headings








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
