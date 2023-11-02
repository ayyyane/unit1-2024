# quiz018

## prompt
<img width="1470" alt="Screenshot 2023-11-02 at 12 37 09" src="https://github.com/ayyyane/unit1-2024/assets/142702159/c69019fa-766b-462e-a20c-9baa58ada5bd">


## flowchart
<img width="645" alt="Screenshot 2023-10-25 at 17 51 12" src="https://github.com/ayyyane/unit1-2024/assets/142702159/df5a2bfe-b83e-4b18-a4de-312c26e4b912">


## solution
```.py
def get_truth():
  a,b,c = 0,0,0
  a_count,b_count = 0,0
  out = "| A | B | C |\n"
  for x in range(8):
    a_count += 1
    b_count += 1
    c = not c
    if a_count%4 == 0:
      a = not a
    if b_count%2 == 0:
      b = not b
    out += f"| {int(a)} | {int(b)} | {int(c)} |\n"
  return out

```

## evidence
<img width="1417" alt="quiz018_e" src="https://github.com/ayyyane/unit1-2024/assets/142702159/35a92284-88dd-4a8c-956e-052ef0d870e4">
