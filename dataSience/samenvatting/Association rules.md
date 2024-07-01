# Kansen

- notatie 
	- kans dat A waar is $$ P(A) $$
	- kans dat B waar is, gegeven dat A waar is $$ P(B | A)$$
	- kansen zijn getallen tussen 0 en 1 (0% en 100%)
- eigenschap
	- $$ P(A en B) = P(A) * P(B | A)$$
	- Dus :
		- P(B | A) = P(A en B) / P(A)
# Apriori algoritme

## Limiteren van combinaties
 - we zijn enkel geïnteresseerd in rules met hoge confidence
	 - confidence > min. confidence
- min. confidence is afhankelijk van de situatie
- confidence is hoog als support van (A en B) hoog is

# orange 
## Aandachtspunten
- formaat moet juist zijn
	- sparse matrix
	- enkel dingen aanduiden die gekocht zijn
	- geen waarden (? of NA) voor dingen die niet gekocht zijn
- fout formaat leidt tot foute regels
	- soms moet je pre-processen
- opletten voor transactie ids
	- mogen niet opgenomen worden in resultaten
	- best zelf verwijderen met skip of Select Columns widget
![[Pasted image 20240611043815.png]]

![[Pasted image 20240611043803.png]]

![[Pasted image 20240611043746.png]]