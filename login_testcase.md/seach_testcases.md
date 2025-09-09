# Søgefunktion – Testcases  

---

### Testcase 1: Gyldig søgning  
**Forudsætning**  
Søgefeltet er synligt på siden.  

**Trin**  
1. Indtast et eksisterende produktnavn (fx “phone”).  
2. Tryk Enter eller klik “Søg”.  

**Forventet resultat**  
En resultatside/sektion vises med mindst ét match. Titler/links er klikbare.  

---

### Testcase 2: Ingen resultater  
**Forudsætning**  
Søgefeltet er synligt.  

**Trin**  
1. Indtast en streng, der ikke findes (fx “zzzz123”).  
2. Tryk Enter eller klik “Søg”.  

**Forventet resultat**  
Resultatlisten er tom, og der vises en venlig besked: *“Ingen resultater fundet”*.  

---

### Testcase 3: Tom søgning  
**Forudsætning**  
Søgefeltet er synligt.  

**Trin**  
1. Lad feltet være tomt.  
2. Tryk Enter eller klik “Søg”.  

**Forventet resultat**  
Systemet afviser søgningen (ingen navigation) og/eller viser besked: *“Indtast en søgetekst”*.  

---

### Testcase 4: Trimming af mellemrum  
**Forudsætning**  
Søgefeltet er synligt.  

**Trin**  
1. Indtast `"   phone   "` (med mellemrum foran og bagved).  
2. Udfør søgning.  

**Forventet resultat**  
Systemet fjerner mellemrum og behandler søgningen som “phone”. Resultater vises.  

---

### Testcase 5: Specialtegn  
**Forudsætning**  
Søgefeltet er synligt.  

**Trin**  
1. Indtast `phone (2024)!`.  
2. Udfør søgning.  

**Forventet resultat**  
Ingen fejl i UI eller konsol. Systemet håndterer specialtegn (enten resultater eller “ingen resultater”) uden at crashe.  
