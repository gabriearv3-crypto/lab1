# Lab 1 – Planering
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

### Steg 1: Förstå
- **Vad är indata?** 
  Antal enheter som ska konfigureras (heltal).
- **Vad är utdata?** 
  Totalt antal minuter samt tiden omräknad till timmar och minuter.
- **Vilka regler gäller?** 
  Basinstallationen tar alltid 15 minuter totalt. Varje enhet tar ytterligare 10 minuter. Tiden ska redovisas både i minuter och i timmar + minuter (t.ex. 1 timme och 15 minuter).
- **Vad kan gå fel?** 
  Användaren kan skriva in bokstäver istället för siffror eller mata in ett negativt tal.

### Steg 2: Planera
LÄS IN antal_enheter
BERÄKNA total_tid = 15 + (antal_enheter * 10)
BERÄKNA timmar = total_tid // 60
BERÄKNA minuter = total_tid % 60
SKRIV UT total_tid
SKRIV UT timmar och minuter

## Problem 3
### Steg 1: Förstå
- **Vad är indata?** 
  Enhetens IP-adress (text/sträng) och nätmask (heltal, t.ex. 24).
- **Vad är utdata?** 
  Nätverksadress i CIDR-notation (t.ex. "192.168.1.0/24").
- **Vilka regler gäller?** 
  Sista oktetten i IP-adressen ska ersättas med en nolla. Resultatet ska sättas ihop med nätmasken med ett snedstreck `/`.
- **Vad kan gå fel?** 
  Användaren kan mata in en ogiltig IP-adress eller en ogiltig nätmask.

### Steg 2: Planera
LÄS IN ip_adress
LÄS IN natmask
DELA IP-adressen vid punkterna (split)
ERSÄTT sista delen med "0"
SÄTT IHOP IP-adressen igen med punkter
SKRIV UT resultat i formatet ip_adress/natmask
## Del 4: Från källkod till körning