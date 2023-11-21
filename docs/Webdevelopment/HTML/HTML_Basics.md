Murphys Gesetz:

- „Alles, was schiefgehen kann, wird auch schiefgehen.“ 
- „Wenn es mehrere Möglichkeiten gibt, eine Aufgabe zu erledigen, und eine davon in einer Katastrophe endet oder sonst wie unerwünschte Konsequenzen nach sich zieht, dann wird es jemand genauso machen.“
- „Was man dem Unbewussten als wahr übermittelt, wird wahr.“ 

---

|              | WebDev          |                             |
| :----------: | :-------------- | :-------------------------: |
|              | HTML (Struktur) |                             |
| CSS (Design) |                 | JavaScript (Funktionalität) |

# HTML (Hypertext Markup Language)
- ist eine Auszeichnungssprache
  - Sagt aus was für ein Element verwendet wird
    - Eine Überschrift
    - Ein Absatz
    - Eine Liste
    - Eine Tabelle
  - Sagt aus welche Bedeutung dieser Text hat
  - Hat nur einen begrenzten Wortschatz

## Struktur
```html
	<html>
		<head>
		</head>
		<body>
		</body>
</html>
```
- Head
  - Im head Bereich werden sämtliche Metadaten und Verlinkungen zu CSS untergebracht
  - In den Title tag `<title>` Dokumentennname `</title>` wird der Dokumentenname (das was im Browser im Tab angezeigt werden soll) hineingeschrieben
  - Alles was im Head eingefügt wird, wird nicht auf die Homepage übernommen (nicht sichtbar!)
- Body:
  - Im body Bereich wird alles eingefügt was tatsächlich auf der Homepage sichtbar sein soll!
  - Unter anderem die Tags für 
    - `<p>` Absätze `</p>`
    - `<h1>` Überschriften und Subüberschriften h1-h3 `</h1>`
    - `<br>` Zeilenumbrüche (dieser Tag hat seit html5 keinen Schließenden Tag mehr!!)
    - `<hr>` Trennstriche (dieser Tag hat keinen Schließenden Tag)
    - `<ul>` Ungeordnete Liste
    - `<ol>` Geordnete Liste
    - `<dl>` Definitions Liste
    - etc


Index.html
  - Die Startseite des Ganzen Projekts / der ganzen Homepage
  - Sollte immer auf der obersten Ebene liegen damit diese vom Server erkannt wird und auf gerufen werden kann
  - Wird nicht in einen der Ordner abgelegt!!!!

## HTML Version
- Bevor man mit HTML Coding beginnt, muss man der Datei bekannt geben, mit welcher HTML-Version man arbeiten möchte!
- document type declaration
- `<!doctype html>`
- Für die Sprachkennzeichnung in den `<html>` Tag das Sprachkürzel einfügen!
  - `<html lang="de">`
- Meta-Tag:
  - Wer hat es erstellt
  - Keywords
  - Welcher Zeichensatz/Charakter-Set
    - `<meta charset="utf-8">`

## Kommentare in HTML
```<!-- Dieser Text wird auskommentiert! -->```

Alles was innerhalb der Pfeile steht wird auf der Homepage nicht mehr angezeigt und kann unter anderem zur Strukturierung verwendet werden!
## Tags
- Sagt dem Programm um welche Art von Text es sich handelt!
- Fast jeder Tag hat einen Anfang und ein Ende!
  -  <…> … </….>
-  Um bekannt zu geben das es sich um eine Überschrift handelt benutzt man diesen Tag
   - ```<h1> Hier wird die Überschrift eingegeben </h1>```
     - Überschriften können von h1 bis h6 reichen und werden je nach subüberschriften immer kleiner! Im normal fall wird h1 - h3 verwendet

## Verlinkung von Index zu Page 1
- Von der Index-Datei ausgehend, der Ordner im Selben Verzeichnis liegen!
- Es ist nicht notwendig das komplette Verzeichnis anzugeben!
- ```<a href="html/page_1.html">```
  - In dem Verzeichnis wo die Index Datei liegt, wird nach dem Ordner "html" gesucht und in diesem Ordner die Datei Page_1 verwendet!

