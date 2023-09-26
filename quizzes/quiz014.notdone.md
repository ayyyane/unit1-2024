# quiz014

## prompt

## solution
```.py

def mystery_box4(given:str)-> str:
  count = []
  alpha = 'abcdefghijklmnopqrstuvwxyz'
  output = " "
  for i in range(26):
    count.append(0)
  for letter in given:
    if letter == " ":
      output += " "
    for x in range (26):
      if letter == alpha[i]:
        count[i] += 1
        output += str(count[i])
    return output

print(mystery_box4("hello world"))
print(mystery_box4("aaaaAABB"))
print(mystery_box4("abABabAB"))
print(mystery_box4("Create a function"))




```

## evidence
<img width="1470" alt="quiz014_e" src="https://github.com/ayyyane/unit1-2024/assets/142702159/ac1ab343-40be-4cea-9de3-428d9d8a5285">
