# name# 

📸 Namnträning

Ett enkelt träningsprogram för att lära sig namn kopplade till bilder.

## 🚀 Kom igång
1. Öppna sidan i din webbläsare: https://mattiasleandersson-afk.github.io/name/

2. Klicka **Hantera** för att:
   - Ladda upp bilder (via knappen eller dra & släpp).
   - Skriv namn direkt under varje bild.
   - Lägg till kön (kille/tjej).
   - Lägg till en valfri minnesregel.
   - Justera beskärning genom att dra i bilden (panorera/zooma med mus).

3. Klicka **Quiz** för att träna.
   - **Bild → Namn**: välj rätt namn till en bild.
   - **Namn → Bild**: välj rätt bild för ett namn.
   - **Skriv namn**: skriv själv (fuzzy match).
   - Du får feedback om rätt/fel. Rätt svar visas vid fel.
   - Efter quizet visas en genomgång av de namn du missade, med möjlighet att träna på bara dem.

## 📊 Statistik
- Varje person har statistik: försök, rätt/fel, ledtrådar, reaktionstid, svårighetsnivå.
- Topp 5 svåraste visas under Statistik.
- Statistik sparas lokalt i webbläsaren (LocalStorage).
- Knappar:
  - **Exportera**: spara data (JSON). Denna fil lagras lokalt på din dator, inget sparas online.
  - **Importera**: ersätt allt med ny data.
  - **Importera (slå ihop)**: kombinera ny data med befintlig.
  - **Nollställ statistik**: nollställer enbart statistiken.
  - **Rensa**: tar bort alla bilder & namn, men behåller statistik.

## ❓ Hjälp - använda olika enheter
Exportera mellan olika enheter. Alla filer lagras genom "export" lokalt som en json-fil. Denna kan du sedan kopiera mellan enheter för att öppna genom "import" på din andra enhet. 
---
