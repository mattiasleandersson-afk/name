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

## 📁 Grupper
- Skapa flera grupper via rullgardinsmenyn högst upp.
- Välj, skapa eller ta bort grupper. Vald grupp sparas lokalt i webbläsaren.

### Exportera & importera
- **Exportera**: sparar den aktiva gruppen som JSON. Om flera grupper finns kan du välja att exportera alla.
- **Importera**: ersätter alla befintliga grupper med filens innehåll.
- **Importera (slå ihop)**: lägger till grupper från filen och slår ihop med befintliga vid matchande id.

### Filformat
```json
{
  "groups": [
    {
      "id": "grp1",
      "name": "Grupp 1",
      "photos": [
        {
          "id": "...",
          "data": "data:image/png;base64,...",
          "name": "Anna",
          "gender": null,
          "posX": 50,
          "posY": 50,
          "zoom": 1,
          "mnemonic": "",
          "stats": { "attempts":0, "correct":0, "wrong":0, "hints":0, "avgRT":0, "level":0, "streak":0, "lastAt":0 }
        }
      ]
    }
  ]
}
```

## 📊 Statistik
- Varje person har statistik: försök, rätt/fel, ledtrådar, reaktionstid, svårighetsnivå.
- Topp 5 svåraste visas under Statistik.
- Statistik sparas lokalt i webbläsaren (LocalStorage).
- Knappar:
  - **Exportera**: spara grupper till JSON-fil.
  - **Importera**: ersätt alla grupper med data från fil.
  - **Importera (slå ihop)**: kombinera grupper från fil med befintliga.
  - **Nollställ statistik**: nollställer enbart statistiken.
  - **Rensa**: tar bort alla bilder & namn i aktiv grupp, men behåller statistik.

## ❓ Hjälp - använda olika enheter
Exportera mellan olika enheter. Alla filer lagras genom "export" lokalt som en json-fil. Denna kan du sedan kopiera mellan enheter för att öppna genom "import" på din andra enhet. 
---
