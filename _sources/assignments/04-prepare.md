---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/DDHG6bu4)
  date : 2020-10-05 11:59pm
---
# Assignment 4:

__Due: {{ date }}__

{{ accept_assignment }}

```{list-table} practice basic pandas by reshaping and organizing data
:header-rows: 1

* - task
  - skill (max level)
* - drop nan rows from a dataset
  - prepare (2)
* - display parts of a dataframe
  - summarize (1)
* - impute a value to fill missing values
  - prepare (2)
* - filter data based on extreme values or other outliers
  - prepare (2)
* - convert a variable to one hot encoding
  - prepare (2)
* - add a new column computed from one or more other columns
  - prepare (2)
* - transform a dataset to tidy format
  - prepare (2)
* - compute overall and individual summary statistics
  - summarize (2)
* - use split-apply-combine paradigm
  - summarize (2)
* - generate at least two types of plots
  - visualize (2)
* - interpret statistics and plots
  - summarize, visualize
* - use list comprehensions or loops and pythonic conventions
  - python (2)
* - load data from at least two types
  - access (2)
* - compare data storage formats
  - access (2)
* - match EDA techniques to questions appropriately
  - process (1)
```

For this assignment, prepare the provided datasets.  Your preparation needs to include the following steps and narrative description of how you're making decisions about your data cleaning.

The notebooks in the template have instructions for how to work with each dataset.

To earn prepare level 2, clean the data and do just enough exploratory data analysis to show that the data is usable (eg 1 stat and/or plot).
For prepare level 2:
- travel_times AND
one of:
- cs_degrees, airlines, and coffee

To earn summarize and visualize level 2, add extra exploratory data analyses meeting the criteria above.

To earn python level 2, make sure that you use a function or lambda and comprehension or pythonic loops somewhere. The CS degrees data will have that, but it's harder. The coffee data will be the easiest one to get all python level 2.

For access level 2 you must clean the airline data (to get data in a second file type).

```{hint}
renaming thing is often done well with a dictionary comprehension or lambda.
```

<!-- - display only part of the dataframe to build a narrative of how you are making decisions
- drop rows with `NaN` in one column, based on what is most important for the dataset
- retain only some of the columns of the dataset
- fill in missing values for one column with an appropriate value (eg the mean)
- convert a categorical variable to one-hot encoding
- add a column to the dataset that is computed by applying a custom function to other columns -->
