# quiz024

## prompt
![Screen Shot 2023-11-19 at 19 41 46](https://github.com/ayyyane/unit2_g11/assets/142702159/a7b830b0-006e-45cf-9876-015b66bb8307)

## solution
```.py
import matplotlib.pyplot as plt
import numpy as np

humidity = [57.0, 56.0, 57.0, 56.0, 55.0, 55.0, 54.0, 54.0, 54.0, 53.0, 53.0, 54.0, 53.0, 53.0, 52.0, 52.0, 51.0, 51.0, 51.0, 50.0, 50.0, 49.0, 50.0, 49.0, 49.0, 48.0,
            49.0, 49.0, 48.0, 48.0, 48.0, 49.0]
time = []

t = 0
for x in range(len(humidity)):
    time.append(t)
    t += 10

# scatter plot
plt.scatter(time,humidity,color = "blue") # scatter is for 散布図 scatter plot
plt.xlabel("Time(min)")
plt.ylabel("Humidity(%)")

m,b = np.polyfit(time,humidity,1) # np.polyfit(x-axis,y-axis,a) x^a
print(f"Linear model h(t) = {m:.2f}t+{b:2f}")

# graph
time_model = []
humidity_model = []
t = 0
for i in range(len(humidity)):
    time_model.append(t)
    humidity_model.append(m*t+b)
    t += 10

plt.plot(time_model,humidity_model)
plt.text(80,50,f"h(t)={m:.2f}t+{b:.2f}", fontsize = 10)
plt.show()


```

## evidence
<img width="628" alt="Screenshot 2023-11-23 at 17 29 00" src="https://github.com/ayyyane/unit2_g11/assets/142702159/ee57a79f-35fc-479f-9c0f-c15e079e1a11">


## convert
![IMG_5302 copy](https://github.com/ayyyane/unit2_g11/assets/142702159/d011d5ed-7948-4f08-80e0-d8a0b05f1efe)
