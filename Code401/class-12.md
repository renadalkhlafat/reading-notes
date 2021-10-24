# Pandas
**pandas** is an open source data analysis and manipulation tool,
built on top of the Python programming language.

**Example:** 
```python 
import pandas as pd
```

## Object creation
 
**Example:** 
```python 
import pandas as pd

s = pd.Series([1, 3, 5, np.nan, 6, 8])

dates = pd.date_range("20130101", periods=6)

df2 = pd.DataFrame(
    {
        "A": 1.0,
        "B": pd.Timestamp("20130102"),
        "C": pd.Series(1, index=list(range(4)), dtype="float32"),
        "D": np.array([3] * 4, dtype="int32"),
        "E": pd.Categorical(["test", "train", "test", "train"]),
        "F": "foo",
    }
)
```

## Viewing data
+ df.head() ->view the top row
+ df.tail(3) -> view the bottom rows 
+ df.index -> Display the index
+ df.columns -> Display the colummns
+ df.to_numpy()
+ df.describe() ->  shows a quick statistic summary of your data

## Selection
ways to accessing data :
1.  .at
2.  .iat
3.  .loc
4.  .iloc

## Getting
* single column :
**Example:**  `df["A"]`
+ slicing : 
**Example:**`df[0:3]`

## Setting 
Setting a new column automatically aligns the data by the indexes.

**Example:** 
`df.at[dates[0], "A"] = 0`

## Grouping
By “group by” we are referring to a process involving one or more of the following steps:

+ Splitting the data into groups based on some criteria

+ Applying a function to each group independently

+ Combining the results into a data structure


`df.groupby("A").sum()`

## Merge
+ Concat 

```python
pieces = [df[:3], df[3:7], df[7:]]

pd.concat(pieces)
```

+ Join

``` jupyter
left = pd.DataFrame({"key": ["foo", "foo"], "lval": [1, 2]})

right = pd.DataFrame({"key": ["foo", "foo"], "rval": [4, 5]})

left
Out[79]: 
   key  lval
0  foo     1
1  foo     2

right
Out[80]: 
   key  rval
0  foo     4
1  foo     5

pd.merge(left, right, on="key")
```