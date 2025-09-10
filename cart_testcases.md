# Indkøbskurv - Testcases . 

---

### Testcase 1 (Positiv): Læg vare i kurv 
**Forudsætning**
Produktliste er vist. Lagerstatus: på lager.

**Trin**
1. Åbn et produktside
2. Vælg evt. størrelse/farve 
3. Klik "læg i kurv"
4. Åben kurven

**Forventet resultat** 
Varen vises i kurven med korrekt navn, pris, antal = 1 og subtotal opdateret. 

---

### Testcase 2 (Negativ): Fjern fra kurv når kurven er tom
**Forudsætning**
Kurven er tom. 

**Trin**
1. Åbn kurven
2. Klik "fjern" på en (ikke eksisterende) vare / forsøg at fjerne.

**Forventet resultat**
Ingen fejl/crash. Systemet viser stadig "kurven er tom". Ingen negative værdier, ingen NaN

---

### Testcase 3 (edge): Antal = meget hæjt tal
**Forudsætning**
Produktet findes, lager kan være lavt 

**Trin**
1. Læg varen i kurven (antal=1).
2. Prøv at sætte antal til 9999 (via input/plus-knap).
3. Opdater. 

**Forventet resultat**
Systemet begrænser til max lager/forretningsregel (fx 10 stk).
Viser klar besked ("Maks 10 pr. kunde").
Ingen overflow i pris/subtotal 

