# Bildbanken - användare

Bildbanken är en söksida för bilder.

## Söka

Skriv i sökfältet för att söka på katalognamn och bildfilnamn.

Du kan söka på flera ord:

```text
anna cramling
```

Träffar som innehåller alla orden visas först. Därefter visas träffar på första ordet och så vidare.

Om sökfältet är tomt visas alla bilder i den aktuella katalogen.  
Du kan binda ihop t ex förnamn och efternamn. anna_cramling  
Bilder läses in efter hand när du scrollar.  

## Kataloger

Katalogknapparna visar katalogerna på aktuell nivå. Siffran inom parentes visar hur många bilder som finns i katalogen. Klicka på en katalog för att gå ner i den. Använd `Upp` för att gå tillbaka till föräldrakatalogen.

Sökfältet visas högst upp. Aktuell sökväg visas under sökfältet, med antal matchande bilder direkt till höger, till exempel `2026 • Turnering (123)`. På toppnivån visas `Bildportalen`. Antalet räknas om när du skriver i sökfältet.

Sökning och bildlistan gäller inom den aktuella katalogen.

Koder som `T18469` eller `C1209676` visas inte i katalog- eller bildtext. När aktuell katalog innehåller en sådan kod visas länken `Turnering` på egen rad ovanför katalogknapparna. Koder som börjar med `I`, `F` eller `R` visas inte ännu.
PDF-, URL- och TXT-filer i aktuell katalog visas också som länkar ovanför katalogknapparna, med filnamnet utan filändelse som länktext. PDF- och TXT-filer öppnas via Google Drives `/preview`-adress. Webbadressen i URL-filens andra rad läses av uppdateringsprogrammet och används direkt som länk. Länkar öppnas i samma flik.
Bildtexten visar kataloger på första raden och fotografnyckel samt EXIF-tid på egen rad, till exempel `CN @ 2022-07-10 15:58:00`.

## URL

Sökningen och aktuell katalog sparas i URL:en. Det betyder att du kan kopiera länken och skicka samma vy till någon annan.

Exempel:

```text
https://christernilsson.github.io/BildbankenForAll?q=anna cramling&folder=2026/2026-05-20 Stockholmsmästerskap 60plus snabb
```

## Öppna bild

Klicka på en bild för att öppna den direkt i Googles visningsprogram. Där kan du zooma, panorera och använda Drive-menyn.

## Ladda ner

När bilden är öppnad i Google Drive kan du normalt ladda ner den via Drive-menyn. Om nedladdning saknas har ägaren begränsat rättigheterna.

## Om en bild saknas

Om en bild inte går att öppna kan den ha flyttats, raderats eller fått ändrade delningsrättigheter i Google Drive.
