# TODO

[Try it!](https://christernilsson.github.io/BildbankenForAll/)

## HIGH 

### GUI Katalogknappar

* Typ 2026, turneringskataloger samt grupper.
* Visa antalet träffar i katalogerna med ().
* `Upp` för att komma tillbaka.

### PYTHON Automatisk exekvering av update.py

* Github secrets
* schedule cron

### Krockar mellan fotografer

* De ska hålla sig till exakt samma namn för turneringskatalogen
* De ska ha olika bildfilnamn annars tappar man en bild
* Då blir merge korrekt och båda bilderna kommer med i samma katalog

## LOW ###################

### PYTHON Logga filer som saknar datum i namnet tillsammans med fotografens nyckel.

### PYTHON Effektivisering

* [ ] update.py kan fråga efter flera fotografer samtidigt.

### Chess-Results

* [ ] C1209676 => "https://chess-results.com/tnr1209676.aspx?lan=1&art=4"

## DONE 

### Inbjudan, Fakta, Resultat

Dessa hanteras tillsvidare genom att ta bilder.

### GUI Knappar
* [x] Share kan skippas. Urlen ska vara up to date. Dvs vald katalog och söksträng
* [x] Download skippas. Enstaka bilder sköts av enbildsvisningen.
* [x] Clear Bort
* [x] Case bort
* [x] All bort
* [x] Help bort
* [x] "found 66424 images in 52 ms" bort
* [x] AB:7 A:2 bort

### GUI Selektion med kryssrutor och bildspel
* [x] Tas bort - verkar inte användas.

### GUI Turneringslänk
* [x] T12345 är löst. Medlemssystemet enbart.

## SKA EJ GÖRAS

### PYTHON och GUI Länk till Inbjudan och Facts
* I12345 och F12345. Det behövs en fil file_index.txt som mappar mot en url
* Varje fotograf har en egen nummer serie
* Filnamnet sparas i JSON-filen

