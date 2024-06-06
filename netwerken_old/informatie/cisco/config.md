#config #info 
## Twee type configuratie 
1. **startup-config**: Dit is het opgeslagen configuratiebestand dat is opgeslagen in NVRAM. Het bevat alle opdrachten die door het apparaat worden gebruikt bij het opstarten of opnieuw opstarten. Flash verliest zijn inhoud niet wanneer het apparaat wordt uitgeschakeld.
2. **running-config**: Dit wordt opgeslagen in Random Access Memory (RAM). Het weerspiegelt de huidige configuratie. Het wijzigen van een actieve configuratie heeft onmiddellijk invloed op de werking van een Cisco-apparaat. RAM is vluchtig geheugen. Het verliest alle inhoud wanneer het apparaat wordt uitgeschakeld of opnieuw wordt opgestart.
## Note 
Als de stroom naar het apparaat uitvalt of als het apparaat opnieuw wordt opgestart, gaan alle configuratiewijzigingen verloren, tenzij ze zijn opgeslagen. Om wijzigingen in de actieve configuratie op te slaan in het opstartconfiguratiebestand, gebruikt u de opdracht copy running-config startup-config bevoorrechte EXEC-modus.