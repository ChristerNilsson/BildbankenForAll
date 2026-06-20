UTF-8 gäller i alla textfiler.

Detta projekt består av:

1. Ett pythonprogram, update.py, som sammanställer index.json för ett antal fotografer

2. Ett webprogram, index.html, som tillåter sökning och visning mha photos.json

# update.py

Pythonprogrammet ska hämta nytillkomna filer i fotografernas kataloger.

Fotografernas kataloger ligger på olika Google Drives.

photos.json ska innehålla ett katalogträd där löven utgörs av länkar till bilder.

photographers.json innehåller registrerade fotografer samt url till deras bilder.

Detta program kan inte läsa lokala filer. 

Tills vidare lagras de båda json-filerna lokalt.

För att få bättre prestanda, ska varje fotograf ska sparas i en egen json-fil. T ex CN.json.

Dessa filer ska sparas i katalogen photographers tillsammans med manifest och changes.

Jag antar att du kontrollerar om något nytt tillkommit, för varje fotograf, innan du återskapar fotografens json.

Logga till update.log. Ska även innehålla tidpunkter. Logga varje json-fil som skapas.
Före "Startar uppdatering" ska en blank rad skrivas ut.

# photographers.json

Denna fil uppdateras manuellt.

{
	"CN": ["Christer Nilsson", "https://drive.google.com/drive/folders/1IQSQUGml83eFJQAxqi_ymg1UXhtqSv4K?usp=sharing"]
}

https://drive.google.com/drive/folders/1IQSQUGml83eFJQAxqi_ymg1UXhtqSv4K?usp=sharing pekar på denna dators drive-katalog där bilderna ligger.

# photos.json:

Behöver kataloger och filnamn visas i klartext eller räcker det med B8KCKkfXjk ?

Denna fil underhålls av update.py

{ 
	"2025": {
		"2025-09-21 Knatte-Lag-DM Stockholm_I10748_T16960": {
			"Knattelag-DM_01.Wasa_SK_2025-09-21.jpg":["B8KCGMzp4X","LOAH"],
			"Knattelag-DM_01.Wasa_SK_med_samtliga_lagtränare_2025-09-21.jpg":["B8KGJDuLbi","LOAH"],
			"Knattelag-DM_03_Wasa_SK_II_2025-09-21.jpg":["B8KCKkfXjk","CN"]
			}
		}	
}

Förklaring:

* B8KCGMzp4X = Bildfilens nyckel
* LOAH = Fotografens nyckel

# index.html

Starta inte någon web server, jag använder Go Live!

## Input 

* photographers.json
* photos.json

## Sökning

Då man ändrar i queryfältet ska urlen uppdateras. Den ska även läsa in det som står där initialt.

Om query är tomt ska bara de senaste tio bilderna visas.  
Programmet ska ha sökmöjligheter på katalognamn och bildfilsnamn.  
Färskaste bilden ska visas först.  

Sökning ska kunna ske på flera termer. Om två termer, A och B, används ska resultaten visas i ordningen AB, A, B.

## Helskärmsläge

Då man klickar på en bild ska den visas på hela skärmen.

När hela skärmen används ska man kunna zooma i en bild med mushjulet. Punkten där musen står ska stå still under zoomandet. Bilden ska kunna flyttas med mus-drag.

EXIF verkar inte gå att göra pga CORS.
