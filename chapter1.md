---
title: Test
description: Test
---

## Familiarity with the Data

```yaml
type: NormalExercise
key: 698a5d3711
lang: python
xp: 100
skills: 2
```

The first step in feature engineering is understanding the data. The simplest way to do this is to start looking at the data with summary methods.

`@instructions`
- Print out the first 5 rows of the data
- Display summary statistics for each column of the data
- Instruction 3

`@hint`
- Here is the hint for this setup problem. 
- It should get students 50% of the way to the correct answer.
- So don't provide the answer, but don't just reiterate the instructions.
- Typically one hint per instruction is a sensible amount.

`@pre_exercise_code`
```{python}
import pandas as pd
```

`@sample_code`
```{python}
# Read in dataset, parsing the date column
data = pd.read_csv('online-retail_sample.csv', parse_dates = 'order_date')
```

`@solution`
```{python}
# Print the first five rows
data.head()

# Print a summary of each column
data.describe()
```

`@sct`
```{python}
# Update this to something more informative.
success_msg("Some praise! Then reinforce a learning objective from the exercise.")
```
