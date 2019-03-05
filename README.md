# Bokeh
Interactive data visualization library in Python, similar to matplotlib and seaborn

Sample Code to create a basic Bokeh line graph:

```python

#Importing bokeh

from bokeh.plotting import figure
from bokeh.io import output_file, show

#Prepare some data

x = [1, 2, 3, 4, 5]
y = [6, 7, 8, 9, 10]

#Prepare the output file

output_file("Line.html")
f = figure()

#Create a line plot

f.line(x,y)

show(f)
```

Sample Code to create a basic Bokeh line graph from a csv file using the Pandas library:

```python

from bokeh.plotting import figure
from bokeh.io import output_file, show
import pandas

df = pandas.read_csv("data.csv")

x = df["x"]
y = df["y"]

output_file("line_from_csv.html")

f = figure()

f.line(x,y)

show(f)
```
