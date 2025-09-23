# Python function rules 

# Python – funktion rules (fra 0 til “hej unknown”)

> **Sådan læser du eksemplerne:** Linjer med `# ->` viser, hvad koden giver som output.  
> Eksempel: `print(2+3)  # -> 5`

---

## 1) `print` – skriv noget på skærmen (terminalen)
```python
print("Hej verden")            # -> Hej verden
print("Hej unknown")           # -> Hej unknown

---

navn = "unknown"               # en tekst (str)
alder = 34                     # et helt tal (int)

print(navn)                    # -> unknown
print(alder)                   # -> 34

---

t = "34"                       # str                    (gåseøjne= tekst)
x = int(t)                     # "34" -> 34 (int)       (Uden decimal)
y = float("3.14")              # "3.14" -> 3.14 (float) (med decimal)
s = str(99)                    # 99 -> "99" (str)       (str står for tekst)

sand = True                    # bool
falsk = False                  # bool

---

navn = input("Hvad hedder du? ")                 # skriver fx: unknown
alder = int(input("Hvor gammel er du? "))        # skriver fx: 34

print(f"Hej {navn}, du er {alder} år.")          # -> Hej unknown, du er 34 år.
print("Om 5 år er du", alder + 5)                # -> Om 5 år er du 39
# eller med f-string:
print(f"Om 5 år er du {alder + 5}")              # -> Om 5 år er du 39

## Altid patanteser pr variabel - eksembel se int + input

by = "København"
print(f"{navn} bor i {by}.")                     # -> unknown bor i København.

---

## Betingelser if/elif/else 

alder = int(input("Alder: "))

if alder < 13:
    print("Du er et barn")
elif 13 <= alder < 18:
    print("Du er teenager")
elif 18 <= alder < 30:
    print("Du er ung voksen")
else:
    print("Du er voksen")

## Flere operatore 

x = 10
print(x == 10)   # -> True
print(x != 5)    # -> True
print(x > 7)     # -> True
print(x <= 9)    # -> False

## Logiske operatore and or not 

alder = 20
har_id = True
if alder >= 18 and har_id:
    print("Adgang tilladt")    # -> Adgang tilladt

---

## Range og for-loop(gentagelser)

for i in range(3):
    print(i)
# -> 0
# -> 1
# -> 2

for i in range(1, 6):
    print(i)
# -> 1 2 3 4 5 (på hver sin linje)

---

## Random navn 

import random

navne = ["Patrick", "Maria", "Jonas", "Aisha"]
tilfældigt_navn = random.choice(navne)

print(f"Random navn: {tilfældigt_navn}")   # -> fx: Random navn: Maria

---


