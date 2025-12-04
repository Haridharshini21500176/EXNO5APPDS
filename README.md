# EXNO5APPDS

# AIM:

      To implement Dashboards creation with Plotly and Dash using python.
      

# About Dash and Plotly tools:

Dash is a Python framework for building analytical web applications. Dash helps in building responsive web dashboards that is good to look at and is very fast without the need to understand complex front-end frameworks or languages such as HTML, CSS, JavaScript. Let’s build our first web dashboard using Dash.

Plotly library in Python is an open-source library that can be used for data visualization and understanding data simply and easily. Plotly supports various types of plots like line charts, scatter plots, histograms, box plots, etc.


# ALGORITHM:

Step 1: Import Necessary Library like dash and plotly.

Step 2: Load the dataset.

Step 3: Add dropdown using layout function and include the necessary options.

Step 4: Display the necessary visualization tools and include the necessary parameters.

Step 5: Display the output.


# CODING AND OUTPUT:
```
Developed By: Haridharshini S
Register No : 212221230033
```
```
pip install dash plotly pandas
import dash
from dash import dcc, html
from dash.dependencies import Input,Output
import plotly.express as px
import pandas as pd
import plotly.graph_objects as px
import numpy as np
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt
df = sns.load_dataset('tips')
```
```
plot=px.Figure(data=[px.Scatter(x=df['day'],y=df['tip'],mode='markers')])
plot.update_layout(updatemenus=[dict(buttons=list([dict(args=["type","scatter"],label="Scatter Plot",method="restyle"),dict(args=["type","bar"],label="Bar Chart",method="restyle")]),direction="down",)])
plot.show()
```
```
import plotly.express as px
df=px.data.tips()fig = px.scatter_3d(df, x="total_bill",y="sex",z="tip",color='day',size='total_bill',symbol='time')
fig.show()
```
```
import plotly.express as px
df=px.data.tips()
fig = px.bar(df, x='day',y='total_bill',color='sex',facet_row='time',facet_col='sex')
fig.show()
```
```
import plotly.express as px
df=px.data.tips()
fig = px.histogram(df, x='total_bill',color='sex',nbins=50,histnorm='percent',barmode='overlay')
fig.show()
```
```
import plotly.express as px
df=px.data.tips()
fig = px.pie(df, values='total_bill',names='day')
fig.show()
```
## OUTPUT
![Screenshot 2024-11-27 185537](https://github.com/user-attachments/assets/0a0987ce-9435-4e5e-9f0b-3a86f2611345)
![Screenshot 2024-11-27 185606](https://github.com/user-attachments/assets/3bce83f6-c2fc-4840-ae5d-3c505b9fa76e)
![Screenshot 2024-11-27 185631](https://github.com/user-attachments/assets/b3c3c629-4358-4dd3-b1fc-2cbbb6a54c88)
![Screenshot 2024-11-27 185701](https://github.com/user-attachments/assets/bf7d47fa-05f0-4bb3-b56a-257044011ec1)
![Screenshot 2024-11-27 185726](https://github.com/user-attachments/assets/fc91df9a-18a3-471b-9fde-f3b53af04bde)
![Screenshot 2024-11-27 185749](https://github.com/user-attachments/assets/312f4fd8-67a3-41ab-815b-a33ae398442e)
![Screenshot 2024-11-27 185813](https://github.com/user-attachments/assets/16cd414b-135f-4555-a8dd-243e025229c2)


# RESULT:
Thus , To implement Dashboards creation with Plotly and Dash using python is successfully done.



