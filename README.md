# Analyzing Portfolio Risk and Return

---

## Introduction 

The python script reads in a timestamp csv file filled with four different investment funds (Soros Fund Managment, Paulson & Co Inc., Tiger Global Management, and Berkshire Hathaway) and the S&P 500 closing prices within the time range of 10/01/2014 to 09/11/2020. Using this imported data, the script will be able to determine the portfolio risk of all funds, as well as, determine the best return. 

---

## Folders 

[Example CSV File]("Columbia_Module_4/Resources/whale_navs.csv")

[Risk Return Analysis Python Script]("Columbia_Module_4/risk_return_analysis.ipynb")

---

## Resources

The code will import the following libraries and dependencies: Pandas, Numpy, Pathlib, and Matplotlib.

"""python
import pandas as pd
import numpy as np
from pathlib import Path 
%matplotlib inline
"""

