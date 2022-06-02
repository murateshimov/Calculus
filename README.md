# Calculus II 
Porgram plots function using python library matplotlib 
```python 
import numpy as np
import matplotlib.pyplot as plt

def f(x,a,b,c):
    return a*x**2+b*x+c

xlist = np.linspace(-10,10,num=1000)

a,b,c=5,1,4
ylist = f(xlist,a,b,c)

plt.figure(num=0,dpi=120)
plt.plot(xlist,ylist,label="f(x)")
plt.plot(xlist,ylist**(1/2),'--g',label=r"f(x)$^{0.5}$")
plt.title("Calculus II")
plt.xlabel("Distance / ft")
plt.ylabel("Height / ft")
plt.legend()
plt.show()
```
![](graph%20of%20function%20.png)
