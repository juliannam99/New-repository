# New-repository


here we are, I missed this step and just clicked finish

import pandas as pd
import numpy as np
import matplotlib.pyplot as plt

df = pd.read_csv('https://raw.githubusercontent.com/CSSEGISandData/COVID-19/master/csse_covid_19_data/csse_covid_19_time_series/time_series_covid19_confirmed_US.csv')

plt.title('New reported cases')
plt.xlabel('Days since Jan 22, 2020')
plt.ylabel('Cases')
plt.grid(True, which='major')
plt.plot(np.diff(df.sum()[10:]))
