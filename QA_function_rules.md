# QA funktioner

git add filnavn
👉 Fortæller Git: "Hold øje med denne fil, den skal med i næste commit."
Hvis du bruger git add ., så tager den ALT i mappen.

git commit -m "besked"
👉 Laver et "snapshot" af dine ændringer. Beskeden i -m er bare din note til dig selv og andre: "hvad ændrede jeg her?"

git push
👉 Skubber dine commits op til GitHub (så de ligger online).

git status
👉 Viser hvad der er ændret, hvad der er tilføjet, og om alt er klar til push.

---

# QA Funktion Rules

## Hvad er en test case?
En **test case** er en opskrift på, hvordan man tester en bestemt funktion i et system.  
Den består af:
- Forudsætninger (hvad skal være klar inden testen)  
- Trin (hvad gør jeg)  
- Forventet resultat (hvad skal ske)  

---

## Eksempler

### 1. Login med korrekt brugernavn og password
- **Forudsætning:** Gyldigt brugernavn og password findes i systemet.  
- **Trin:**  
  1. Åbn login siden  
  2. Indtast brugernavn og password  
  3. Tryk på "Login"  
- **Forventet resultat:**  
  Brugeren bliver logget ind og ser sin profilside.  

---

### 2. Login med forkert password
- **Forudsætning:** Gyldigt brugernavn findes.  
- **Trin:**  
  1. Åbn login siden  
  2. Indtast korrekt brugernavn og forkert password  
  3. Tryk på "Login"  
- **Forventet resultat:**  
  Systemet viser en fejl: *"Forkert password"*, og login mislykkes.

  ---      

  # QA Funktion Rules

## Hvad er en test case?
En **test case** er en opskrift på, hvordan man tester en bestemt funktion i et system.  
Den består af:
- Forudsætninger (hvad skal være klar inden testen)  
- Trin (hvad gør jeg)  
- Forventet resultat (hvad skal ske)  

---

## Login Testcases

### 1. Login med korrekt brugernavn og password
- **Forudsætning:** Gyldigt brugernavn og password findes i systemet.  
- **Trin:**  
  1. Åbn login siden  
  2. Indtast brugernavn og password  
  3. Tryk på "Login"  
- **Forventet resultat:**  
  Brugeren bliver logget ind og ser sin profilside.  

---

### 2. Login med forkert password
- **Forudsætning:** Gyldigt brugernavn findes.  
- **Trin:**  
  1. Åbn login siden  
  2. Indtast korrekt brugernavn og forkert password  
  3. Tryk på "Login"  
- **Forventet resultat:**  
  Systemet viser en fejl: *"Forkert password"*, og login mislykkes.  

---

### 3. Login med tomme felter
- **Forudsætning:** Ingen input.  
- **Trin:**  
  1. Åbn login siden  
  2. Lad felterne være tomme  
  3. Tryk på "Login"  
- **Forventet resultat:**  
  Systemet viser en fejl: *"Udfyld brugernavn og password"*.  

---

## Søgefunktion Testcases

### 4. Søge efter gyldigt produkt
- **Forudsætning:** Produktet findes i databasen.  
- **Trin:**  
  1. Gå til søgefeltet  
  2. Indtast produktnavn (fx "sko")  
  3. Tryk Enter  
- **Forventet resultat:**  
  Resultatsiden viser produktet "sko".  

---

### 5. Søge efter ugyldigt produkt
- **Forudsætning:** Produkt findes ikke i databasen.  
- **Trin:**  
  1. Gå til søgefeltet  
  2. Indtast "XYZ123"  
  3. Tryk Enter  
- **Forventet resultat:**  
  Systemet viser besked: *"Ingen resultater fundet"*.  

---

## Indkøbskurv Testcases

### 6. Tilføje produkt til kurv
- **Forudsætning:** Produkt findes og er på lager.  
- **Trin:**  
  1. Find produktet via søgning  
  2. Klik "Læg i kurv"  
  3. Åbn kurven  
- **Forventet resultat:**  
  Kurven viser produktet med korrekt navn, pris og antal.  

---

### 7. Fjerne produkt fra kurv
- **Forudsætning:** Kurven indeholder et produkt.  
- **Trin:**  
  1. Åbn kurven  
  2. Klik "Fjern" ved produktet  
- **Forventet resultat:**  
  Kurven bliver tom og viser besked: *"Din kurv er tom"*.  

