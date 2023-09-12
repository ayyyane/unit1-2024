# quiz001

## test
![quiz001](https://github.com/ayyyane/unit1-2024/assets/142702159/654e3bb7-ecf2-48be-bb4f-488df874548d)
*fig.1* **screenshot of quiz slides**

## Soluition Overview
```.py
def black_box(user_input:str) -> str:
  strings = user_input.split(' ')
  output= ''

for word in strings:
  if len(word) <= 2:
      output += word + ' '
  else:
    output += word[0] + str(len(word) - 2) + word[-1] + ' '

return output

# check if it works:
print(black_box("internationalization"))
print(black_box("localization"))
print(black_box("Hello world!"))
print(black_box("98 99 100 101 1062"))
print(black_box("(codin) + (game) = (codingame)"))
```

## Evidence
<img width="985" alt="quiz001 e" src="https://github.com/ayyyane/unit1-2024/assets/142702159/f8d0b444-94fa-48b3-b269-2ca6e9ff0011">
*fig.2 **screenshot of output in console
