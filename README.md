
## Correlation Plot Visualization

Most of the known corr_plot functions take raw data as input in order to visualize
correlation matrix, which might be very time consuming with big data. Thus, I have decided
to make my one function that takes already prepared correlation matrix an makes visualization
very fast. In addition, code is very simple, one can easyly customize it based on need.

Function is built with matplotlib library under Python3.5. It takes corr. matrix as 2d np.array
and axis labels as list. 


```python
import pandas as pd
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline
```


```python
df = pd.read_csv("corr_mat_both")
df = round(df,2)
data =df.values
data = data.T
```


```python
from CorrPlot import CPlot
```


```python
fig = plt.figure(num=None, figsize=(8.636,7), facecolor='w')
CPlot(corr_mat = data, axis_labs = labels, cmap='PuBu', pad = 0.1, rad = 270)
```

![png](output_3_0.png)



```python

```
