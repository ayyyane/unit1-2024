# quiz017

## prompt
<img width="1470" alt="Screenshot 2023-10-25 at 16 16 13" src="https://github.com/ayyyane/unit1-2024/assets/142702159/508b3b9a-e538-470b-8951-db2d7a5aaafc">

# Question a
## flaw chart
<img width="257" alt="Screenshot 2023-10-25 at 16 39 01" src="https://github.com/ayyyane/unit1-2024/assets/142702159/dfa5476c-3f22-407b-9c90-aafc20ee4e53">


## solution 
```.py

def get_13tt3r(msg:str)->str:
  msg = input()
  dic = ["a":"4", "e":"3", "i":"1","o":"0"," ":"_"]
  #number must be str
  output = ""
  for letter in msg:
    if letter in dic:
      letter = dic[letter]
      output += letter
    else:
      output += letter
  return output

**test**
get_13tt3r("hello world")
get_13tt3r("Why did I choose CS?")
get_13tt3r("Remember the Figure Caption")

```

## evidence 
<img width="726" alt="quiz017_e" src="https://github.com/ayyyane/unit1-2024/assets/142702159/f666aa94-b1d0-4fdb-875e-533346676225">

# Question b
