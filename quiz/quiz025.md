# quiz025

## prompt
<img width="1470" alt="25" src="https://github.com/ayyyane/unit2_g11/assets/142702159/3bd8af0f-e1f4-42eb-9c7f-c5c5f4edc96a">

## solution
```.py
import matplotlib.pyplot as plt
import numpy as np

def error_bar(sensorA:list,sensorB:list,sensorC:list):
    x = list(range(1,len(sensorA)+1))
    mean = []
    std = []
    min = []
    max = []

    for i in range(len(sensorA)):
        data = [sensorA[i], sensorB[i], sensorC[i]]
        mean.append(np.mean(data))
        std.append(np.std(data))
        min.append(np.min(data))
        max.append(np.max(data))

    plt.fill_between(x,max,min,alpha=0.5, linewidth=0, color="#8ecae6")
    plt.errorbar(x,mean,std,fmt="o")
    # why does this circle exist one in each value?
    plt.show()

A = [16,24,24,9,23,26,26,23,25,14]
B = [2,19,25,10,11,24,17,7,24,17]
C = [15,11,24,21,6,2,18,27,1,16]
error_bar(A,B,C)

```

## evidnece
<img width="601" alt="quiz025 ev" src="https://github.com/ayyyane/unit2_g11/assets/142702159/53ce52c1-d87e-4118-aed5-6a88f2fe7c6a">


## convert

![IMG_1137](https://github.com/ayyyane/unit2_g11/assets/142702159/1171b991-2af8-4d32-ac14-620851eab804)
