# quiz023

## prompt
![Screen Shot 2023-11-19 at 19 41 44](https://github.com/ayyyane/unit2_g11/assets/142702159/adc4ec6b-3e24-43cb-aabc-88d1360ee5b7)

## solution
```.py
def graph_maker():
    x = []
    y = []
    for i in range(-10,11,1):
        x_rnd =i
        if x_rnd<0:
            y_rnd = -(x_rnd)
        else:
            y_rnd = x_rnd
        x.append(x_rnd)
        y.append(y_rnd)

    fig = plt.figure(figsize=(9,7))
    plt.plot(x,y,linewidth = 2)
    plt.title("$y = |x| $")
    plt.xlabel("x")
    plt.ylabel("$y = |x| $")
    plt.show()

print(graph_maker())

```
## evidence
<img width="778" alt="Screenshot 2023-11-23 at 16 56 54" src="https://github.com/ayyyane/unit2_g11/assets/142702159/70b6903f-0510-4436-b05d-ad7ab61a6cfe">

## decimal
![IMG_1087](https://github.com/ayyyane/unit2_g11/assets/142702159/0d91c0d8-727a-4c39-b50c-d13ebc5ced0a)
