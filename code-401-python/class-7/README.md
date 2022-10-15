### `matplotlib` : is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats.

## IPython and the pylab mode

[IPython](http://ipython.org/) is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, improved debugging and much more.

> When we start it with the command line argument `-pylab` (`--pylab` since IPython version 0.12), it allows interactive matplotlib sessions that have Matlab/Mathematica-like functionality.
## pyplot

`pyplot` is an object oriented plotting library, it is modeled closely to Matlab<sup>TM</sup>.

> The majority of plotting commands in `pyplot` have Matlab<sup>TM</sup> analogs with similar arguments. Important commands are explained with interactive examples.



## [NumPy Tutorial: Data Analysis with Python](https://www.dataquest.io/blog/numpy-tutorial-python/)

[NumPy](http://www.numpy.org/) is a commonly used Python data analysis package. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like [scikit-learn](http://scikit-learn.org/), that use NumPy under the hood. NumPy was originally developed in the mid 2000s, and arose from an even older package called Numeric. This longevity means that almost every data analysis or machine learning package for Python leverages NumPy in some way.

## Lists Of Lists for CSV Data

Before using NumPy, we’ll first try to work with the data using Python and the csv package. We can read in the file using the csv.reader object, which will allow us to read in and split up all the content from the ssv file.

In the below code, we:

Import the csv library.
Open the winequality-red.csv file.
With the file open, create a new csv.reader object.
Pass in the keyword argument delimiter=";" to make sure that the records are split up on the semicolon character instead of the default comma character.
Call the [list](https://docs.python.org/3/library/functions.html#func-list) type to get all the rows from the file.
Assign the result to wines.

```
import csv
with open('winequality-red.csv', 'r') as f:
    wines = list(csv.reader(f, delimiter=';'))
```

The below code will:

- Extract the last element from each row after the header row.
- Convert each extracted element to a float.
- Assign all the extracted elements to the list qualities.
- Divide the sum of all the elements in qualities by the total number of elements in qualities to the get the mean.

```
qualities =
[float(item[-1]) for item in wines[1:]]
sum(qualities) / len(qualities)
```
> Returned Value: `5.6360225140712945`
## Numpy 2-Dimensional Arrays

With NumPy, we work with multidimensional arrays. We’ll dive into all of the possible types of multidimensional arrays later on, but for now, we’ll focus on 2-dimensional arrays. A 2-dimensional array is also known as a matrix, and is something you should be familiar with. In fact, it’s just a different way of thinking about a list of lists. A matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.


## Creating A NumPy Array

We can create a NumPy array using the numpy.array function. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns. Because we want all of the elements in the array to be float elements for easy computation, we’ll leave off the header row, which contains strings. One of the limitations of NumPy is that all the elements in an array have to be of the same type, so if we include the header row, all the elements in the array will be read in as strings.

## Alternative NumPy Array Creation Methods

There are a variety of methods that you can use to create NumPy arrays. To start with, you can create an array where every element is zero. The below code will create an array with 3 rows and 4 columns, where every element is 0, using numpy.zeros :

import numpy as np
empty_array = np.zeros((3,4)) empty_array
It’s useful to create an array with all zero elements in cases when you need an array of fixed size, but don’t have any values for it yet.

You can also create an array where each element is a random number using numpy.random.rand .

## References


https://www.dataquest.io/blog/numpy-tutorial-python/