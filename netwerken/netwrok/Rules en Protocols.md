#protocol

# <span style="color:rgb(255, 255, 0)">Rules</span>
## <span style="color:rgb(229, 211, 11)">Message Encoding </span>

- Encoding: proces van het omzetten van informatie in een andere aanvaardbare vorm voor overdragen
- Decoding: keert dit proces om om de informatie te interpreteren
## <span style="color:rgb(229, 211, 11)">Message Formatting and Encapsulation</span>
-  het moet een specifiek formaat of structuur gebruiken
- formaten zijn afhankelijk van het type bericht en het kanaal dat gebruikt wordt breng de boodschap over
## <span style="color:rgb(229, 211, 11)">Message Size</span>
De codering tussen hosts moet in een geschikt formaat voor het medium plaatsvinden
- Berichten die over het netwerk worden verzonden, worden omgezet in bits
- De bits worden gecodeerd in een patroon van licht, geluid of elektrische impulsen
- De bestemmingshost moet de signalen decoderen om het bericht te kunnen interpreteren

## <span style="color:rgb(229, 211, 11)">Message Timing</span>
omvat het volgende:
- Flow Control : Beheert de snelheid van de gegevensoverdracht en bepaalt hoeveel informatie kan worden verzonden en de snelheid waarmee deze kan worden afgeleverd
- Response Timeout: Beheert hoe lang een apparaat wacht wanneer het geen antwoord hoort de bestemming
- Access method: Bepaalt wanneer iemand een bericht kan verzenden
	- Er kunnen verschillende regels gelden voor zaken als “botsingen”. Dit is wanneer er meer dan één is apparaat verzendt tegelijkertijd verkeer en de berichten worden beschadigd
	- Sommige protocollen zijn proactief en proberen botsingen te voorkomen; andere protocollen zijn dat wel reactief en stel een herstelmethode vast nadat de botsing heeft plaatsgevonden

## <span style="color:rgb(229, 211, 11)">Message Delivery Options</span>
omvat de volgende methodes:
- Unicast: één op één communicatie
- Multicast:  one to many, typically not all
- Broadcast: één voor allen

# <span style="color:rgb(255, 255, 0)">P<span style="color:rgb(255, 255, 0)">r</span>otocols </span>
## <span style="color:rgb(229, 211, 11)">Functions </span>
- Apparaten gebruiken overeengekomen protocollen communiceren
- kan er misschien een hebben of functies
![[Pasted image 20240603162127.png]]

##  <span style="color:rgb(229, 211, 11)">Segmenting</span>
Het proces van uit elkaar gaan berichten in kleinere eenheden. Multiplexen wel
de processen van het nemen van meerdere stromen gesegmenteerde gegevens en deze interleaven samen

twee primaire voordelen:
- *Increases speed*  Grote hoeveelheden gegevens kunnen over het netwerk worden verzonden zonder een communicatieverbinding te verbreken 
- *Increases efficiency* Alleen segmenten die de bestemming niet bereiken, moeten opnieuw worden verzonden, niet de volledige gegevens stroom
## <span style="color:rgb(229, 211, 11)">Sequences </span>
proces van nummering van de segmenten zodat de bericht kan opnieuw worden samengesteld op de bestemming

**<span style="color:rgb(0, 176, 240)">TCP</span>** is verantwoordelijk voor het sequencen van de individuele segmenten
