#osi 

# Responsibilities

- Het volgen van individuele gesprekken
- Gegevens segmenteren en opnieuw samenstellen
- Voegt headerinformatie toe
- Identificeer, scheid en beheer meerdere gesprekken
- Maakt gebruik van segmentatie en multiplexen om verschillende mogelijk te maken communicatiegesprekken te zijn interleaved op hetzelfde netwerk

# Transmission Control Protocol(TCP)
- Nummer en volg gegevenssegmenten verzonden naar een specifieke host van een specifieke toepassing
- Ontvangen gegevens bevestigen
-   Verzend onbevestigde berichten opnieuw gegevens na een bepaalde hoeveelheid 
- Sequentiegegevens die mogelijk binnenkomen in verkeerde volgordetijd
- Verzend gegevens tegen een efficiënte snelheid aanvaardbaar is voor de ontvanger

## Overview
-  Establishes a Session: TCP is een verbindingsgericht protocol dat onderhandelt en brengt een permanente verbinding (of sessie) tot stand tussen bron- en bestemmingsapparaten voordat er verkeer wordt doorgestuurd
- Ensures Reliable Delivery
- Provides Same-Order Delivery
- Supports Flow Control

![[Pasted image 20240603203659.png]]
## Connection Establishment
1. The initiating client requests a client to-server communication session with the server
2. The server acknowledges the clientto-server communication session and requests a server-to-client communication session
3. The initiating client acknowledges the server-to-client communication session
![[Pasted image 20240603203924.png]]
## Session Termination
1. When the client has no more data to send in the stream, it sends a segment with the FIN flag set.
2. : The server sends an ACK to acknowledge the receipt of the FIN to terminate the session from client to server
3. The server sends a FIN to the client to terminate the server-to-client session
4. The client responds with an ACK to acknowledge the FIN from the server
![[Pasted image 20240603204012.png]]
# User Datagram Protocol (UDP)
Udp is connectionless 

biedt de basisfunctiesvoor het leveren van datagrammen tussen
de juiste toepassingen, metzeer weinig overhead en data controleren
![[Pasted image 20240603203502.png]]

# Port Number Groups
![[Pasted image 20240603203732.png]]


![[Pasted image 20240603203744.png]]