## Form Tag:
Im HTML verwendet man für Formulare das Form-Tag.
Das Form-Tag besitzt ein öffnendes und ein schließendes Tag.

	<form>  Formular Inhalt </form>

Innerhalb des öffnenden Tags kann man durch das Attribut "method" festlegen ob das Formular Daten von einem Server abrufen soll oder ob man selbst die Daten übermitteln möchte.

`<form method="post"> Formular Inhalt </form>`

- Methode Post:
  - Die POST-Methode schreibt die URL-Parameter in den HTTP-Request für den Server. Sie sind damit für Benutzer nicht sichtbar. Der Umfang der POST-Anfragen ist unbeschränkt.
- Methode Get:
  - Bei der GET-Methode werden die Daten, die an den Server gesendet werden sollen, direkt in die URL geschrieben.

## Input Tag:
Für die Eingabefelder des Kontaktformulars werden Input-Tags verwendet.
Die Input-Tags brauchen kein schließendes Tag!
Innerhalb des Tags kannman durch das Attribut "typ" festlegen, welche Funktion das Eingabefeld hat. Beim E-Mail Eingabefeld tragt man dann an dieser Stelle "email" ein und bei einem Text Eingabefeld "text".

`<input type="text">`
`<input type="email">`
	
## Textarea Tag
Für ein großes Textfeld in einem Kontaktformular verwendet man das Textarea-Tag. Dieses Tag besitzt ein öffnendes und ein schließendes Tag!
Innerhalb des öffnenden Tags kann man durch das Attribut "rows" festlegen, wie viele Zeilen das Texteingabefeld besitzen soll. Soll das Eingabefeld 7 Zeilen hoch sein, muss an dieser Stelle die Zahl 7 eingetragen werden.

`<textarea rows="7"></textarea>`
	
## Label Tag:
Die Eingabefelder benötigen jetzt auch noch eine Überschrift, damit der Besucher der Webseite weiß welche Informationen in welches Feld gehören. Hierfür verwendet man bei Formularen das Label-Tag. Dieser Tag besitzt ein öffnendes und ein schließendes Tag. Zwischen geöffneten und geschlossenen Tag fügt man die den jeweiligen Text ein der neben dem Feld angezeigt werden soll.

```html
<label>Name:</label> 
<input type="text"> 
<label>E-Mail:</label> 
<input type="email"> 
<label>Betreff:</label> 
<input type="text"> 
<label>Nachricht:</label> 
<textarea rows="7"></textarea>
```
	
## Label Tag mit ID's: 
Damit sich der Label-Tag auf seinen vorgesehenen Input auch wirklich bezieht, wird der Input zusätzlich mit einer ID versehen! 

`<input type="text" name="name" id="name">`

Damit der Label-Tag sich jetzt direkt auf den Input bezieht, muss dieser jetzt mit "label for =" beschrieben werden! Das wird in späterer folge mit PHP einfacher zu lesen sein!

```html
<label for="name">Name:</label> 
<input type="text" name="name" id="name"> 
```

## Name-Attribute:
Jedem Eingabefeld muss noch mit einem Namen versehen werden, sodass auch der Server versteht, in welchem Feld sich welche Information befindet. Hierfür wird das Attribut "name" verwendet.

```html
<label>Name:</label> 
<input type="text" name="name"> 
<label>E-Mail:</label> 
<input type="email" name="email"> 
<label>Betreff:</label> 
<input type="text" name="betreff"> 
<label>Nachricht:</label> 
<textarea rows="7" name="text"></textarea>
```
	
## Pflichtfelder festlegen:
Soll das Kontakformular Pflichtfelder enthalten, muss das Attribut "required" festgelegt werden.

	<label>Name:</label> 
	<input type="text" name="name"> 
	<label>E-Mail:</label> 
	<input type="email" name="email" required> 
	<label>Betreff:</label> 
	<input type="text" name="betreff"> 
	<label>Nachricht:</label> 
	<textarea rows="7" name="text" required></textarea>
	
## Einen Button hinzufügen:
Als letztes muss das Kontaktformular noch ein Button hinzugefügt werden. Für einen Button verwendet man den Button-Tag. Dieses Besitzt ein öffnendes und ein schließendes Tag.
Innerhalb des öffnenden Tags muss das Attribut "type="submit"" angegeben werden um klar zu machen, dass es sich hierbei um den Absende-Button handelt.
Zwischen den öffnenden und dem schließenden Tag, kann man wieder einen beliebigen Text einfügen, der dann auf dem Button angezeigt wird.
	
`<button type="submit">Jetzt abschicken!</button>`
	

## Die Fertige Kontaktformular Struktur:
Das Formular ist jetzt fertig, um es funktionsfähig zu machen wird PHP benötigt!

```html
<form method="post"> 
  <label>Name:</label> 
  <input type="text" name="name"> <br> 
  <label>E-Mail:</label>
    <input type="email" name="email" required> <br> 
  <label>Betreff:</label> 
  <input type="text" name="betreff"> <br> 
  <label>Nachricht:</label> 
  <textarea rows="7" name="nachricht" required></textarea> <br> 
  <button type="submit">Jetzt abschicken!</button> 
</form>
```
	
	
## Sonstiges Nützliches:

Drop-Down-Menü erstellen:

```html
<div>
  <label>
    Titel:
    <select>
      <option> </option>
      <option>Herr</option>
      <option>Frau</option>
      <option>Inter</option>
      <option>Divers</option>
    </select>
  </label>
</div>
```

Radio Buttons (immer nur einer auswählbar):
Damit hier nur einer der Buttos klickbar ist, muss bei dem Attribut Name immer der selbe Name vergeben werden!
Wird der andere Button geklickt, wählt sich der erste wieder ab.

```html
  <input type="radio" name="gender" value="Männlich">
  <label for="männlich">Männlich</label>
  <input type="radio" name= "gender" value="Weiblich">
  <label for="weiblich">Weiblich</label>
```
Damit immer nur ein Radio-Button ausgewählt sein kann, muss der Name gleich sein!

Mehrere Checkboxen zusammenhängend übergeben:
Wenn mehrere Checkboxen zusammenhängen sollen, muss sowohl der Name gleich sein und dahinter bei allen Checkboxen eine eckige Klammer [ ] dazugefügt werden

```html
  <input type="checkbox" name="Box[]" value="blah">
  <input type="checkbox" name="Box[]" value="blubb">
```

Wenn mehrere Checkboxen zusammen hängen sollen muss der name gleich sein und mit [] versehen werden, damit die Werte in einem Array gespeichert werden. Damit man auch weiß welche Boxen angeklickt wurden, muss ein Value angegeben werden!