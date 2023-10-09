# quiz015

## propmpt
<img width="1470" alt="quiz015" src="https://github.com/ayyyane/unit1-2024/assets/142702159/60cb97c8-ef53-4b51-9512-796eaecda2ab">

## solution
```.py
def opendoor(num_students:int)->int:
    counts = []
    for i in range(num_students):
        counts.append(False)
    for x in range(num_students):
        for i in range(x,num_students,x+1):
            counts[i] = not counts[i]
    return counts.count(True)

print(opendoor(10))
print(opendoor(100))
print(opendoor(200))
print(opendoor(5678))
```


## evidence

![Uploading Screenshot 2023-10-10 at 8.21.56.png…]()
