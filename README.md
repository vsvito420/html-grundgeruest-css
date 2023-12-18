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
    - [Vorrang der Regeln](#vorrang-der-regeln)
    - [Box-Modell](#box-modell)
      - [Webseite zentrieren mit Width und Margin](#webseite-zentrieren-mit-width-und-margin)
      - [Alle Boxen sind gleich - das Modell](#alle-boxen-sind-gleich-das-modell)
      - [Der Inhaltsbereich: Width und Height](#der-inhaltsbereich-width-und-height)
      - [Der Innenabstand: Padding](#der-innenabstand-padding)
      - [Der Rahmen drumherum: Border](#der-rahmen-drumherum-border)
      - [Der Außenabstand: Margin](#der-äußenabstand-margin)
      - [Gesammtbreite einer Box berechnen](#gesammtbreite-einer-box-berechnen)

User:

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

#### Webseite zentrieren mit Width und Margin
Um eine Webseite zu zentrieren, kann die `margin-left` und `margin-right` auf `auto` gesetzt werden. Beispiel:
```css
body {
  width: 80%;
  margin-left: auto;
  margin-right: auto;
}
```
In diesem Beispiel wird die Breite der Webseite auf 80% der verfügbaren Breite eingestellt und der linke und rechte Rand wird automatisch angepasst, um das Element zentriert darzustellen.

Hier sind die Inhalte zum Box-Modell:

#### Alle Boxen sind gleich - das Modell
Das Box-Modell ist ein grundlegendes Konzept in CSS, das die verschiedenen Teile eines HTML-Elements beschreibt, wie z.B. Inhaltsbereich, Innenabstand, Rahmen und Außenabstand.

#### Der Inhaltsbereich: Width und Height
Der Inhaltsbereich einer Box ist der Bereich, in dem der Inhalt (z.B. Text oder Bilder) angezeigt wird. Die Breite und Höhe des Inhaltsbereichs können mit den CSS-Eigenschaften `width` und `height` festgelegt werden.

#### Der Innenabstand: Padding
Der Innenabstand ist der Abstand zwischen dem Inhalt und dem Rahmen einer Box. Er kann mit der CSS-Eigenschaft `padding` festgelegt werden. Zum Beispiel:
```css
div {
  padding: 20px;
}
```
In diesem Beispiel wird der Innenabstand der `div`-Elemente auf 20 Pixel gesetzt.

#### Der Rahmen drumherum: Border
Der Rahmen einer Box ist die Begrenzung des Inhaltsbereichs und kann mit der CSS-Eigenschaft `border` festgelegt werden. Zum Beispiel:
```css
div {
  border: 2px solid #000000;
}
```
In diesem Beispiel wird der Rahmen der `div`-Elemente auf eine 2 Pixel dicke, durchgezogene schwarze Linie gesetzt.

#### Der Außenabstand: Margin
Der Außenabstand ist der Abstand zwischen einer Box und anderen angrenzenden Elementen. Er kann mit der CSS-Eigenschaft `margin` festgelegt werden. Zum Beispiel:
```css
div {
  margin: 10px;
}
```
In diesem Beispiel wird der Außenabstand der `div`-Elemente auf 10 Pixel gesetzt.

#### Gesammtbreite einer Box berechnen
Die Gesammtbreite einer Box kann mit der Formel `width + padding-left + padding-right + border-left + border-right` berechnet werden. Zum Beispiel:
```css
div {
  width: 300px;
  padding-left: 20px;
  padding-right: 20px;
  border-left: 2px;
  border-right: 2px;
}
```
In diesem Beispiel beträgt die Gesammtbreite der `div`-Elemente 300 Pixel (300px Breite + 20px linke Padding + 20px rechter Padding + 2px linke Border + 2px rechte Border).
