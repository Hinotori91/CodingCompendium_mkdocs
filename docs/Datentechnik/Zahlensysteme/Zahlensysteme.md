IPO = Input | Progressing | Output

EVA = Eingabe | Verarbeitung | Ausgabe

$$f(x) = 2x + 7$$

Ausgabe = Input + Verarbeitung

|      |       |       |       |
| ---- | ----- | :---: | :---: |
| exa  | 10^18 | 2^60  |   ?   |
| peta | 10^13 | 2^50  | pebi  |
| tera | 10^12 | 2^40  | tebi  |
| giga | 10^9  | 2^30  | gibi  |
| mega | 10^6  | 2^20  | mebi  |
| kilo | 10^3  | 2^10  | kibi  |

# Dezimal
- Basiszahl 10
- Alles Links vom Komma hat positive hochstellen
- Alles rechts vom Komma hat negative hochstellen
- Wechsel des Zahlensystems ist die Änderung der Grundzahl (10)
- Zahlen gehen von 0-9

$5732,81 = 5 * 10^3 + 7 * 10^2 + 3 * 10^1 + 2 * 10^0 + 8 * 10^{-1} + 1 * 10^{-2}$

$5732,61 = 5 * 8^3 + 7 * 8^2 + 3 * 8^1 + 2 * 8^0 + 6 * 8^{-1} + 1 * 8^{-2}$ = $5 * 512 + 7 * 64 + 3 * 8 + 2 * 1 + \frac{6}{8}+ \frac{1}{64}$

# Hexadezimal
Große Binärzahlen haben den Nachteil, dass sie sehr unübersichtlich sind. Um dem Abhilfe zu schaffen hat man das Hexadezimalsystem eingeführt. Dabei werden 4-Bit Dualzahl durch ein hexadezimales Zeichen ersetzt.
Da eine 4-Bit Dualzahl 16 Zustände annehmen kann, wir aber nur 10 dezimale Zahlen kennen, hat man dem hexadezimalen Zahlensystem 6 Buchstaben hinzugefügt.

> Jede 4 Stellige Binärzahl ist mit einer einstelligen Hexadezimalzahl darstellbar
- Immer wenn die Basis erreicht ist, muss eine neue Stelle aufgemacht werden
  - von 9 auf 10
  - von 99 auf 100
  - von 1 auf 2
    - Die größte Zahl die man mit 4 (Binär) Stellen darstellen kann ist 15

**Nennwerte**: 0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F

**Basis**: 16

**Größter Nennwert**: F

**Stellenwerte**: $16^0 = 1, 16^1 = 16, 16^2 = 256$ usw.

Zum besseren Verständnis der Zählweise im hexadezimalen Zahlensystem dient diese Tabelle. Jeweils 4 Dualstellen bilden eine Hexadezimalstelle.

| Dezimal | Binär/Dual |       |       |       | Hexadezimal |
| :-----: | :--------: | :---: | :---: | :---: | :---------: |
|    0    |     0      |   0   |   0   |   0   |      0      |
|    1    |     0      |   0   |   0   |   1   |      1      |
|    2    |     0      |   0   |   1   |   0   |      2      |
|    3    |     0      |   0   |   1   |   1   |      3      |
|    4    |     0      |   1   |   0   |   0   |      4      |
|    5    |     0      |   1   |   0   |   1   |      5      |
|    6    |     0      |   1   |   1   |   0   |      6      |
|    7    |     0      |   1   |   1   |   1   |      7      |
|    8    |     1      |   0   |   0   |   0   |      8      |
|    9    |     1      |   0   |   0   |   1   |      9      |
|   10    |     1      |   0   |   1   |   0   |      A      |
|   11    |     1      |   0   |   1   |   1   |      B      |
|   12    |     1      |   1   |   0   |   0   |      C      |
|   13    |     1      |   1   |   0   |   1   |      D      |
|   14    |     1      |   1   |   1   |   0   |      E      |
|   15    |     1      |   1   |   1   |   1   |      F      |

