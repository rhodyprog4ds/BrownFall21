# Glossary

```{admonition} Ram Token Opportunity
Contribute glossary items and  links for further reading using the suggest an edit button behind the GitHub menu at the top of the page.
```


```{glossary}

[aggregate](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.core.groupby.DataFrameGroupBy.aggregate.html#pandas.core.groupby.DataFrameGroupBy.aggregate)
  to combine data in some way, a function that can produce a customized summary table

[anonymous function](https://en.wikipedia.org/wiki/Anonymous_function#:~:text=Anonymous%20functions%20are%20often%20arguments,than%20using%20a%20named%20function)
  a function that's defined on the fly, typically to lighten syntax or return a function within a function. In python, they're defined with the {term}`lambda` keyword.

[DataFrame](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)
  a data structure provided by pandas for tabular data in python.

[dictionary](https://docs.python.org/3/glossary.html#term-dictionary)
  a mapping array that matches keys to values.

git
  a version control tool; it's a fully open source and always free tool, that can be hosted by anyone or used without a host, locally only.

GitHub
  a hosting service for git repositories

index
  (verb) to index into a data structure means to pick out specified items, for example index into a list or a index into a data frame. Indexing usually invovlees square brackets `[]`
  (noun) the index of a dataframe is like a column, but it can be used to refer to the rows. It's the list of names for the rows.

interpreter
  the translator from human readable python code to something the computer can run.  An interpreted language means you can work with python interactively

iterate
  To do the same thing to each item in an {term}`iterable` data structure, typically, an iterable type. Iterating is usually described as iterate over some data structure and typically uses the `for` keyword

[iterable](https://docs.python.org/3/glossary.html#term-iterable)
  any object in python that can return its members one at a time. The most common example is a list, but there are others.

kernel
  in the jupyter environment, [the kernel](https://jupyter-notebook-beginner-guide.readthedocs.io/en/latest/what_is_jupyter.html#kernel) is a language specific computational engine

[lambda](https://docs.python.org/3.9/reference/expressions.html#lambda)
  they keyword used to define an anonymous function; lambda functions are defined with a compact syntax `<name> = lambda <parameters>: <body> `

[PEP 8](https://www.python.org/dev/peps/pep-0008/pep-0008/)
  [Python Enhancement Proposal](https://www.python.org/dev/peps/) 8, the Style Guide for Python Code.

repository
  a project folder with tracking information in it in the form of a .git file

suffix
  additional part of the name that gets added to end of a name in a merge operation
[Tidy Data Format](https://www.jstatsoft.org/article/view/v059i10)
  Tidy data is a database format that ensures data is easy to manipulate, model and visualize. 
  The specific rules of Tidy Data are as follows: Each variable is a column,
  each row is an observation, and each observable unit is a table. 
TraceBack
  an error message in python that traces back from the line of code that had caused the exception back through all of the functions that called other functions to reach that line. This is sometimes call tracing back through the stack

[Series](https://pandas.pydata.org/docs/reference/api/pandas.Series.html)
  a data structure provided by pandas for single columnar data with an index.  Subsetting a Dataframe or applying a function to one will often produce a Series

[Split Apply Combine](https://pandas.pydata.org/pandas-docs/stable/user_guide/groupby.html#group-by-split-apply-combine)
  a paradigm for splitting data into groups using a column, applying some function(aggregation, transformation, or filtration) to each piece and combinging in the individual pieces back together to a single table
```
