## Responsive Design

Für die Darstellung auf verschiedenen Geräten!
Wenn die Darstellung zu klein wird, verschwindet das Menü und es entsteht ein "Hamburger-Menü"!

- HTML:
  - Zu aller erst wird das grobe Design der Homepage erstellt
  - In der Navigationsleiste muss ein Checkbutton erstellt und eingefügt werden
  - Zusätzlich zur Checkbox muss noch das Hamburger-Menü Icon (oder ein Bild das dafür stehen soll) eingebunden werden
  - Dann gehört noch die Liste mit den Verlinkungen auf die anderen Seiten eingefügt!

- CSS:
  - In CSS wird dann die nav ul zu einer Flexbox gemacht
  - Und die Unterstriche wegen der Links entfernt
  - Die Checkbox wird unsichtbar gemacht
    - Da diese ja nur aufscheinen soll wenn das Bild zu klein für die Navigationsleiste ist
  - Mit @media (max-width : 800px) wird bekannt gegeben das sich das Bild bei einer Größe von 800 Pixel verändern soll
    - Hier wird die Checkbox wieder sichtbar gestellt
    - Und bei der Nav UL wird auch einiges umgestellt!
      - Display auf Inline-Block 
      - Position auf fixed
      - Left auf -100%
        - Damit die Leiste außerhalb es Sichtbaren Bereichs ist
      - Mit check:checked ~ ul sagt man was passieren soll wenn der Burger-Button geklickt wurde
        - Wenn der Button geklickt wurde, soll die Menü-Leiste wieder auf Ihren ursprünglichen Platz zurück rutschen
          - Left auf 0
  - Für jede weitere Verkleinerung mit @media kann alles andere verändert werden, aber nicht mehr zwingend der Burger-Button!