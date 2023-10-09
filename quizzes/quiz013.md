# quiz013

## prompt
<img width="1470" alt="quiz013" src="https://github.com/ayyyane/unit1-2024/assets/142702159/34cb2975-79a7-481a-8fb6-5beedbfa6c2f">

## solution
```.py
def mystery_box3(given:str)->str:
    counts = []
    alpha = 'abcdefghijklmnopqrstuvwxyz'
    output = " "
    for x in range(26):
        counts.append(0)
    for letter in given:
        if letter == " ":
            output += " "
        for i in range(26):
             if letter == alpha[i]:
                counts[i] += 1
                output += str(counts[i])
    return output


print(mystery_box3("hello world"))
print(mystery_box3("aaaaAABB"))
print(mystery_box3("abABabAB"))
print(mystery_box3("Create a function"))
```
## evidence
<img width="902" alt="Screenshot 2023-10-09 at 20 26 12" src="https://github.com/ayyyane/unit1-2024/assets/142702159/e4077655-a19a-41cc-a2ee-d4be0efb7b33">

