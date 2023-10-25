# quiz018

## prompt

## flowchart



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
