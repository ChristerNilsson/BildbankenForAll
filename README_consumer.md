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

## URL

Sökningen sparas i URL:en. Det betyder att du kan kopiera länken och skicka samma sökning till någon annan.

Exempel:

```text
http://127.0.0.1:5500/index.html?q=wasa%20klass
```

## Öppna bild

Klicka på en bild för att öppna den direkt i Google Drive.

Länken har formatet:

```text
https://drive.google.com/file/d/<bild-id>/view?usp=drive_link
```

I Google Drive kan du använda Googles egna verktyg för att zooma, ladda ner eller dela bilden, beroende på vilka rättigheter du har.

## Ladda ner

När bilden är öppnad i Google Drive kan du normalt ladda ner den via Drive-menyn. Om nedladdning saknas har ägaren begränsat rättigheterna.

## Om en bild saknas

Om en bild inte går att öppna kan den ha flyttats, raderats eller fått ändrade delningsrättigheter i Google Drive.

