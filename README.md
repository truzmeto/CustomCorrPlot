

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
