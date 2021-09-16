---
substitutions:
  accept_assignment: |
    [accept the assignment](https://classroom.github.com/a/damCPljl)
  date : 2020-09-21
---
# Assignment 2: Practicing Python and Accessing Data


due : {{ date }}



## Objective & Evaluation

This assignment is an opportunity to earn level 1 and 2 achievements in `python` and `access` and begin working toward level 1 for `summarize`. You can also earn level 1 for `process`.

In this assignment, you'll practice/ review python skills by manipulating datasets
and extracting


```{list-table} practice python by manipulating data files, load datasets of different types
:header-rows: 1

* - Task
    Skills (max level)
* - identify possible uses for data in a data science pipeline
    [process (1)]
* - load data from one file format
    [ access (1)]
* - load data from at least two of  (.csv, .tsv, .dat, database, .json)
    [access (2)]
* - compare the data formats
    [ access (2)]
* - complete the assignment in python
    [python (1)]
* - use python data types (eg dictionaries) to prepare information about datasets
    [python (2)]
* - use informative variable names, pythonic iteration, and other common PEP 8 conventions
    [python (2)]
* - display DataFrame properties
    [summarize (1)]
```

First, {{ accept_assignment }}. It contains a notebook with some template structure (and will set you up for grading).


## Find Datasets

Find 3 datasets of interest to you that are provided in at least two different file formats. Choose datasets that are not too big, so that they do not take more than a few second to load. At least one dataset, must have non numerical (eg string or boolean) data in at least 1 column.

In your notebook, create a markdown cell for each notebook that includes:
- heading of the dataset's name
- a link to where someone can learn about the dataset
- a 1-2 sentence summary of what the dataset contains and why it was collected
- 1-2 questions you would like to answer with that dataset.

## Store them for loading

Create a list of dictionaries in `datasets.py`, so that there is one dictionary for each dataset with the url, a name, and what function should be used to load the data into a `pandas.DataFrame`.

````{margin}
```{tip}
Urls are strings. The `string` class in python has a lot of helpful methods for manipulating strings, like [`split`](https://docs.python.org/3/library/stdtypes.html#str.split).
```
````


## Make a dataset about your datasets

Import the list fomr the `datasets` module you created in the step above.
Then terate over the list of dictionaries, and:  

1. save it to a local csv using the short name you provided for the dataset as the file name, without writing the index column to the file.
1. record attributes about the dataset as in the table below in a list of lists:
1. Use that to create a DataFrame with the following columns:

```{list-table} Meta Data Description of the DataFrame to build
:header-rows:0

* - name
  - a short name for the dataset
* - source
  - a url to where you found the data
* - num_rows
  - number of rows in the dataset
* - num_columns
  - number of columns in the dataset
* - num_numerical
  - number of numerical variables in the dataset
```

## Manipulate your datasets

For one dataset that includes nonnumerical data:
- display the heading and the last 4 rows
- make and display a new data frame with only the numerical columns (select these programmatically)


For any other dataset:
- display the heading and the first three rows
- display the datatype for each column
- Are there any variables where pandas may have read in the data as a datatype that's not what you expect (eg a numerical column mistaken for strings)? If so, investigate and try to figure out why.

For the third dataset:
- display the first 3 odd rows (eg 1,3,5) of the data for two columns of your choice


## Exploring data files

For each dataset, in a separate section of your notebook titled `When things go wrong`:
- try reading in data with the wrong `read_` function and make notes about what happens.
- was the format that the data was provided in a good format? why or why not?
- try to read in the `.csv` file that's included in the template repository (), use the error messages you get to try to fix the file manualy (any text editor, including jupyter can edit a `.csv`), making notes about what changes you made in a markdown cell.



## Thinking ahead

```{warning}
his section is not required, but is intended to help you get started thinking
about ideas for your portflio.  If you complete it, we'll give your feedback to
help shape your ideas to get to level 3 achievements.  If you want to focus only
on level 2 at this moment in time, feel free to skip this part.
```


1. When might you prefer one datatype over another?
1. How does PEP 8 standard code help you be collaborative?
1. Learn about [Datasheets for Datasets](https://arxiv.org/pdf/1803.09010.pdf) eg this [google scholar result](https://scholar.google.com/scholar?q=datasheets+for+datasets&hl=en&as_sdt=0&as_vis=1&oi=scholart) How could something like this impact your work as a datascientist?
