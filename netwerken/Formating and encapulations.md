#term 
Wanneer een bericht wordt verzonden, moet het een specifiek formaat of specifieke structuur gebruiken.

Berichtformaten zijn afhankelijk van het type bericht en het kanaal dat gebruikt wordt
breng de boodschap over

![[Pasted image 20240512220253.png]]


# Encapsulation 

## Segmenting 
Het is het proces van uit elkaar gaanberichten in kleinere eenheden. Multiplexen wel
de processen van het nemen van meerdere stromen van gesegmenteerde gegevens en deze interleaven samen.

**twee primaire voordelen**: 
1. **Increases speed**: Grote hoeveelhedengegevens kunnen over het netwerk worden verzonden zonder een communicatieverbinding te verbreken.
2. **Increases efficiency**: Alleen segmentendie de bestemming niet bereiken, moeten opnieuw worden verzonden, niet de volledige gegevens stroom.

## Sequences 
**Sequencing messages** is het proces van nummering van de segmenten zodat de
bericht kan opnieuw worden samengesteld op de bestemming.

**TCP** is verantwoordelijk voor het sequencen van de individuele segmenten.

### Protocol Data Units
In elke fase van het proces heeft een PDU een andere naam om de nieuwe functies weer te geven. 

Er bestaat geen universele naamgevingsconventie voor PDU's.

PDU door de stapel gaan zijn als volgt: 
- Data (Data Stream)
- Segment 
- Packet 
- Frame 
- Bits( Bit Stream )