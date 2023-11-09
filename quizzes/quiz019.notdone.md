## quiz019

## quiz019a

## prompt
<img width="1470" alt="Screenshot 2023-11-02 at 12 41 31" src="https://github.com/ayyyane/unit1-2024/assets/142702159/6b6d26f4-fdbe-4473-b352-77d826df8e8d">
*A = 1, B = 1 and C = 0 -> output: 1

## flowchart


## solution
```.py
def truth_table():
    a,b,c = 1,1,1
    ab = 0
    not_cb = 0
    ans = 0
    output = "| A | B | C | AB + not B + not CB|\n"
    for x in range(8):
        c = not c
        if x%2 == 0:
            b = not b
        if x%4 == 0:
            a = not a
        if int(a) == 1 and int(b) == 1:
            ab = 1
        else:
            ab = 0
        if int(b) == 1 and int(c) == 1:
            not_cb = 0
        else:
            not_cb = 1
        not_b = not b
        if not_b == 0 and ab == 0 and not_cb == 0:
            ans = 0
        else:
            ans = 1
        output += (f"| {int(a)} | {int(b)} | {int(c)} |         {ans}          |\n")
    return output

** test **
print(truth_table())


```

## evidence
<img width="700" alt="Screenshot 2023-11-07 at 17 36 17" src="https://github.com/ayyyane/unit1-2024/assets/142702159/ab7da4f9-3b25-41ba-ac8b-e09ccfc4957f">



## quiz019b

![IMG_1004](https://github.com/ayyyane/unit1-2024/assets/142702159/2e03a258-3b21-4083-b741-2b7476804826)
