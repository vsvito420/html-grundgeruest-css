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
  - [CSS](#css)
    - [Kommentare](#kommentare)
    - [Verbindung zwischen HTML und CSS](#verbindung-zwischen-html-und-css)
    - [Hintergrund und Schriftfarbe](#hintergrund-und-schriftfarbe)
    - [Schrift und Schriftgröße](#schrift-und-schriftgröße)
    - [Schriftgröße der Überschrift ändern](#schriftgröße-der-überschrift-ändern)
    - [Kontaktadresse in Fußzeile](#kontaktadresse-in-fußzeile)
    - [Links (das HTML-Element a)](#links-das-html-element-a)
    - [Wenn die Maus darüberschwebt (Pseudoklassen)](#wenn-die-maus-darüberschwebt-pseudoklassen)
    - [Möglichkeit 1: CSS-Regeln in einer eigenen Datei](#möglichkeit-1-css-regeln-in-einer-eigenen-datei)
    - [Möglichkeit 2: Zwischen head und head Element style](#möglichkeit-2-zwischen-head-und-head-element-style)
    - [Möglichkeit 3: Direkt im HTML-Element mit dem Attribut](#möglichkeit-3-direkt-im-html-element-mit-dem-attribut)
    - [Box-Modell](#box-modell)
    - [Vorrang der Regeln](#vorrang-der-regeln)
    - [Webseite zentrieren mit Width und Margin](#webseite-zentrieren-mit-width-und-margin)

### Kommentare
```css
/* Dies ist ein einzeiliger Kommentar */

/*
Dies ist
ein mehrzeiliger
Kommentar
*/
```

### Verbindung zwischen HTML und CSS
```html
<link rel="stylesheet" type="text/css" href="styles.css">
```

### Hintergrund und Schriftfarbe
```css
body {
  background-color: #f2f2f2;
  color: #333333;
}

div {
  background-color: #ffffff;
  color: #666666;
}

header {
  background-color: #008080;
  color: #ffffff;
}
/* Weitere Selektoren und Eigenschaften können entsprechend hinzugefügt werden */

### Schrift und Schriftgröße
```css
body {
  font-family: Arial, sans-serif;
  font-size: 16px;
}
```

### Schriftgröße der Überschrift ändern
```css
h1 {
  font-size: 24px;
}
```

### Kontaktadresse in Fußzeile
```html
<footer>
  Kontakt: example@example.com
</footer>
```

### Links (das HTML-Element a)
```html
<a href="https://www.example.com">Besuch unsere Website</a>
```

### Wenn die Maus darüberschwebt (Pseudoklassen)
```css
a:hover {
  color: #ff0000;
}
```

## Regeln:
### Möglichkeit 1: CSS-Regeln in einer eigenen Datei
Um CSS-Regeln in einer eigenen Datei zu speichern, erstelle eine separate CSS-Datei (z.B. `styles.css`) und verlinke sie in deinem HTML-Dokument.

### Möglichkeit 2: Zwischen head und head Element style
```html
<style>
  /* CSS-Regeln hier einfügen */
</style>
```

### Möglichkeit 3: Direkt im HTML-Element mit dem Attribut
```html
<p style="color: #0000ff;">Dies ist ein Beispieltext.</p>
```

### Vorrang der Regeln
In CSS gelten die Regeln, die später im Code stehen, wenn mehrere Regeln auf das gleiche Element angewendet werden. Zum Beispiel:
```css
p {
  color: #000000;
}

p {
  color: #ff0000;
}
```
In diesem Beispiel wird die Textfarbe der Absätze auf Rot gesetzt, da die zweite Regel später im Code steht.

### Box-Modell
Das Box-Modell beschreibt die verschiedenen Teile eines HTML-Elements, wie z.B. margin (Außenabstand), border (Rahmen), padding (Innerabstand) und content (Inhalt).

### Webseite zentrieren mit Width und Margin
Um eine Webseite zu zentrieren, kann die `margin-left` und `margin-right` auf `auto` gesetzt werden. Beispiel:
```css
body {
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}
```
In diesem Beispiel wird die Breite der Webseite auf 80% der verfügbaren Breite eingestellt und der linke und rechte Rand wird automatisch angepasst, um das Element zentriert darzustellen.
