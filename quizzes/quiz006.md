# quiz006

## prompt
<img width="1470" alt="quiz006" src="https://github.com/ayyyane/unit1-2024/assets/142702159/63431e86-5076-469d-932c-aaa30dd9168f">


## solution

'''.py

def room_checker(num:int)->str:
  for num in range(1,101):
    if num/10 == 0:
      floor = num//10
    else:
      floor = num//10+1
print(f"{num}-Room {Floor}F{num%10:02d}")



```
