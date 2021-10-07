---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/dX4PBo-T)
  date : 2020-10-12 11:59pm
---
# Assignment 5: Constructing Datasets and Using Databases


__Due: 2020-10-11__

```{list-table} access data from a database and merge multiple tables from a dataset
:header-rows: 1

* - task
  - skill
* - drop nan rows from a dataset
  - prepare (2)
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
* - append a dataset provided in pieces
  - construct (2)
* - merge data with a shared column
  - construct (2)
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
```


## Constructing Datasets

Your goal is to programmatically construct two ready to analyze dataset from multiple sources.

- Each dataset must combine at least 2 source tables(4 total).
- At least one source table must come from an sqlite database or from web scraping.
- You should use at least two different joins(types of merges, or concat).


The notebook you submit should include:

- a motivating question for why you're combining the datasets in an introduction section
- code and description of how you built and prepared each dataset. For each step describe what you're about to do, the code with output, interpretation that leads into the next step.
- exploratory data analysis that shows why you built the data and confirms that is prepared enough to analyze.

For construct, this can be very minimal EDA.

**You may build one dataset from three tables instead of two from two each if you'd like**

## Earning additional achievements

To earn additional achievements, you must do more cleaning and/or exploratory data analysis.

### Prepare level 2
To earn level 2 for prepare, you must, either on component table(s) or the final dataset:
- transform into a tidy format
- add a new column by computing from others
- handle NaN values by dropping or filling
- drop a column, row, or duplicates in another way

### Summarize and Visualize level 2
To earn level 2 for summarize and/or visualize, include additional analyses after building the datasets.
Include:
- compute overall summary statistics
- compute individual summary statistics
- use split-apply-combine with two categorical variables
- at least two types of plots for visualize
- use a categorical variable to modify the plot (color points or create subplots)


### Python Level 2

Use pythonic naming conventions throughout, AND:

- Use pythonic loops and a list or dictionary OR
- use a list or dictionary comprehension

```{admonition} Thinking Ahead
Compare the level 2 skill definitions to level 3, how could you extend and adapt what you've done to meet level 3? 
```
