# Box Modell
Jedes Rechteck ist definiert für breite, höhe, padding und margin, auch über die Stärke des Borders!


```CSS
dif {
	box-sizing: border-box;     //wird mittlerweile global bei * reingeschrieben 
                              und nicht mehr in die dif's
	background-color: #999;     // 100% breite Box trotz Border, margin und 
                              padding => ganze Seitenbreite
	width: 100%;                // 100% weil man nicht weiß wie groß der 
                              Bildschirm des Betrachters ist
	height: 300px;
	padding: 10px;              // Bei padding margin und border weren jeweils 
                              10px links und rechts dazu gegeben!
	margin: 10px;               // Kann man auch weglassen damit es von einer 
                              Bildschirmseite zur anderen geht ohne einen Abstand
	border: 10px solid #000;
}

```

![BoxModel](css-box-model.png)
# Flexbox
- Gegenstände werden zu Flex-Items!
- Alle Gegenstände werden automatisch nebeneinander angeordnet
- Modifizierung möglich damit ich die Richtung ändern kann, zb. Von oben nach unten oder von Rechts nach Links aber auch von unten nach oben möglich!
- Man kann mit der Flexbox entweder horizontal oder vertikal arbeiten!

- Braucht ein Eltern-Element das es zu einer Flexbox wird!
wenn das Eltern-Element aktiv ist, werden die anderen Elemente zu Flex-Items
Mit mehr Div Elementen, rücken die Elemente trotz vorab definierter Breite zusammen bis es sich nicht mehr ausgeht!
!Flexbox ist das erste Werkzeug für responsives Webdesign!

Um ein Element zu einer Flexbox/einem Flex-Container zu machen wird der html-Tag in CSS mit `display:flex` definiert.

Es kann auch die Anordnung der Flex-Items innerhalb einer Flexbox gereiht bzw die Richtung angegeben werden in der sie gelistet werden. Wenn die Flex-Items untereinander gereit werden sollen, benutzt man `flex-direction:column`. Sonst werden die Elemente nebeneinander gereiht solange Platz im Container ist und anschließend in die nächste Zeile umgebrochen.

> jusitify-content:center;
> - Zentriert die Attribute in der Flexbox
> verteilt die Elemente anhand der Hauptachse -> Zentriert
> justify-contnt: space-evenly;
> - Elemente werden gleichmäßig auf der verfügbaren Fläche verteilt
> justify-content: space-between;
> - Alles was an leeraum da ist, wird gleichmäßig zwischen die Elemente aufgeteilt
> justify-content: Space-around;
> - Der anfang und end abstand ist kleiner als zwischen den Elementen
> - Die Abstände teilen sich links und rechts der Elemente auf

# Grid