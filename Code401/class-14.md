# Matplotlib
A package provides both a very quick way to visualize data from Python and publication-quality figures in many formats. We are going to explore matplotlib in interactive mode covering most common cases.

## pyplot
It's provides a convenient interface to the matplotlib object-oriented plotting library

```python
import numpy as np

X = np.linspace(-np.pi, np.pi, 256, endpoint=True)
C, S = np.cos(X), np.sin(X)

```

## Bokeh 
is an interactive visualization library that targets modern web browsers for presentation.

`from bokeh.io import output_notebook, show output_notebook()`

## Seaborn
a Python visualization library ,it is based on matplotlib and provides a high-level interface for drawing attractive statistical graphics.

```python
>>> import matplotlib.pyplot as plt
>>> import seaborn as sns
```

**Example** 
```python
tips = sns.load_dataset("tips")
g = sns.relplot(data=tips, x="total_bill", y="tip")
g.ax.axline(xy1=(10, 2), slope=.2, color="b", dashes=(5, 2))
```

![plot](https://seaborn.pydata.org/_images/function_overview_19_0.png)

## Customizing plots from a figure-level function

The figure-level functions return a FacetGrid instance, which has a few methods for customizing attributes of the plot in a way that is “smart” about the subplot organization

```python
g = sns.relplot(data=penguins, x="flipper_length_mm", y="bill_length_mm", col="sex")
g.set_axis_labels("Flipper length (mm)", "Bill length (mm)")
```
![xyz](https://seaborn.pydata.org/_images/function_overview_21_0.png)

## Combining multiple views on the data
Two important plotting functions in seaborn don’t fit cleanly into the classification scheme discussed above.

```python
sns.jointplot(data=penguins, x="flipper_length_mm", y="bill_length_mm", hue="species")
```
![dff](https://seaborn.pydata.org/_images/function_overview_38_0.png)