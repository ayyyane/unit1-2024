# quiz006

## prompt
![quiz006_a](https://github.com/ayyyane/unit1-2024/assets/142702159/35e4cf5b-27ea-4b0d-ad40-58586435568f)

## solution

'''.py

def room_checker(num:int)->str:
  for num in range(1,101):
    if num/10 == 0:
      floor = num//10
    else:
      floor = num//10+1
print(f"{num}-Room {Floor}F{num%10:02d}")
