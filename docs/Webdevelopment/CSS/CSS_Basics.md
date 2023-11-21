# CSS - Cascading Style Sheet

- In HTML wird grob strukturiert und die großen Bereiche definieren
- In CSS wird grob strukturiert und Farben vergeben für bessere Sichtbarkeit


- Man kann Elementen Stiele geben
  - Farben
  - Größen
  - Positionierung
- Es ist auch möglcih mehrere Attribute gleichzeitig zu bearbeiten, auch wenn sie in anderen Elementen verschachtelt sind
- Allgemeine Definitionen werden von spezielleren Definitionen überschrieben!

|                      |                                                                           |
| :------------------: | :-----------------------------------------------------------------------: |
|      `<p>…</p>`      | Im CSS sagen das alle <p> rot sein sollen aber alle `<p id="lala">` grün! |
| `<p id="lala">…</p>` | somit wird nur der <p> - Tag mit der id umgefärbt weil es spezifisch ist! |

# Wie kann man CSS in HTML verwenden?
- Direkt im HTML-Tag
- CSS-Block im HTML-File (im Header)
  - ist nur sinnvoll wenn es nur eine einzige HTML Seite gibt
- Externes CSS-File
  - wird in HTML-File im Header verlinkt
  - `<link rel="stylesheet" href="css/styles.css">`

# CSS Beispiele
```CSS
body {
  background-color: #CC0000;
  color: #FFF;            // Color wird immer auf Texte bezogen!
  font-familiy: Arial;    // Welche Schriftart möchte ich verwenden!
                          // -> Schriftarten mit Leerzeichen im Namen müssen in "..." gesetzt werden
}

h1 {
  color: #00;             // alle h1 Überschriften werden rot angezeigt
}

p {
  background-color: #CCC;
  padding: 20px 50px      // padding ist der Innenabstand!
                          // 1. Wert (20px) beschreibt den wert oben und unten
                          // 2. Wert (50px) beschreibt den Wert links und rechts
}

p {
  background-color: #CCC;
  padding: 20px 50px 100px 350px;   // es ist auch möglich 4 Werte bei padding anzugeben
                                    // top / right / bottom / left
                                    // die Werte werden im Uhrzeigersinn definiert!
}

body, h1, p, ul {
  margin: 0;             // Man kann auch mehrere Elemente gleichzeitig angreifen und bearbeiten
}

```

> Padding = Innenabstand
> Margin = Außenabstand

> * Selektor für ALLE Elemente die es gibt!

```CSS
* {               // Entfernt alle vordefinierten Abstände
  margin: 0;      // maximal 50-70 Zeichen in einer Zeile in einem Text
  padding: 0;     // für bessere Lesbarkeit!
}

p {               // Definiert die Breite des Textes!
  width: 700px;   // keine höhe angegeben, da sich diese selbt generiert!
                  // wenn doch angegeben, wird der Text komisch aussehen wenn dieser doch mehr Platz braucht und ist dann nicht mehr leserlich!
}
```

> -Wenn nichts davor steht, ist es ein normaler HTML Tag
> -# Steht für ID's
> -. steht für Class
> -%-Angaben bezeihen sich immer auf das eltern element!

# Class Attribut
Class Attribute knan man auch einfach verwenden wenn diese in verschiedenen Attributen liegen! ID's NICHT!




- Wenn ein aktiver Button gesondert gestylte werden möchte! Muss ich diesem Punkt eine zusätzliche class oder ID geben damit ich diesen anders stylen kann als die anderen!
  - Class="act"
