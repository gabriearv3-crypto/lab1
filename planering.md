# Lab 1 – Planering
## Problem 1
## Problem 2
## Problem 3
## Del 4: Från källkod till körning# Lab 1 – Planering
## Problem 1

### Steg 1: Förstå
- **Vad är indata?** 
  Platskod (text), Enhetstyp (text) och Senaste använda nummer (heltal).
- **Vad är utdata?** 
  Ett sammansatt och formaterat hostnamn (text) för nästa enhet, till exempel "sto-srv-08".
- **Vilka regler gäller?** 
  Platskod och enhetstyp måste göras om till små bokstäver. Delarna ska sättas ihop med bindestreck. Det nya numret (senaste numret + 1) måste formateras så att det alltid har två siffror (en nolla läggs till framför siffrorna 1–9).
- **Vad kan gå fel?** 
  Användaren kan skriva in bokstäver istället för siffror när numret efterfrågas. Numret kan bli 100 eller mer, vilket bryter regeln om två siffror. Användaren kan lämna inmatningen tom.

### Steg 2: Planera
LÄS IN platskod
LÄS IN enhetstyp
LÄS IN senaste_nummer
BERÄKNA nästa_nummer = senaste_nummer + 1
BERÄKNA formaterat_nummer = nästa_nummer med två siffror (t.ex. 08)
BERÄKNA hostnamn = platskod (små bokstäver) + "-" + enhetstyp (små bokstäver) + "-" + formaterat_nummer
SKRIV UT "Nästa hostnamn: " + hostnamn

## Problem 2
## Problem 3
## Del 4: Från källkod till körning