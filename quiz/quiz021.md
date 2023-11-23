# quiz021

## prompt
![Screen Shot 2023-11-19 at 19 41 39](https://github.com/ayyyane/unit2_g11/assets/142702159/8f0888a0-d983-4dd9-b618-d2cb6b72e3a7)

## solution
```.py
import matplotlib.pyplot as plt

# we want to graph y = x^3 from x = [-15,15]
x= []
y = []
for n in range(-15,15,1):
    x.append(n)
    y.append(n**3)

fig = plt.figure(figsize = (9,7))
# size of the graph
plt.plot(x,y,linewidth = 2)
plt.title("graph of the equation $y = x^3$")
# $ x**3をクリアにするため
plt.xlabel("x",fontsize=18)
plt.ylabel("y",fontsize = 18)
plt.show()

```

## evidnece
<img width="874" alt="Screenshot 2023-11-23 at 14 55 57" src="https://github.com/ayyyane/unit2_g11/assets/142702159/917ed957-f600-42c2-b82f-4b378f96dd26">

