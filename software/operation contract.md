- Operation Contracts beschrijven hoe de interne staat van de concepten in het Domain Model veranderen door het uitvoeren van een operatie.
 - Input 
	 - De concepten en associaties van het Domain Model
	 - De system events die getoond worden op het SSD
- Output 
	- Een mini-contract per operation waarbij vooral de beschrijving van POST-conditie relevant is
![[Pasted image 20240607023621.png]]

# Werkwijze 
1. Bepalen welke operaties er zijn in één UC/SSD
	- Alle volle pijlen in SSD = input messages
	- Operaties hebben dezelfde namen als input messages, en bevatten de reacties op deze vraag
2. Bepalen postcondities
	- We vermelden enkel systeemveranderingen in OC postcondities (⇔ UC postcond.)
		- Een OC focust op systeem, niet het UC-proces
		- Drie soorten van postcondities
			- Instantie creaties en verwijderingen
			- Link creaties en verwijderingen
			- Veranderingen in attribuutwaarden
3. Bepalen precondities
	- Bepaal de precondities op basis van de postcondities: wat moet er bestaan voor de operatie om deze correct te kunnen uitvoeren
	- We vermelden enkel systeemstatus in OC precondities (⇔ UC precondities)