## Verlinkung von Page 1 zu Index
- Die Index Datei befindet sich außerhalb des Ordners in dem Page 1 liegt. Also muss man aus dem Ordner heraus navigieren. 
- Aus dem Ordner herausnavigieren ist `../`
  - ```<a href="../Index_html">```

## Listen
- ungeordnete Liste
```html
  <ul>
    <li> Spalte1 </li>
    <li> Spalte2 </li>
  </ul>
```
Ausgabe:
- Spalte1
- Spalte2

- geordnete Liste

```html
  <ol>
    <li> Spalte1 </li>
    <li> Spalte2 </li>
  </ol>
```
Ausgabe:
1. Spalte1
2. Spalte2

- Definitions Liste
```html
  <dl>
    <dt> allg. </dt>      // einen zu beschreibenden Audruck in einer Beschreibungsliste
    <dd> allgemein </dd>  //enthält eine Beschreibung oder Definition in einer Beschreibungsliste
```

## Tabellen
```html
<table>
  <thead>
    <tr>
      <td>ID</td>
      <td>Vorname</td>
      <td>Nachname</td>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>1</td>
      <td>Susi</td>
      <td>Muster</td>
    </tr>
  </tbody>

  <tfoot>
  <tr>
    <td>Summe</td>
    <td></td>
    <td>2</td>
  </tr>
</table>
```

<table>
  <thead>
    <tr>
      <td>ID</td>
      <td>Vorname</td>
      <td>Nachname</td>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>1</td>
      <td>Susi</td>
      <td>Muster</td>
    </tr>
  </tbody>

  <tfoot>
  <tr>
    <td>Summe</td>
    <td></td>
    <td>2</td>
  </tr>
</table>


## Links in HTML einfügen

```<a href="page_1.html">…Text…</a>```
- a = Anker-Tag
- href = Attribut Name
- "page_1.html" = Attribut Wert

## Bilder in HTML einfügen
```<img src="Pfad zu dem Bild.jpg" alt="Was ist auf dem Bild zu sehen" title="Bildbeschreibung" width="Wert in Pixel" height="Wert in Pixel">```

- img 
  - Tag muss nicht geschlossen werden da er alle Informationen besitzt die er braucht!
- alt
  - Alternativtext
  - Für Barrierefreiheit
  - zum Vorlesen
  - Wenn das Bild nicht geladen wird, ist das der Text der angezeigt wird.
- title
  - wird angezeigt wenn man mit der Maus über das bild fährt
- width / height
  - Angabe von Breite und Höhe in Pixel
  - Wenn nur einer der beiden Werte angegeben wird, wird der zweite Wert proportional berechnet
  - Man sollte **IMMER** einen Width oder Height Wert angeben da sonst bei einer Langsamen Internetverbindung die Bilder langsamer nachgeladen werden als der Text und dieser somit im schlimmsten Fall während des Lesens immer weiter nach unten rutscht!
    - Cumulative Layout Shift
      - Kein Platzhalter war für das Bild geplant, somit ist der Text ganz oben auf der Seite bis die Bilder geladen werden.

## Video in HTML einfügen
- `<video src="…" width="800" autoplay>`
  - Autoplay wird in den meisten Browsern blockiert
- `<video src="…"width="800" controls>`
  - bei controls Bedienelemente werden eingeblendet

> Video Tag muss geschlossen werden `</video>`


## HTML-Tags identifizierbar machen
- ```<h2 id="headline_1"> Überschrift </h2>```
- Für den Link selbst: ```<a href="#headline_1>Text</a>```
- Id's MÜSSEN immer mit einem Buchstaben anfangen!!!

## Responsive Design
- Auf jedem Gerät sieht es gleich aus
- Es wird alles auf die Größe des Geräts angepasst!
