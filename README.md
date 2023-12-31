# Implementation of Univariate Linear Regression
## Aim:
To implement univariate Linear Regression to fit a straight line using least squares.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
![Screenshot 2023-12-31 144239](https://github.com/PremkumarG3/Univariate-Linear-Regression/assets/138955646/6288b6e7-95fd-4e63-a9bb-dc3a63f3dce0)
## Program
```
# Univariate Linear Regression
# Develpoed by:PREM KUMAR G
# Register number:23003614
import numpy as np
import matplotlib.pyplot as plt x=np.array([0,1,2,3,4,5,6,7,8,9])
y=np.array([1,3,2,5,7,8,8,9,10,12])
plt.scatter(x,y)
plt.show()
xmean=np.mean(x)
ymean=np.mean(y)
num=0
den=0
for i in range(len(x)):
num+=(x[i]-xmean)*(y[i]-ymean)
den+=(x[i]-xmean) **2
m=num/den
b=ymean-m*xmean
print(m,b)
ypred=m*x+b
print(ypred)
plt.scatter(x,y,color="Red")
plt.plot(x,ypred, color="Blue")
plt.show()
```
## Output
![WhatsApp Image 2023-12-28 at 23 32 24_a9aaf394](https://github.com/PremkumarG3/Univariate-Linear-Regression/assets/138955646/b02689f9-6878-4853-8477-69ccb39bdfe6)
![WhatsApp Image 2023-12-28 at 23 29 32_949ae0fe](https://github.com/PremkumarG3/Univariate-Linear-Regression/assets/138955646/0e13d1d4-0c06-46b1-b966-adaf48d2a38d)
## Result
Thus the univariate Linear Regression was implemented to fit a straight line using least squares.
