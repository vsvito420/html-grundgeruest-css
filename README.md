
# CSS-Themen
- [Kommentare](#kommentare)
- [Verbindung zwischen HTML und CSS](#verbindung-zwischen-html-und-css)
- [Hintergrund und Schriftfarbe](#hintergrund-und-schriftfarbe)
- [Schrift und Schriftgröße](#schrift-und-schriftgröße)
- [Schriftgröße der Überschrift ändern](#schriftgröße-der-überschrift-ändern)
- [Kontaktadresse in Fußzeile](#kontaktadresse-in-fußzeile)
- [Links (das HTML-Element a)](#links-das-html-element-a)
- [Wenn die Maus darüberschwebt (Pseudoklassen)](#wenn-die-maus-darüberschwebt-pseudoklassen)
- [Möglichkeit 2: Zwischen head und head Element style](#möglichkeit-2-zwischen-head-und-head-element-style)
- [Möglichkeit 3: Direkt im HTML-Element mit dem Attribut](#möglichkeit-3-direkt-im-html-element-mit-dem-attribut)

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
