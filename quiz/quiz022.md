# quiz022

# prompt

![Screen Shot 2023-11-19 at 19 41 42](https://github.com/ayyyane/unit2_g11/assets/142702159/d9f56fdb-cd44-4157-a3f0-a1a09b99b524)

## solution

```.py
from matplotlib import pyplot as plt

def graph_maker():
    x = []
    y = []
    for n in range(-10,11,1):
        x.append(n)
        y.append(2*(n+5)**2)

    fig = plt.figure(figsize = (9,7))
    plt.plot(x,y,linewidth = 2)
    plt.title("graph of the equation $y = 2(x+5)^2$")
    plt.xlabel("X")
    plt.ylabel("$f(x) = 2(x+5)^2$")
    plt.show()

print(graph_maker())
```

## evidence
<img width="847" alt="Screenshot 2023-11-23 at 15 16 02" src="https://github.com/ayyyane/unit2_g11/assets/142702159/b9502060-9660-4c37-b224-e9329380f6b5">

## circuit
![IMG_1086](https://github.com/ayyyane/unit2_g11/assets/142702159/45d2d44a-9577-4ee8-a4d4-6640110b986d)
