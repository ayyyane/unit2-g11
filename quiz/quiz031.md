# quiz031

## prompt

## solution

```.py
import requests
from gomi4 import get_sensor
import matplotlib.pyplot as plt

s1 = get_sensor(id=1)
s2 = get_sensor(id=2)

sum = []
for x in range(0,len(s1)):
    sum.append(s1[x]+s2[x])
    x += 1

plt.subplot(3,1,1) # (howmany,列,何こめ)
plt.plot(s1)
plt.subplot(3,1,2)
plt.plot(s2)
plt.subplot(3,1,3)
plt.plot(sum)
plt.show()
```

## evidence
<img width="574" alt="Screenshot 2023-11-30 at 10 34 46" src="https://github.com/ayyyane/unit2_g11/assets/142702159/3bc4f7bc-0b0a-40fd-9b97-3d6d7a430a48">
