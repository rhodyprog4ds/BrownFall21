---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/XHCX306d)
  date : 2021-12-08 11:59pm
  early: 2021-12-02 6:00pm
---

# Assignment 12: Fake News

## Quick Facts
- {{accept_assignment}}
- First feedback: {{ early }}
__Final due date: {{ date }}__


## Evaluation
```{list-table} use text to predict fake from real news
:header-rows: 1

* - task
  - skill
* - transform text data to a format compatible with ML
  - representation (2)
* - plan to solve a real world problem using the tools from class
  - workflow (2)
* - usse EDA techniques to interpret the experimental results
  - summarize (2), visualize (2)
* - determine the best model for this task
  - compare (2)
* - determine the best parameter settings for this task
  - optimize (2)
```

## Instructions

Use the dataset in the assignment template repo to answer the following questions.
The data includes variables:
- ‘text’: contents of an article
- ‘label’: whether it is real or fake news
- 'title': title of the article

1. Is the text or the title of an article more predictive of whether it is real or fake?
1. Are titles of real or fake news more similar to one another?

Consider what difference you can have in how you represent the data and how that might impact your model performance in order.
Use summary statistics and visualizations appropriately in order to explain your results.

```{hint}
The data set contains a large number of articles (takes a long time to train), you can downsample this to something like a 1,000 articles or so in order to speed up training and evaluation (hint: use shuffle).

```
