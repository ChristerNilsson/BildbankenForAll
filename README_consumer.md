# Bildbanken - användare

Bildbanken är en söksida för bilder.

## Söka

Skriv i sökfältet för att söka på katalognamn och bildfilnamn.

Du kan söka på flera ord:

```text
wasa klass
```

Träffar som innehåller båda orden visas först. Därefter visas träffar på första ordet och sedan träffar på andra ordet.

Om sökfältet är tomt visas alla bilder i den aktuella katalogen.
Bilder läses in efter hand när du scrollar.

## Kataloger

Katalogknapparna visar katalogerna på aktuell nivå. Siffran inom parentes visar hur många bilder som finns i katalogen. Klicka på en katalog för att gå ner i den. Använd `Upp` för att gå tillbaka till föräldrakatalogen.

Sökfältet visas högst upp. Aktuell katalog visas under sökfältet, med antal matchande bilder direkt till höger om katalognamnet, till exempel `Bildbanken (123)`. Antalet räknas om när du skriver i sökfältet.

Sökning och bildlistan gäller inom den aktuella katalogen.

Koder som `T18469` visas inte i katalog- eller bildtext. När aktuell katalog innehåller en sådan kod visas länken `Turnering` på egen rad under katalogknapparna. Koder som börjar med `I`, `F` eller `R` visas inte ännu.
Bildtexten visar kataloger på första raden och fotografnyckel samt EXIF-tid på egen rad, till exempel `CN21 @ 2022-07-10 15:58:00`.

## URL

Sökningen och aktuell katalog sparas i URL:en. Det betyder att du kan kopiera länken och skicka samma vy till någon annan.

Exempel:

```text
http://127.0.0.1:5500/index.html?q=wasa%20klass&folder=2026/2026-05-20%20Stockholmsm%C3%A4sterskap%2060plus%20snabb
```

## Öppna bild

Klicka på en bild för att öppna den direkt i Googles visningsprogram. Där kan du zooma, panorera och använda Drive-menyn.

## Ladda ner

När bilden är öppnad i Google Drive kan du normalt ladda ner den via Drive-menyn. Om nedladdning saknas har ägaren begränsat rättigheterna.

## Om en bild saknas

Om en bild inte går att öppna kan den ha flyttats, raderats eller fått ändrade delningsrättigheter i Google Drive.
