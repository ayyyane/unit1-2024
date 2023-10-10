# quiz009

## prompt
<img width="1470" alt="quiz009" src="https://github.com/ayyyane/unit1-2024/assets/142702159/1cbdb485-319e-484f-b523-8b37f22c2a5f">

## flawchart
<img width="486" alt="Screenshot 2023-10-10 at 15 40 15" src="https://github.com/ayyyane/unit1-2024/assets/142702159/cd7fa9f1-a66e-4a20-99e5-c6c4d73418a3">

## solution
```.py
def powers_ten(s:int) -> str:
    num = s.split(" ")[0]
    unit = " ".join(s.split()[1:])
    prefixes = ['tera', 'giga', 'mega', 'kilo', '', 'milli', 'micro', 'nano', 'pico']
    powers = [12, 9, 6, 3, 0, -3, -6, -9, -12]
    out = []
    count = 8
    for power in powers:
        if power < 0:
            temp = f"0.{('000 ' * (abs(power) // 3))[:-2]}{num}"
        elif power > 0:
            temp = f"{num}{' 000' * (abs(power) // 3)}"
        else:
            temp = num
        temp = temp.ljust(20)
        out.append(f"{temp}{prefixes[count]}{unit}")
        count -= 1
    return "\n".join(out)

print(powers_ten(input("input the number:")))
```

## evidence
<img width="763" alt="Screenshot 2023-10-10 at 8 29 32" src="https://github.com/ayyyane/unit1-2024/assets/142702159/f1acdf42-8ff1-41c3-bc9c-7446382840a6">
