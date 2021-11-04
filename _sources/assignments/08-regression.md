---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/_mbBAMxP)
  date : 2020-11-03 11:59pm
---
# Assignment 8: Regression

## Quick Facts
- {{accept_assignment}}
- __Due: {{ date }}__

## Related notes

- [2021-10-25](../notes/2021-10-25)
- [2021-10-29](../notes/2021-10-29)

## Assessment

```{list-table}
:header-rows: 1

* - task
  - skill
* - fit a linear regression model
  - regression (2)
* - evaluate fit of linear regression
  - evaluate (2)
* - use multiple metrics evaluate performance
  - evaluate (2)
* - interpret how decisions (test/train size, model parameters) impact model performance
  - evaluate (2)
* - interpret the model performance in the context of the dataset
  - process (2)
* - analyze the impact of model parameters on model performance
  - process (2)
* - use loops and lists effectively
  - python (2)
* - use EDA techniques to examine the experimental results
  - summarize (2), visualize (2)
* - create a dataset by combining data from multiple sources
  - construct (2)

```

## Instructions

Find a dataset suitable for regression. We recommend a dataset from the UCI repository.
Complete the following in a single notebook.

### Linear Regression Basics

Fit a linear regression model, measure the fit with two metrics, and make a plot that helps visualize the result.

1. Include a basic description of the data(what the features are)
1. Write  your own description of what the regression task is and why a decision tree is a reasonable model to try for this data.
1. Fit a linear model with 75% training data
1. Test it on 25% held out test data and measure the fit with two metrics and one plot
1. Inspect the model to answer:

    - Does this model make sense?
    - What to the coefficients tell you?
    - What to the residuals tell you?
1. Repeat the split, train, and test steps 5 times.

    - Is the performance consistent enough you trust it?
1. Interpret the model and its performance in terms of the application. Some questions you might want to answer in order to do this include:

  - do you think this model is good enough to use for real?
  - is this a model you would trust?
  - do you think that a more complex model should be used?
  - do you think that maybe this task cannot be done with machine learning?
1. Try fitting the model only on one feature. Justify your choice of feature based on the results above.  Plot this result.



### Part 2: Exploring Evaluation

```{note}
If you have the relevant level 2 achievements (evaluation, summarize, visualize)
you can skip this part, but it might still be interesting.
```

````{margin}



```{tip}
The summary statistics and visualization we used before are useful for helping to
investigate the performance of our model.  We can try fitting a model  with different settings
to create a new "dataset" for our experiments.
The same skills apply.
```

````
Do an experiment to compare test set size vs performance:
1. Re-fit your regression model using 10%, 30%, ... , 90% of the data for training. Save the results of both test and train r2 and MSE for each size training data in a DataFrame with columns ['train_pct','n_train_samples','n_test_samples','train_r2','test_r2','train_mse','test_mse']
1. Plot the metrics vs training percentage in a line graph.  
1. Interpret these results.  How does training vs test size impact the model?



```{admonition} Thinking Ahead

1. Try these experiments with a different type of regression.
1. How do your evaluation experiment results compare in regression vs classification?



```
