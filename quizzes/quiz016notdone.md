# quiz016

## prompt
<img width="1470" alt="Screenshot 2023-10-09 at 20 11 40 1" src="https://github.com/ayyyane/unit1-2024/assets/142702159/ca74867a-505c-4328-b8e0-4b22ef70e6fe">

## solution
```.py
def averageletter(word:list)->float:
    char = 0
    num_l = 0
    for l in word:
        num_l +=1
        for w in l:
            char += 1

    return char/num_l
print(averageletter(["hello", "main"]))
print(averageletter(["Peru", "France", "Nepal"]))
print(averageletter(["computer science", "art"]))
print(averageletter(["one", "two"]))


```

## evodence
<img width="778" alt="Screenshot 2023-10-10 at 8 54 21" src="https://github.com/ayyyane/unit1-2024/assets/142702159/82b28373-a9f5-4e55-a727-3fb2d2e9c19e">

