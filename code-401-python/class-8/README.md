# pandas

## Object creation



Creating a `Series` by passing a list of values, letting pandas create a default integer index:

```
In [3]: s = pd.Series([1, 3, 5, np.nan, 6, 8])
In [4]: s
Out[4]: 
0    1.0
1    3.0
2    5.0
3    NaN
4    6.0
5    8.0
dtype: float64
```

Creating a `DataFrame` by passing a NumPy array, with a datetime index and labeled columns:

```
In [5]: dates = pd.date_range("20130101", periods=6)
In [6]: dates
Out[6]: 
DatetimeIndex(['2013-01-01', '2013-01-02', '2013-01-03', '2013-01-04',
               '2013-01-05', '2013-01-06'],
              dtype='datetime64[ns]', freq='D')
In [7]: df = pd.DataFrame(np.random.randn(6, 4), index=dates, columns=list("ABCD"))
In [8]: df
Out[8]: 
                   A         B         C         D
2013-01-01  0.469112 -0.282863 -1.509059 -1.135632
2013-01-02  1.212112 -0.173215  0.119209 -1.044236
2013-01-03 -0.861849 -2.104569 -0.494929  1.071804
2013-01-04  0.721555 -0.706771 -1.039575  0.271860
2013-01-05 -0.424972  0.567020  0.276232 -1.087401
2013-01-06 -0.673690  0.113648 -1.478427  0.524988
```

## Viewing data

* Here is how to view the top and bottom rows of the frame:
  * ` df.head()`</br>
  * `df.tail(3)`

## Selection

**Getting**

* Selecting a single column, which yields a Series, equivalent to `df.A`:
  * ` df['A']`

* Selecting via [], which slices the rows.

  * ` df[0:3]`  

**Selection by label**

* For getting a cross section using a label:
  * `df.loc[dates[0]]`
  * ` df.loc[:, ['A', 'B']]`

**Selection by position**

* Select via the position of the passed integers:

  * ` df.iloc[3]`
  * `df.iloc[3:5, 0:2]`
  * `df.iloc[[1, 2, 4], [0, 2]]`

## Merge 

**Concat**

* Concatenating pandas objects together with concat():
  * `df = pd.DataFrame(np.random.randn(10, 4))`
  ` pieces = [df[:3], df[3:7], df[7:]]`
  `pd.concat(pieces)`

**Join**

* SQL style merges. See the Database style joining section.
    * ` left = pd.DataFrame({'key': ['foo', 'foo'], 'lval': [1, 2]})`
    ` right = pd.DataFrame({'key': ['foo', 'foo'], 'rval': [4, 5]})`
    `pd.merge(left, right, on='key')`

## Grouping

* By “group by” we are referring to a process involving one or more of the following steps:

  * **Splitting** the data into groups based on some criteria

  * **Applying** a function to each group independently

  * **Combining** the results into a data structure

## References
- https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html
- https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.html#pandas.Series
- https://pandas.pydata.org/pandas-docs/stable/user_guide/cookbook.html#cookbook
- https://pandas.pydata.org/pandas-docs/stable/user_guide/dsintro.html#dsintro
- https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html#pandas.DataFrame