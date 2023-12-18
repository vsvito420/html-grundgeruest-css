# HTML5 & CSS Grundgerüst

## HTML

### Skelett

> Das HTML Grundgerüst ist das Skelett einer Webseite..
> 1. in der ersten Zeile steht DOCTYPE..
> 2. das Stammelement html umschließt den head und den body
> 3. head zeigt Information über die Webseite und Elemente wie title und meta
> 4. body enthällt den inhalt der im browserfenster angezeigt wird.

    <! Kommentare sehen so aus >
   
### DOCTYPE
Der DOCTYPE muss in der allerersten Zeile des Quelltext stehen

    <!DOCTYPE  html>
    <html  lang="de">
    ...
    </html>

### Stammelement

    <html>
      <!.. hier kommt der Ganze HTML code hin>
    </html>

### Header

    <html>
	    <head>
		    <!Wichtige Informationen über die webseite kommen hier  hin>
	    </head>
    <html>
### Metadaten
#### Angabe des Zeichensatzes

    <meta charset="utf-8"
Während des editieren der HTML muss die datei natürlich in UTF-8 auch gespeichert werden.

#### Beschreibung von der Webseite

    <meta name="beschreibung" content="...">
Es sollten ungefähr zwei bis 3 ganze sätze verwendet werden um die webseite zu beschreiben

### Body

    <html>
	    <body>
	    </body>
    </html>
