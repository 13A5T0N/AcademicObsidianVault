#osi 

# Doel 
verantwoordelijk voor communicatie tussen eindapparaat netwerkinterfacekaarten

 Het geeft toegang tot protocollen van de bovenste laag de fysieke laagmedia en
kapselt Layer 3-pakketten in (IPv4 en IPv6) in Layer 2-frames

voert foutdetectie uit en verwerpt corrumpeert frames

Bestaat uit twee sublayers:
- Logical Link Control (LLC): communiceert tussen de netwerksoftware op de bovenste lagen en de apparaathardware op de onderste lagen
- Media Access Control (MAC): is verantwoordelijk voor gegevensinkapseling en mediatoegang controle

## Protocols 
- Institute for Electrical and Electronic Engineers (IEEE).
- International Telecommunications Union (ITU).
- International Organizations for Standardization (ISO).
- American National Standards Institute (ANSI).

# IEEE 802 LAN/MAN Data Link Sublayers

zijn specifiek voor het type netwerk:
- Ethernet 
- LAN 
- WAN 
- WPAN

# Topology 

Er worden twee soorten topologieën gebruikt bij het beschrijven van netwerken:
- Physical topology: toont fysieke verbindingen en hoe apparaten zijn met elkaar verbonden.
- Logical topology: identifies the virtual connections between devices using device interfaces and IP addressing schemes.



# Full duplex 
- Hiermee kunnen beide apparaten tegelijkertijd verzenden en ontvangen op een gedeeld medium
- Ethernet-switches werken in full-duplexmodus
# Halve duplex 
- Hiermee kan slechts één apparaat tegelijk verzenden of ontvangen op een gedeeld medium
- Gebruikt op WLAN's en oudere bustopologieën met Ethernet-hubs

# Acces method 

## Contention based 
Alle nodes werken in half-duplex en concurreren om het gebruik van het medium vb:
- Carrier sense multiple access with collision detection (CSMA/CD)
- Carrier sense multiple access with collision avoidance (CSMA/CA)

### CSMA/CD
- gebruikt door legacy Ethernet lans 
- Beheer in halve duplex 
- gebruikt collission detection om te bepalen wanneer en wat een device iets kan sturen 

#### CSMA/CD collision detection process
- Devices die gelijktijdig verzenden zal resulteren in een signaalbotsing op het gedeelde netwerk media.
- Device detecteerd de botsing 
- Device wacht op een random tijd om weer te sturen 

### CSMA/CA
- gebruikt doorIEEE 802.11 WLANs
- beheert in halve duplex 
- gebruikt collision avoidance 

#### CSMA/CA collision avoidance process
- Bij het zenden houden apparaten ook rekening met de tijdsduur die nodig is voor het verzenden overdragen.
- Andere apparaten op het gedeelde medium ontvangen informatie over de tijdsduur en weten dan hoe lang het medium niet beschikbaar zal zijn
## Controlled based 
- Deterministische toegang waarbij elk node zijn eigen tijd op het medium heeft
- Used on legacy networks such as Token Ring and ARCNET


# frame

drie delen:
1. Header 
2. Data 
3. trailer 
![[Pasted image 20240603202243.png]]
![[Pasted image 20240603202301.png]]





