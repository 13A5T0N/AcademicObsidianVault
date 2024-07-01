- beslissingsbomen zijn een voorbeeld van supervised learning
- het is een classificatietechniek
# Stap 1: discretiseren
- variabelen moeten discreet zijn
- niet te veel verschillende waarden
- we zetten alles om naar nominaal en ordinaal meetniveau
- hoe kan je een continue variabele omzetten naar een discrete met ordinaal meetniveau? (hint: [[frequenties]])
## Orange 
1. import file 
2. select columns 
	- Target Aangeven 
	- ![[Pasted image 20240611035523.png]]
3. Tree
	- ![[Pasted image 20240611035604.png]]
4.  Tree viewer
	- ![[Pasted image 20240611035655.png]]

![[Pasted image 20240611035413.png]]

# Entropie en information gain 
## Entropie
- maat voor "chaos" in de kolom met resultaten (de “afhankelijke variabele” of “target”)
- allemaal dezelfde waarde: E(target)=0
- formule
	- $$ E(target)= ∑ target waarden −( p/n)⋅log2 ( p/n) $$
		- p = aantal rijen met de gegeven waarde in de target kolom
		- n = aantal rijen in de tabel
		- p/n is dus de relatieve frequentie van de waarde in de target kolom
### Vb:
- voorbeeld (simpsons heeft 4 vrouwen en 5 mannen):
$$ E(simpsons) = -(4/9)*log2(4/9)-(5/9)*log2(5/9)$$
## information gain 
- zoek de kolom met het grootste “onderscheidend vermogen”
- vergelijk met correlatie maar dan voor nominale variabelen
- Formule
	- $$ Gain(kolom)=E(target)− ∑ waarden vankolom ( p/n)⋅E(targetsubtabel) $$
		- “subtabel” bevat enkel een bepaalde waarde voor de gegeven kolom
		- p is het aantal rijen in de subtabel
		- n is het totaal aantal rijen in de tabel
		- p/n is dus de relatieve frequentie van de waarde in de kolom
		- E(tabel) is de entropie van die tabel



## orange 
- Import 
	- werkt enkel met categorische variabelen
	- ![[Pasted image 20240611035911.png]]
- Formila 
	- ![[Pasted image 20240611035949.png]]
- Rank
	- ![[Pasted image 20240611040015.png]]
- Data Table 
	- ![[Pasted image 20240611040045.png]]

![[Pasted image 20240611035841.png]]



# voorspellen
- Create instance
	- ![[Pasted image 20240611040650.png]]
- Predictions 
	- ![[Pasted image 20240611040704.png]]
![[Pasted image 20240611040627.png]]

# Bossen 
- Als je door de bomen het bos niet meer ziet
- soms berekent men niet 1 boom, maar meerdere
- in plaats van de hoogste gain te nemen, neem een willekeurige kolom (hoogste gain heeft wel meer kans)
- als je nu een beslissing wil nemen: laat alle bomen beslissen en gebruik een “meerderheidsbeslissing”
## Orange
- Random Foresst 
	- ![[Pasted image 20240611040857.png]]
- Predictions 
	- ![[Pasted image 20240611040914.png]]
![[Pasted image 20240611040838.png]]