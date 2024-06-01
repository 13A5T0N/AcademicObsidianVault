#info  #ip 
Om een eindapparaat via het netwerk te laten communiceren, moet het worden geconfigureerd met de juiste IP-adresinformatie, inclusief het standaard gateway-adres. De standaardgateway wordt alleen gebruikt als de host een pakket naar een apparaat op een ander netwerk wil sturen. Het standaardgatewayadres is doorgaans het routerinterfaceadres dat is aangesloten op het lokale netwerk van de host. Het IP-adres van het hostapparaat en het routerinterfaceadres moeten zich in hetzelfde netwerk bevinden.

![[Pasted image 20240417005122.png]]


### switch
Een switch die clientcomputers met elkaar verbindt, is doorgaans een Layer 2-apparaat. Als zodanig heeft een Layer 2-switch geen IP-adres nodig om goed te kunnen functioneren. Er kan echter een IP-configuratie op een switch worden geconfigureerd om een beheerder externe toegang tot de switch te geven.

Om verbinding te maken met een switch en deze te beheren via een lokaal IP-netwerk, moet er een virtuele switch-interface (SVI) zijn geconfigureerd. De SVI is geconfigureerd met een IPv4-adres en subnetmasker op het lokale LAN. De switch moet ook een standaard gateway-adres hebben dat is geconfigureerd om de switch op afstand te beheren vanaf een ander netwerk.

Het standaard gateway-adres wordt doorgaans geconfigureerd op alle apparaten die buiten hun lokale netwerk communiceren.