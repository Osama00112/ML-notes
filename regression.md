### 3. Regression

#### linear regression

simple:
``y = b0 + b1*x``


#### fitting simple regression
```python
from sklearn.linear_model import LinearRegression
regressor = LinearRegression()
regressor.fit(X_train,y_train)
```

#### predicting our observed test set
```python
y_pred = regressor.predict(X_test)
```

#### plotting train sets and best fit
```python
plt.scatter(X_train,y_train, color = 'red')
plt.plot(X_train,regressor.predict(X_train), color= 'blue')
plt.title('salary vs Exp(training set)')
plt.xlabel('years of exp')
plt.ylabel('salaries')
plt.show()
```
![image](https://user-images.githubusercontent.com/54764108/164254946-c3998f91-d399-40b9-9648-d7327f320118.png)


#### comparing with test sets 
```python
plt.scatter(X_test,y_test, color = 'red')
plt.plot(X_train,regressor.predict(X_train), color= 'blue')
plt.title('salary vs Exp(training set)')
plt.xlabel('years of exp')
plt.ylabel('salaries')
plt.show()
```

![image](https://user-images.githubusercontent.com/54764108/164254991-4c9c1561-7ab3-4d5f-9a8b-d3583b8e89d1.png)
