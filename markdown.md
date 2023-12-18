# HTML5 & CSS Grundgerüst
- [HTML5 & CSS Grundgerüst](#html5--css-grundgerüst)
  - [HTML](#html)
    - [Skelett](#skelett)
    - [DOCTYPE](#doctype)
    - [Stammelement](#stammelement)
    - [Header](#header)
    - [Metadaten](#metadaten)
      - [Angabe des Zeichensatzes](#angabe-des-zeichensatzes)
      - [Beschreibung der Webseite](#beschreibung-der-webseite)
    - [Body](#body)

## HTML

### Skelett

Das HTML-Grundgerüst ist das Skelett einer Webseite. Es besteht aus folgenden Teilen:
1. Die erste Zeile enthält den DOCTYPE.
2. Das Stammelement `<html>` umschließt den `<head>` und den `<body>`.
3. Der `<head>` enthält Informationen über die Webseite und Elemente wie `<title>` und `<meta>`.
4. Der `<body>` enthält den Inhalt, der im Browserfenster angezeigt wird.



```html
<! Kommentare sehen so aus >

``` 

### DOCTYPE
Der DOCTYPE muss in der allerersten Zeile des Quelltexts stehen.



```html
<!DOCTYPE html>
<html lang="de">
...
</html>

``` 

### Stammelement



```html
<html>
  <!-- Hier kommt der gesamte HTML-Code hin -->
</html>

``` 

### Header



```html
<html>
  <head>
    <!-- Wichtige Informationen über die Webseite kommen hier hin -->
  </head>
<html>

``` 

### Metadaten
#### Angabe des Zeichensatzes



```html
<meta charset="utf-8">

``` 
Während des Editierens der HTML-Datei muss die Datei natürlich auch in UTF-8 gespeichert werden.

#### Beschreibung der Webseite



```html
<meta name="description" content="...">

``` 
Es sollten ungefähr zwei bis drei ganze Sätze verwendet werden, um die Webseite zu beschreiben.

### Body



```html
<html>
  <body>
  </body>
</html>

``` 
