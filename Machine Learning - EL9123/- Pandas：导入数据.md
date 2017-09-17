```python
import pandas as pd

names = ['mpg', 'cylinders','displacement', 'horsepower', 
         'weight', 'acceleration', 'model year', 'origin', 'car name’]

df = pd.read_csv('https://archive.ics.uci.edu/ml/machine-learning-databases/'+
                 'auto-mpg/auto-mpg.data',
                 header=None,delim_whitespace=True,names=names,na_values='?’)
# 查看前六行
df.head(6)

# 一些属性
# 返回（行数，列数）
df.shape
# 返回列名
df.columns
df.columns.tolist()
# 返回行数索引
df.index
# 返回每行的数据
df.values

# 选取其中某些列
df2 = df[['cylinders','horsepower']]
# 转化成数组
y = np.array(df['mpg'])
# 转化成多维数组,注意这里要用两层[[]]包起来！不知道为啥
y = np.array(df[['mpg','xxx']])
```