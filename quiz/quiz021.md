# quiz021

## prompt
![Screen Shot 2023-11-19 at 19 41 39](https://github.com/ayyyane/unit2_g11/assets/142702159/8f0888a0-d983-4dd9-b618-d2cb6b72e3a7)

## solution
```.py
import random
import matplotlib.pyplot as plt
def graph_maker(n,m,s):
    x = []
    y = []
    for i in range(n):
        x_rnd = random.randint(0, 100)
        y_rnd = x_rnd ** (0.5 * (m / s) ** 2)
        y.append(y_rnd)
        x.append(x_rnd)
    return x,y



x,y = graph_maker(n=5,m=3,s=2)
fig = plt.figure(figsize=(9,7))
plt.plot(x,y)
plt.title("$y =x^{(1/2)(s/m)^2}$")
plt.show()

```

## evidnece
<img width="819" alt="Screenshot 2023-11-23 at 15 31 29" src="https://github.com/ayyyane/unit2_g11/assets/142702159/7e0483ec-98c7-4a68-9c8a-dfe57a750c0e">


## truth table
![IMG_1085](https://github.com/ayyyane/unit2_g11/assets/142702159/eb0edcf2-40fd-4a16-b8cf-f7a070b153a9)
