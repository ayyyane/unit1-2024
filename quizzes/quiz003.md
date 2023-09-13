# quiz003

## prompt
![quiz003](https://github.com/ayyyane/unit1-2024/assets/142702159/9f10e8b6-f5a8-4d67-8f61-4d951727dbbf)
* fig.2* **screenshot of quiz slides**

## solution

```.py
def convert_protein(in_protein:str)-> str:
  out_protein = ''
  for letter in in_protein:
    if letter == "A":
      out_protein += "T"
    elif letter == "G":
      out_protein += "C"
    elif letter == "T":
      out_protein += "A"
    elif letter == "C":
      out_protein += "G"
    else:
      return "Error: unknown letter in protein string"
```

# check if it works:
print(convert_protein("A"))
print(convert_protein("G"))
print(convert_protein("C"))
print(convert_protein("T"))
print(convert_protein("AGCT"))


## Evidence
<img width="794" alt="quiz003_e" src="https://github.com/ayyyane/unit1-2024/assets/142702159/c9cd20a2-7dd8-4d2b-8ae6-b14ba503323d">

            
