# Bokeh
Interactive data visualization library in Python, similar to matplotlib and seaborn

Sample Code:

```python
#Creating a basic Bokeh line graph

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
