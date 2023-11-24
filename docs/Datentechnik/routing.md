# Routing
Ip ist ein Routbares Protokoll das mittels Routern weitergeleitet wird. Für das Routing gibt es 2 Varianten entweder statisch oder dynamisch. Beim dynamischen Routing gibt es Routingprotokolle. Die Wegwahl (Metrik) basiert auf Hop-Count, Bandbreite, Latenz, usw.  Sowohl IP als auch die Routingprotroklle (RIP OSPF BGP=Routingprotokoll für die Provider) arbeiten auf dem OSI-Layer 3.

## 3. Layer Netzwerklayer
- IP Protokoll
  - ist ein Routbares Protokoll
  - Router ist da wichtigste Gerät auf dem 3. Layer
    - Schickt IP-Pakete durch die gegend
    - Private und Öffentliche Adressen
    - ist zuständig für die Wegfindung
      - RIP - Routing Information Protokoll
        - Dynymische Routing Protokoll
          - Statisch
            - Weniger flexibel weil manuelle eingabe
          - Dynamisch
            - Wenn sich etwas verändert dann wird das automatisch mit rein gerechnet
            - Routing Protokoll
              - Link State
                - OSPF (Open-Shortest-Path-First)
              - Distance Vector
                - Rip
                  - Distanze Vector
                    - Die potentielle Richtiung in die das Datenpakete gesendet werden
                    - die Beste Metrik (Richtung mit der gerinsten Zahl) wird ausgewählt
  
        - Haupt Count (Hops)
        - Metrik
          - `OSPF - Open Shortest Path First (Protokoll)`
            - Misst die Bandbreite und nimmt den schnellsten Pfad
            - Parameter wie der Pfad gefunden werden soll
              - Algorithmus für den kürzesten weg ist ein teil des OSPF
            - Link Status (Verbindung) 
              - welchen Status hat der Link
              - ein status ist die Geschwindigkeit
                - Bandbreite
                  - Ist die Menge der Daten die übertragen werden
                - Verzögerung (Latenz)
                  - ist die Zeit wie lange es dauert
                - Auslastung
                - Zuverlässigkeit
                - Kosten
              - Fließt in eine Datenbank mit dem Algorithmus `Dijkstra`
                - Dijkstra rechnet den weg aus
  - Routing - Protokolle
    - Schauen in die IP Pakete und schicken es in die richtige richtung
      - Entscheidungen werden getroffen wohin die Pakete geschickt werden... auch in welches netz es geschickt wird



# Routing
Routing bezeichnet die Wegfindung von Daten einer Quelle zu einem definierten Ziel.
IP Router kennt die Gnaze Netzwerktopologie als auch einzelne Verbindungswege.
- `Routing`: 
  - Weiterleiten von Datenpaketen in einem Computernetzwerk
- `Router`: 
  - zentrales Gerät für das Routing
- `Routing-Protokolle`: 
  - ermöglichen Informationsaustausch zwischen Routern
- `Netzwerktopologie`: 
  - Berücksichtigung der Netzwerkstruktur
- `Bandbreitenkapazitäten`: 
  - Einbeziehung der verfügbaren Datenübertragungsraten
- `Latenzzeiten`: 
  - Berücksichtigung der Verzögerungen bei der Datenübertragung
- `Metriken`: 
  - Faktoren zur Bewertung der Netzwerkpfade
- `Engpässe vermeiden`: 
  - Verteilung des Datenverkehrs zur Ressourcennutzungsoptimierung
- `Routing-Algorithmen`: 
  - z.B. BGP, RIP
- `Routing-Tabellen`: 
  - Aktualisierung der Routing-Informationen in den Routern
- `Ziel`: 
  - zuverlässige und schnelle Datenübertragung
- `Internet`: 
  - Border Gateway Protocol (BGP)
- `Kleinere Netzwerke`: 
  - Routing Information Protocol (RIP)
- `Effiziente und sichere Datenübertragung`


EGP (Exterior Gateway Protocol):
- Protokoll für das Routing zwischen autonomen Systemen im Internet
- Ermöglicht den Austausch von Routing-Informationen zwischen verschiedenen autonomen Systemen
- alles was mit Öffentlichen adressen in einem netzwerk zu tun hat
- Ziel ist es den besten weg zu finden

IGP (Interior Gateway Protocol):
- Protokolle zur Kommunikation zwischen Routern innerhalb eines autonomen Systems
- Beispiele: RIP, OSPF
- alles mit Privaten adressen in einem Netzwerk zu tun hat
- Ziel ist es den besten weg zu finden

RIP (Routing Information Protocol):
- Ein IGP-Protokoll für kleine Netzwerke
- Verwendet Distanzvektor-Algorithmus zur Berechnung der besten Pfade
- Begrenzte Skalierbarkeit, langsamere Konvergenzzeit

OSPF (Open Shortest Path First):
- Ein IGP-Protokoll für größere Netzwerke
- Verwendet Link-State-Algorithmus zur Berechnung der besten Pfade
- Basiert auf Informationen über den Zustand von Netzwerkverbindungen (Link States)

DV (Distance Vector):
- Eine Art von Routing-Algorithmus
- Basierend auf der Bewertung von Entfernungen (Distanzen) zu Zielen
- Routertabellen werden auf der Grundlage der besten Pfade aktualisiert

Link State:
- Routing-Algorithmus, der Informationen über den Zustand aller Netzwerkverbindungen kennt
- Router teilen sich gegenseitig ihre Link States mit, um Routing-Tabellen zu aktualisieren

BGP (Border Gateway Protocol):
- EGP-Protokoll für das Routing zwischen autonomen Systemen im Internet
- Verwendet Pfadvektor-Algorithmus zur Berechnung der besten Pfade
- Hohe Skalierbarkeit, schnelle Konvergenzzeit
- Verantwortlich für das Routing zwischen Internet Service Providern (ISPs) und die Weiterleitung von Internetverkehr