# Binär
Dateien bestehen nur aus Binärcode (0 und 1)
Um den Inhalt einer Datei darstellen zu lassen, ist dies nur mit Binärcode oder einer 2 Stelligen Hex-Zahl möglich!

Binärcode lässt sich auch mittsl HEX kompakt darstellen, weil HEX in 4er Gruppen gebildet werden können.

|          20 22          |  HEX  |
| :---------------------: | :---: |
| 0010 0000 0010 0010 = 2 |  BIN  |


Basis 2 = nur 2 Ziffern aber mehr Stellen
| Dezimal | Binär |
| :-----: | :---: |
|    0    |   0   |
|    1    |   1   |
|    2    |  10   |
|    3    |  11   |
|    4    |  100  |
|    5    |  101  |
|    6    |  110  |
|    7    |  111  |
|    8    | 1000  |
|    9    | 1001  |
|    1    | 1010  |

$$10 = 1 * 2^3 + 0 * 2^2 + 1 * 2^1 + 0 * 2^0 = 8 + 0 + 2 + 0$$

$$7/2 = 3 -> 1$$

$$3/2 = 1 -> 1$$

$$1/2 = 0 -> 1$$

> 8 Stellige Zahl im Binärsystem = 1 Byte
> 2 Stellige Zahl im Hexadezimalsystem = 1 Byte

# Bit (Binary Digit)
Bit stellt die die kleinste elektronsiche Speichereinheit dar
- Ein Computer kann nur mit zwei Zuständen arbeiten
  - Ja / Nein  |  Wahr / Falsch  |  1 / 0

2 Bit reichen für 4 Unterscheidungen
8 Bit = $2^8$ Informationen = 1 Byte = 256 Inforamtionen

Jedes Zeichen braucht 1 Bit egal ob Buchstabe, Zahl, Lehrzeichen etc.

# Byte
8 Bits ergeben zusammen ein Byte. Ein Byte ist damit die kleinste Datenmenge. Da jedes Bit zwei verschiedene Zustände annehmen kann, ergeben sich auch verschiedene Kombinationsmöglichkeiten, wenn Sie 8 Bits zu einem Byte zusammenfassen. Jede Kombination steht für eine bestimmte Zahl oder einen Buchstaben. So könnte die Kombination 01000001für den Buchstaben A stehen.

# ASCII (American Stadard Code for Information Interchange)
- 7 Bit Zeichencodierung
- 128 Zeichen
  - 95 druckbare Zeichen
  - 33 nicht druckbare Zeichen

- Wörterbuch bzw. Umrechnungstabelle von Zahlen in Symbole
- Die Art und weiße wie Computer Text versteht
- Für welchen Buchstaben steht diese Zahl
- 7 Bit 128 Möglichkeiten
- Pro Byte nur 7 Bit verwenden und ein Kontroll-Bit verwenden
  - Wenn nicht das richtige rauskommt ist ein Datenfehler passiert
  - Kontrollziffern
    - Wenn eine Zahl oder ein Wert (eine Information) übertragen wird besteht die Gefahr das daten verloren gehen
    - Redundant gespeichert und redundant übertragen
      - Redundant = mehr Information als unbedingt notwendig
      - Absicherung falls Information verloren geht
      - Kann mit Fehlerkorrektur hilfreich sein
    -  Ich kann Übertragungsfehler erkennen wenn die Kontrollziffer nicht stimmt

# ANSI
- 8 Bit Zeichencodierung

- In Windows eingeführte Tabelle zur Erweiterung von ASCII
- ANSI ist ASCII+
- Solange 1 Byte pro Symbol vorhanden ist komme ich nicht über 255 Zeichen drüber!
  - Somit gab es auch oft für jede Sprache eine eigene Codepage
- Unicode - 2 Byte oder mehr (UTF8/UTF16)
  - Eine Riesige Codepage die alles vereint
