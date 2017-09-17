import matplotlib.pyplot as plt

%matplotlib inline

```python
# 放大系数
f = 3
# 横坐标
t = np.linspace(0,2,100)  # 注意没有e！！！
y = np.sin(2*np.pi*f*t)

# 可以有多个plot画在一起
plt.plot(t,y)

#一些属性
# o表示用圈圈画图（默认为线），或者用scatter函数
# 颜色：r红  b蓝，y黄
plt.plot(t,y,'or’)
# 用线画图
plt.plot(xplt,yplt,'-',linewidth=3)


# 网格线，两种效果一样
plt.grid()
plt.grid(True)

plt.xlabel('给横坐标起名字', fontsize=16)
plt.ylabel('sin(2pi ft)', fontsize=16)

# 画斜率为1的分割线
plt.plot([0,350],[0,350],'r')

# 画散点图，传入两个长度相等的一维数组
plt.scatter(y_test,y_test_pred)

# legend
属性：label='current data'
plt.legend()

# 设置图形大小
plt.figure(figsize=(10,5))
plt.figure(1) 
```

