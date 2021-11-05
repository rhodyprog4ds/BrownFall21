---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/HDfrB13j)
  date : 2020-11-10 11:59pm
---

# Assignment 9: Clustering

## Quick Facts
- {{accept_assignment}}
- __Due: {{ date }}__

## Related notes

- [2021-11-01](../notes/2021-11-01)
- [2021-11-03](../notes/2021-11-03)
- [2021-11-05]()

## Assessment

```{list-table}
:header-rows: 1

* - task
  - skill
* - apply and interpret kmeans clustering
  - clustering
* - use multiple metrics evaluate performance
  - evaluate (2)
* - interpret how decisions impact model performance
  - evaluate (2)
* - interpret the classifier performance in the context of the dataset
  - process (2)
* - analyze the impact of model parameters on model performance
  - process (2)
* - usse EDA techniques to interpret the experimental results
  - summarize (2), visualize (2)
```

## Instructions

Use the same dataset you used for assignment 7, unless there was a problem, or pick one of the recommended ones for that assignment if you did not complete assignment 7.

1. Describe what question you'd be asking in applying clustering to this dataset.
1. Apply Kmeans using the known, correct
number of clusters, $K$.
1.  Evaluate how well clustering worked on the data:

    - using a true clustering metric
    - using visual inspection
    - using a clustering metric that uses the ground truth labels
1. Include a discussion of your results that addresses the following:

    - describes what the clustering means
    - what the metrics show
    - Does this clustering work better or worse than expected based on the classification performance (if you didn't complete assignment 7, also apply a classifier)
1. Repeat your analysis using a different number of clusters:

    - can you interpret the new clusters?
    - how to they relate to the original clusters? are they completely different, did one split? did some merge?
    - is there a reasonable explanation for more clusters than there are classes in this dataset?


```{admonition} Think Ahead

How  can clustering be used to ask many different questions? What can you do with clustering results?
```
