1. Import Libraries

```
import pandas as pd
import seaborn as sns
import numpy as np
import matplotlib.pyplot as plt
%matplotlib inline

import warnings
warnings.filterwarnings('ignore')

plt.rcParams['figure.figsize'] = (20,20)
plt.rcParams['figure.dpi'] = 1000
pd.options.display.max_rows = 200
```
2. Import Dataset
```

df0 = pd.read_csv('Fortune500.csv')
df = df0.copy()
df.head()
```
|index|rank|company|revenue|profit|num\. of employees|sector|city|state|website|
|---|---|---|---|---|---|---|---|---|---|
|0|1|Walmart|523964\.0|14881\.0|2200000|Retailing|Bentonville|AR|https://www\.stock\.walmart\.com|
|1|2|Amazon|280522\.0|11588\.0|798000|Retailing|Seattle|WA|https://www\.amazon\.com|
|2|3|Exxon Mobil|264938\.0|14340\.0|74900|Energy|Irving|TX|https://www\.exxonmobil\.com|
|3|4|Apple|260174\.0|55256\.0|137000|Technology|Cupertino|CA|https://www\.apple\.com|
|4|5|CVS Health|256776\.0|6634\.0|290000|Health Care|Woonsocket|RI|https://www\.cvshealth\.com|

3. Data Preparation
```
df.info() # no null, great
```
![Screen Shot 2022-08-22 at 6 53 03 PM](https://user-images.githubusercontent.com/108639250/186032562-2803f852-791d-4080-819f-43c5147df4d3.png)

4. Search for NaN
```
df.isna() # no NaN
```
|index|rank|company|revenue|profit|num\. of employees|sector|city|state|website|
|---|---|---|---|---|---|---|---|---|---|
|0|false|false|false|false|false|false|false|false|false|
|1|false|false|false|false|false|false|false|false|false|
|2|false|false|false|false|false|false|false|false|false|
|496|false|false|false|false|false|false|false|false|false|
|497|false|false|false|false|false|false|false|false|false|
|498|false|false|false|false|false|false|false|false|false|
|499|false|false|false|false|false|false|false|false|false|
