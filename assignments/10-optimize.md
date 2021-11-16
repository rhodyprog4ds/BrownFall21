---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/P9srJrwX)
  date : 2020-11-17 11:59pm
---
# Assignment 10: Tuning Model Parameters

## Quick Facts
- {{accept_assignment}}
- __Due: {{ date }}__

## Related notes

- [2021-11-08](../notes/2021-11-08)
- [2021-11-12](../notes/2021-11-12)

## Asseessment
```{list-table} Optimize model parameters
:header-rows: 1

* - task
  - skill
* - test the model on test data and interpret in context
  - classification, clustering, OR regression (2)
* - choose and justify appropriate parameters parameter grid for the context
  - classification, clustering, OR regression (2) AND process (2)
* - evaluate fit of the model while varying the cross validation parameters and interpret
  - evaluate (2)
* - optimize model parameter (s) and interpret
  - optimize (2)
* - ask releveant questions of the data domain and interpret results in context
  - process (2)
```


Note you can only earn one of classification, clustering, OR regression, but to
earn one of those you must both interpret the model and the parameters.

For process you must situate your overall analysis in context (which you should
  do even if you already have the process achievement; you should *always* do
  this) and explain how you're picking parameters to evaluate. Your reasons
  only have to be reasonable, they don't have to be correct.  It's okay if what
  you try doesn't improve the model, but then you have to interpret that.

## Instructions

**summary** Extend the work you did in assignment 7,8, or 9, by optimizing the model parameters.

1. Choose your dataset, task, and a model. It can be any model we have used in class so far.
1. Fit the model and show some exploration to choose reasonable model parameter values for your parameter grid
1. Use grid search to find the best performing model parameters
1. Examine and interpret the cv results. How do they vary in terms of time? Is the performance meaningfully different or just a little?
1. Try varying the cross validation parameters. Does this change your conclusions?


```{tip}
this is best for regression or classificaiton, but if you use clustering
use the `scoring` parameter to pass better metrics than the default
of the score method.
```

```{hint}
Assignment 11 will be to optimize two models and then compare two models on the same task
```

```{admonition} Thinking Ahead
What other tradeoffs might you want to make in choosing a model?
How could you present these results using your EDA skills?
```
