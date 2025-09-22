# Bug report 1 - Login med ugyldigt password 

**ID** BUG-001 
**Titel:** Login acceptere ugyldigt password 
**Beskrivelse:** 
Systemet tillader login med et forkert password, hvilket giver uautoiseret adgang.

**Fordusætning**
En bruger eksistere i systemet (fx brugernavn: testuser).

1. Gå til login-siden
2.Indtast ugyldigt gyldigt brugernavn:
`testuser`.
3. Indtast ugyldigt password: `123456`.
4. Klik på "login".

**Forventet resultat**
Systemet afviser login og viser en fejlmeddelelse *"Ugyldigt password"*.

**Faktisk resultat:**
Bruger logges ind, selv med ugyldigt password.

**Alvorlighed:** Kritisk
**Priortet:** Høj 
