# Stappen 
1. Bepaal welke operaties het onderwerp is 
	- aanduiden met een pijl links boven aan 
	- volle pijl
2.  Bepaal returnwaarde van de operatie
	- zet links onderaan 
	- alle interacties tekenen om return waarde 
	- gestippeld lijn
3. Bepaal volgorde van operaties
	- bepaal de parameters 
	- Operatie = activatielijn op balk 
	- 1 gestippelt van returnwaarde
![[Pasted image 20240607020245.png]]
# Activaite balk 
- aanduiding om aan te geven dat instantie actief is 

# Boodschap 

## Synchrone 
- volle lijn 
- Eindigt met een volle pijl 
- naam boven op de lijn 
## Asynchroen 
- volle lijn 
- Eindigt met een open pijl 
- aanroeper hoeft niet te wachten op een boodschap 
## Antwoord 
- gestippelt lijn 
- Eindigt met een open pijl 
- omgekeerde richting 
- naam boven op de lijn 
## Create
- gestippeld lijn 
- << create >> (:argumenten)
- pijl eindigt, start de levenslijn van het nieuwe object 
![[Pasted image 20240607021612.png]]

## Destroy 
- gestippeld lijn 
- << destroy >>(:argument)
- pijl eindigt, stopt de levenslijn van het object 
![[Pasted image 20240607021804.png]]

# Frame
- groot vierkant volle lijn
- kleine box links boven 
![[Pasted image 20240607022214.png]]
# Fragment 
- grote vierkant volle lijn 
- operator in de kleine box links boven 
- condetioneel gedrag te noteren 
- gaurd binnen het fragment 
![[Pasted image 20240607022225.png]]


| Frame Operator    | Beschrijving                           |
| ----------------- | -------------------------------------- |
| loop              | over het fragment zolang guard WAAR is |
| alt(alternatief ) | voert optionele fragment uit           |
| opt(optionele)    | voert uit wanneer gaurd waar is        |
| break             | om een loop te breken                  |
| ref(reference )   | verwijst naar een andere SD            |
| par               | fragment voert uit in parallel         |
|                   |                                        |
