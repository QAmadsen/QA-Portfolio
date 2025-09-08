# Testcase 1 : Gyldigt login

**Forudsætning**

**Trin**
Indtast gyldigt brugernavn.
Indtast gyldigt password.
Klik på "Login"-knappen.

**Forventet resultat:**
Brugeren bliver logget ind og ført til forsiden. 
---

# Testcase 2 : Ugyldigt login

#**Forudsætning**
Gyldigt brugernavn er indtastet 
**Trin**
Indtast gyldigt brugernavn.
Indast ugyldigt password.
Klik på "Login"-knappen.

**Forventet resultat:**
Brugeren får en fejlmeddelelse:
*"Forkert brugernavn eller adgangskode"*
---

# Testcase 3 : Forkert brugernavn 

# **Forudsætning**
Ugyldigt brugernavn er indtastet 
Gyldigt password er indtastet 

**Trin**
Indtast ugyldigt brugernavn
Indtast gyldigt password 
Klik på "Login"-kappen

**Forventet resultat**
Brugeren får en fejlmeddelelse:
*"Forkert brugernavn eller adgangskode"*
---

##Testcase 4 : Tomme felter ved login 

**Forudsætning**
Login-siden er åbnet. 

**Trin**
Lad feltet for nrugernavn stå tomt.
Lad feltet for adgangskode stå tomt. 
klik på "Login"-knappen

**Forventet resultat**
Systemet viser en fejlmeddelelse 
*"Brugernavn og adgangskode skal udfyldes"*