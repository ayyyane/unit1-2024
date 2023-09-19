# quiz 010
<img width="1470" alt="quiz010" src="https://github.com/ayyyane/unit1-2024/assets/142702159/1ab6bdca-be4a-4f61-81a9-e99a4dfb888f">

# solution
```.py
calender=''
days = ['Fr', 'Sa', 'Su', 'Mo', 'Tu', 'We', 'Th']
for d in range(1,31):
    day = days[d%7-1]
    calender += f"{day} {d} ".center(8)
    if d %7 == 0:
        calender += "\n"

print(calender)
```

# evidence
<img width="1052" alt="quiz010_e" src="https://github.com/ayyyane/unit1-2024/assets/142702159/23c1ffb3-3fa1-4030-af83-aab470dd4540">
