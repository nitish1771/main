import pandas as pd
import numpy as np
df = pd.read_csv('Bank_Copy.csv')
df1 = pd.read_csv('Bank_Copy_1.csv')
df_all = pd.concat([df, df1])
k = df_all.style.hide_index()
k.to_excel('output.xlsx')
