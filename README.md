These commands are used with Pandas to draw graphs:-

*df.plot(kind='line') → draws a line graph

*df.plot(kind='bar') → vertical bar graph

*df.plot(kind='barh') → horizontal bar graph

*df.plot(kind='hist') → shows how data is distributed

*df.plot(kind='box') → shows data range using box plot

*df.plot(kind='kde') → smooth curve showing data density

*df.plot(kind='pie', y='col') → pie chart from one column

*df.plot.scatter(x='c1', y='c2') → scatter plot (dots)

*df.plot(kind='area') → area filled under the line

 *Line Plot  
A line plot is used to show trends over time.  
In this example, we plot monthly sales data.

import pandas as pd
import matplotlib.pyplot as plt
df = pd.DataFrame({
    'Month': ['Jan','Feb','Mar','Apr','May'],
    'Sales': [200, 250, 300, 280, 350]
})
df.plot(kind='line', x='Month', y='Sales', title='Monthly Sales Trend')
plt.show()

 . Scatter Plot :
A scatter plot shows the relationship between two variables.  
We compare Height vs Weight of individuals.
