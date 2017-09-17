```python
# 导入一些包里含有的数据
diabetes = datasets.load_diabetes()
X = diabetes.data
y = diabetes.target

# 多元线性回归
regr = linear_model.LinearRegression()
regr.fit(X_tr,y_tr)
# 各个自变量的系数
regr.coef_
# 常数系数
regr.intercept_
y_tr_pred = regr.predict(X_tr)
```