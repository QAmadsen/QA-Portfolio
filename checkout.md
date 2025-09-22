# Testcases - Checkout 

## Testcase 1. (positiv) vælge vare i kurv 

**Trin**
1. Søg på produkt 
2. Tryk på navn, og vare lægges i kurven. 
3. Indtaste gyldig  adresse
4. Indtast belaingsoplysninger 

**Forventet resultat**
Varen lægges i kurven 
Adresse gyldig
Belaing gennemført

## Testcase 2. (Negativ) tom kurv, 

**Trin** 
1. TRyk på kurv.
2. Slet nurværende vare så kurv er tom.
3. Indtast forkert adresse
4. Indtast forkerte betalingsoplysninger

andet eksempel

1. Tryk på vare som ikke er på lager 
2. Adresse ugyldig
Belatingsopysninger forkerte - Indtast korrekte

**Forventet resultat**

Første eksempel 
Vare slettet og kurv er hermed tom 

Anden eksempel 
Vare kommer ikke i kurv, da den ikke er på lager .
Adresse er gyldig - Indtast venlig gyldig adresse
Betalingsoplysninger forkerte - indtast korrekte


## Testcase 2. (Edge) 

**Trin**

1. Trykker 11 gange på antal af produkt.
2. Skriver flere adresser
3. Skriv betalingsoplysninger uden nok penge 

**Forventet resultat**

Begrænset køb pr kunde . kun tilladt "10" pr kunde
Kun en adresse tilladt 
Ikke nok pengep på konto

