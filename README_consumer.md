# Bildbanken - användare

Bildbanken är en söksida för bilder.

## Söka

Skriv i sökfältet för att söka på katalognamn och bildfilnamn.

Du kan söka på flera ord:

```text
wasa klass
```

Träffar som innehåller båda orden visas först. Därefter visas träffar på första ordet och sedan träffar på andra ordet.

Om sökfältet är tomt visas de tio senaste bilderna.

Turneringskoder i katalognamn visas som länken `Resultat`, till exempel för `T18469`.
Bildtexten visar kataloger på första raden och fotografnyckel samt EXIF-tid på egen rad, till exempel `CN @ 2022-07-10 15:58:00`.

## URL

Sökningen sparas i URL:en. Det betyder att du kan kopiera länken och skicka samma sökning till någon annan.

Exempel:

```text
http://127.0.0.1:5500/index.html?q=wasa%20klass
```

## Öppna bild

Klicka på en bild för att öppna den direkt i Googles visningsprogram. Där kan du zooma, panorera och använda Drive-menyn.

## Ladda ner

När bilden är öppnad i Google Drive kan du normalt ladda ner den via Drive-menyn. Om nedladdning saknas har ägaren begränsat rättigheterna.

## Om en bild saknas

Om en bild inte går att öppna kan den ha flyttats, raderats eller fått ändrade delningsrättigheter i Google Drive.
