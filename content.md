### Izveidot number guessing ar Python programmēšanas valodu

### Dokumenta saturs

### 1. Aprakstīt spēli
### 2. Speles loģika

Dators nejauši ģenerē vienu skaitli no 1 līdz 100. Tālāk, piedāvā spēlētājam uzminēt to skaitli. Un t.t.

Spēles loģika ir labi apskatāma šajā kodā:
```py

import random

number = random.randint (1, 100)
guess = 0

while guess != number:
    if guess < number:
        print("Pamēģini lielāku skaitli.")
    else:
        print("Pamēģini mazāku skaitli.")

    guess = int(input("Uzmini skaitli: "))
    tries += 1
else:
    if tries <4:
        print(f"WOW! Tu uzminēji tikai pēc {tries} reizēm!")
    elif tries < 7:
        print (f"Nav slikti, uzmineji pēc {tries} reizēm! ")
    else:
        print(f"Hm... vajadzētu patrenēties, uzmineji")
```

