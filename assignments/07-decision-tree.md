---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/zZzNUmzG)
  date : 2021-10-27 11:59pm
  recommended : 2021-10-26 11:59pm
---
# Assignment 7: Decision Trees

## Quick Facts
- {{accept_assignment}}
- _Recommended completion: {{ reccomended }}_
- __Due: {{ date }}__


## Related notes

- [2021-10-18](../notes/2021-10-18)
- [2021-10-20](../notes/2021-10-20)
- [2021-10-22](../notes/2021-10-22)

## Assessment
```{list-table} fit a decision tree
:header-rows: 1

* - task
  - skill
* - fit a decision tree
  - classification (2)
* - apply a decision tree to get predictions
  - classification (2)
* - interpret the model assumed by a decision tree
  - classification (2)
* - use multiple metrics evaluate performance
  - evaluate (2)
* - interpret how decisions (test/train size, model parameters) impact model performance
  - evaluate (2)
* - interpret the classifier performance in the context of the dataset
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

Choose a datasets that is well suited for classification and that has only numerical features.

```{tip}
A file can be a "comma separated file" and read in with `pd.read_csv` even if the
file name does not end in ".csv". The part after the '.' in a file name is
called the file *extension* and its a sort of metadata built into a file. CSV is a
specification for how to write data to a file, or a file *format*.  It's best
practice to make the file extension match the file format, but it's very much
not required. Espeically the older files on the UCI repository, the extension is
something else (eg dat, or data, or names), but the actual contents of the files are comma separated and compatible with `read_csv`
```

````{margin}
```{note}
If you want to use a dataset with nonnumerical features you will have to convert
the categorical features to one hot encoding or drop them if there are enough continuous values in addition to the categorical.   
```
````

Practice using decision trees and exploring how classification works, and what evaluations mean in the following exercises.

```{hint}
the Wisconsin Breast Cancer data from UCI is a good option as is the wine data set, which has the red & white wines separated, so you can earn prepare with this.  You could also use the NSA data and try to predict who will makes the NBA 75 based on their game stats, this would require some manipulation and so would be a way to earn construct.
```

### Part 1: DT Basics
1. Include a basic description of the data(what the features are)
1. Write  your own description of what the classification task is and why a decision tree is a reasonable model to try for this data.
1. Fit a decision tree with the default parameters on 50% of the data
1. Test it on 50% held out data and generate a classification report
1. Inspect the model to answer:

    - Does this model make sense?
    - Are there any leaves that are very small?
    - Is this an interpretable number of levels?
1. Repeat the split, train, and test steps 5 times.

    - Is the performance consistent enough you trust it?
1. Interpret the model and its performance in terms of the application. Some questions you might want to answer in order to do this include:

  - do you think this model is good enough to use for real?
  - is this a model you would trust?
  - do you think that a more complex model should be used?
  - do you think that maybe this task cannot be done with machine learning?


### Part 2: Exploring Evaluation

````{margin}


```{hint}
The most important thing about the max depth here is that it's the same across all of the models. If you get an error, try making it smaller.
```

```{tip}
The summary statistics and visualization we used before are useful for helping to
investigate the performance of our model.  We can try fitting a model  with different settings
to create a new "dataset" for our experiments.
The same skills apply.
```

````
Do an experiment to compare test set size vs performance:
1. Train decision tree with max depth 2 less less than the depth it found above on 10%, 30%, ... , 90% of the data. Save the results of both test and train accuracy for each size training data in a DataFrame with columns ['train_pct','n_train_samples','n_test_samples','train_acc','test_acc']
1. Plot the accuracies vs training percentage in a line graph.  
1. Interpret these results.  How does training vs test size impact the model?

```{hint}
use a loop for this part, possibly also a function
```

### Part 3: DT parameters

Experiment with DT Parameters:
1. Choose one parameter to change in the training that you think might improve the model and say why, then train a second decision tree
1. Check the performance of the new decision tree with at least two performance metrics
1. Did changing the parameter do what you expected?
1. Choose a second parameter to change in the training that you think might improve the model and say why, then train a third decision tree
1. Validate your third decision tree with at least two performance metrics.
1. Did changing the parameter do what you expected?



```{admonition} Thinking Ahead

Repeat your experiment from Part 2 with cross validation and plot with error bars.
- What is the tradeoff to be made in choosing a test/train size?
- What is the best test/train size for this dataset?

Repeat the experiment in part 2 with variations:
- allowing it to figure out the model depth for each training size, and recording the depth in the loop as well.  
- repeating each size 10 items, then using summary statistics on that data

Use the extensions above to experiment further with other model parameters.

**some of this we'll learn how to automate in a few weeks, but getting the
ideas by doing it yourself can help**
```
