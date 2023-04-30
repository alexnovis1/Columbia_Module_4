# Analyzing Portfolio Risk and Return

---

## Introduction 

The python script reads in a timestamp csv file filled with four different investment funds (Soros Fund Managment, Paulson & Co Inc., Tiger Global Management, and Berkshire Hathaway) and the S&P 500 closing prices within the time range of 10/01/2014 to 09/11/2020. Using this imported data, the script will be able to determine the portfolio risk of all funds, as well as, determine the best return. 

---

## Folders 

[Example CSV File](Columbia_Module_4/Resources/whale_navs.csv)

[Risk Return Analysis Python Script](Columbia_Module_4/risk_return_analysis.ipynb)

---

## Resources

The script uses Python 3.7. The code will import the following libraries and dependencies: Pandas, Numpy, Pathlib, and Matplotlib.

```python
import pandas as pd
import numpy as np
from pathlib import Path 
%matplotlib inline
```

[For more information on Pandas](https://pandas.pydata.org/)

[For more information on Numpy](https://numpy.org/)

[For more infomration on Pathlib](https://docs.python.org/3/library/pathlib.html)

[For more information on Matplotlib](https://matplotlib.org/)

---

## Usage

After reading the csv file, using `pd.read_csv()`, the script calculates the daily returns by using the `pct_change()` function and then `dropna` to find teh daily returns of the four funds and S&P 500. 

```python 
whale_navs_daily_returns = whale_navs.pct_change().dropna()
```

The script goes one step further, by isolating the daily returns by each fund and S&P 500 to have more control over visualization tactics. Using the Soros Management Fund as an example: 

```python
daily_return_soros = whale_navs.iloc[:,0].pct_change().dropna()
```
