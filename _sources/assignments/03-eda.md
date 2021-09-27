---
substitutions:
  accept_assignment: |
    [Template repo for submission](https://classroom.github.com/a/WL4HroJ_)
  date : 2020-09-28 11:59pm
---

# Assignment 3: Exploratory Data Analysis

__Due:{{ date }} __

{{ accept_assignment }}

## Objective & Evaluation

This week your goal is to do a small exploratory data analysis for two datasets of your choice.

```{list-table} plot basic views of data and generate descriptive statistics and basic plots
:header-rows: 1

* - task
  - skill (max level)
* - compute and display overall statistics
  - summarize (2)
* - compute and display individual statistics of a datasets
  - summarize (2)
* - group a data set by a variable and compute summary statics
  - summarize (2)
* - plot two different pairwise relationships
  - visualize (2)
* - interpret the statistics and plots
  - summarize (2), visualize (2)
* - load data from at least two different file types
  - access (2)
* - compare and contrast the file types and/or sources
  - access (2)
* - match questions appropriate to the dataset and match plots and stats
  - process (1)
```

## Choose Datasets

Each Dataset must have at least three variables, but can have more. Both datasets
must have multiple types of variables. These can be datasets you used last week,
if they meet the criteria below.

### Dataset 1 (d1)

must include at least:
- two continuous valued variables and
- one categorical variable.


### Dataset 2 (d2)

must include at least:
- two categorical variables and
- one continuous valued variable


## EDA

Use a separate notebook for each dataset, name them `dataset_01.ipynb` and `dataset_02.ipynb`.

For **each** dataset, in a dedicated notebook, complete the following:

1. Load the data to a notebook as a `DataFrame` from url or local path, if local, include the data in your repository.
1. Explore the dataset in a notebook enough to describe its structure use the heading `## Description`

    - shape
    - columns
    - variable types
    - overall summary statisics
1. Write a short description of what the data contains and what it could be used for
1. Ask and answer 4 questions using statistics, split-apply-combine, and visualizations. Make a heading for each question using a markdown cell and H2:`##`. Make sure your analyses meet the criteria in the check lists below. Interpret the answer from the analysis/plot.
1. Describe what, if anything might need to be done to clean or prepare this data for further analysis

### Dataset 1 Checklist



1. Overall summary statistics grouped by a categorical variable
1. A single statistic grouped by a categorical variable
1. a scatter plot with the points colored by a categorical variable
1. a plot and summary table that convey the same information. This can be one statistic or many.


### Dataset 2 Analysis

1. two individual summary statistics for one variable
1. one summary statistic grouped by two categorical variables
1. a figure with a grid of subplots that correspond to two categorical variables
1. a plot and summary table that convey the same information. This can be one statistic or many.



```{tip}
Be sure to start early and use help hours to make sure you have a plan for all of these.
```




````{margin}
```{warning}
This section is not required, but is intended to help you get started thinking
about ideas for your portflio.  If you complete it, we'll give your feedback to
help shape your ideas to get to level 3 achievements.  If you want to focus only
on level 2 at this moment in time, feel free to skip this part.
```
````

```{admonition} Think Ahead
1. How could you make more customized summary tables?
1. Could you use any of the variables in this dataset to add more variables that would make interesting ways to apply split-apply-combine? (eg thresholding a continuous value to make a categorical value)
```
