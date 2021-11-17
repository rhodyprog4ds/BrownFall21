---
jupytext:
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.10.3
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Portfolio Dates and Key Facts

```{code-cell} ipython3
:tags: [remove-input]

import yaml as yml
import pandas as pd
import os
pd.set_option('display.max_colwidth', None)


def yml_df(file):
    with open(file, 'r') as f:
        file_unparsed = f.read()

    file_dict = yml.safe_load(file_unparsed)
    return pd.DataFrame(file_dict)

outcomes_df = yml_df('../_data/learning_outcomes.yml')
outcomes_df.set_index('keyword',inplace=True)
schedule_df = yml_df('../_data/schedule.yml')
schedule_df.set_index('week', inplace=True)
# schedule_df = pd.merge(schedule_df,outcomes_df,right_on='keyword',  left_on= 'clo')
rubric_df = yml_df('../_data/rubric.yml')
rubric_df.set_index('keyword', inplace=True)
rubric_df.replace({None:'TBD'},inplace=True)
rubric_df.rename(columns={'mastery':'Level 3',
              'compentent':'Level 2',
              'aware':'Level 1'}, inplace=True)

```

```{code-cell} ipython3
:tags: [remove-input]



portfolio_dummies  = pd.get_dummies(rubric_df['portfolios'].apply(pd.Series).stack()).groupby(level=0).sum()
col_rename = {float(i):'P' + str(i) for i in range(1,5)}
portfolio_dummies.rename(columns =col_rename,inplace=True)


rubric_df = pd.concat([rubric_df,
                      portfolio_dummies],axis=1)


portfolio_cols = [ 'Level 3'] + ['P' + str(i) for i in range(1,5)]
portfolio_df = rubric_df[portfolio_cols]
```

This section of the site has a set of portfolio prompts and this page has instructions for portfolio submissions.  


Starting in week 3 it is recommended that you spend some time each week working on items for your portfolio, that way when it's time to submit you only have a little bit to add before submission.
The portfolio is your only chance to earn Level 3 achievements, however, you can also earn level 1 or 2.
The prompts provide a starting point, but remember that to earn achievements, you'll be evaluated by the rubric.
You can see the full rubric for all portfolios in the [syllabus](portfolioskills).
Your portfolio is also an opportunity to be creative, explore things, and answer your own questions that we haven't answered in class to dig deeper on the topics we're covering.
Use the feedback you get on assignments to inspire your portfolio.

```{important}
Each submission should include an introduction and a number of 'chapters'.  The grade will be based on both that you demonstrate skills through your chapters that are inspired by the prompts and that your [summary](intro_reflection) demonstrates that you *know* you learned the skills. See the [formatting tips](formatting) for advice on how to structure files.
```

In each chapter(for a file) of your portfolio, you should identify which skills by their keyword, you are applying.

You can view a (fake) example [in this repository](https://github.com/rhodyprog4ds/portfolio-example) as a [pdf](https://github.com/rhodyprog4ds/portfolio-example/blob/gh-pages/portfolio.pdf) or as a [rendered website](https://rhodyprog4ds.github.io/portfolio-example/intro.html)

## Current: Check 3

The third submission will be graded on the following criteria and due on  {{ p3due }}:

```{code-cell} ipython3
:tags: [remove-input]

portfolio_df['Level 3'][portfolio_df['P3']==1].reset_index().set_index('keyword')
```

Submision Checklist:



- [ ] update your gh action or precommit hook
- [ ] complete your KWL chart
- [ ] add notebooks

## Upcoming Checks

<!-- - Check 2: {{ p2due }}   -->
<!-- - Check 3: {{ p3due }}   -->
- Check 4: {{ p4due }}  


<!--
```{code-cell} ipython3
:tags: [remove-input]

portfolio_df['Level 3'][portfolio_df['P2']==1].reset_index().set_index('keyword')
```


The first portfolio check will be due {{ p2due }} and will cover the following skills.

```{code-cell} ipython3
:tags: [remove-input]

portfolio_df[portfolio_df['P2']==1]
```







```{code-cell} ipython3
:tags: [remove-input]

portfolio_df['Level 3'][portfolio_df['P4']==1].reset_index().set_index('keyword')
```
 -->
