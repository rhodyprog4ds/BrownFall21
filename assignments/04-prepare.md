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
  - skill
* - drop nan rows from a dataset
  - prepare
* - display parts of a dataframe
  - summarize
* - impute a value to fill missing values
  - prepare
* - filter data based on extreme values or other outliers
  - prepare
* - convert a variable to one hot encoding
  - prepare
* - add a new column computed from one or more other columns
  - prepare
* - transform a dataset to tidy format
  - prepare
* - compute overall and individual summary statistics
  - summarize
* - use split-apply-combine paradigm
  - summarize
* - generate at least two types of plots
  - visualize
* - interpret statistics and plots
  - summarize, visualize
* - use list comprehensions or loops and pythonic conventions
  - python
* - load data from at least two types
  - access
* - compare data storage formats
  - access
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
