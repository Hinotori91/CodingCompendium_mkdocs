# DORA - Prinzip
D - Discover
O - Offer
R - Request
A - Acknowledge

Port 67, 68

In der Netzwerktechnik bezieht sich DORA normalerweise auf einen Prozess im DHCP (Dynamic Host Configuration Protocol). DHCP ist ein Protokoll, das die automatische Zuweisung von IP-Adressen und anderen Netzwerkkonfigurationen an Geräte in einem Netzwerk ermöglicht.

- Discover (Entdecken): 
    - Ein Gerät, das sich mit dem Netzwerk verbinden möchte und eine IP-Adresse benötigt, sendet ein DHCP-Discover-Paket an das Netzwerk. Dieses Paket fragt nach verfügbaren DHCP-Servern.

- Offer (Angebot): 
    - Die DHCP-Server im Netzwerk empfangen das Discover-Paket und antworten mit einem DHCP-Offer. Dieses Angebot beinhaltet eine IP-Adresse und andere Netzwerkkonfigurationen, die dem anfragenden Gerät zugewiesen werden können.

- Request (Anfrage): 
    - Nachdem das anfragende Gerät ein DHCP-Offer erhalten hat, wählt es eine der angebotenen IP-Adressen aus und sendet eine DHCP-Request-Nachricht an den ausgewählten Server. Dies ist eine formelle Anfrage, die besagt, dass das Gerät die angebotene Konfiguration akzeptiert.

- Acknowledge (Anerkennen): 
    - Der DHCP-Server erhält die DHCP-Request-Nachricht und bestätigt die Zuweisung der angefragten IP-Adresse und Konfiguration, indem er eine DHCP-Acknowledgement-Nachricht zurücksendet. Dadurch akzeptiert das Gerät offiziell die zugewiesene Netzwerkkonfiguration.

DORA beschreibt also den Prozess der IP-Adresszuweisung durch den DHCP-Server an ein Gerät, das sich mit einem Netzwerk verbinden möchte.

## UNC (Uniform Naming Convention)
//`Servername oder IP-Adresse` \ `Ordner-Name`