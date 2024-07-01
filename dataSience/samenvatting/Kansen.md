# Slaagkans 
- 2 mogelijkheden 

## Volgens laplace 
- P(gebeurtenis) = aantal gunstige uitkomsten / aantal mogelijke uitkomsten 
- notatie = P()
	- vb: P(regen), P(ziek)
- Kans * 100 = precent 
	- notatie  = %
- g = gebeurtenis 
- u = uitkomsten 
```mathpad
%$2:=P*g=g*u^(-1)
P*g=g*u==?
```

## Voorwardelijke kansen 
- afhangen van bepaalde kennis 
```mathpad
P(niet A) = 1 - P(A)=~?
```



# Rekenen 

## inversie
$$
P(niet G) = 1 - P(G)
$$

- Notaties
	- G = gebeurtenis 

### VB:
 kans dat het regent is 55%, wat is de kans dat het niet regent?
 - P(regent niet) = 1 - P(regent) = 1 - 0,55

## Product regel 

- gebeurtenis zijn onafhanklijk 
$$ 
P(A|B)=P(A)
$$
### VB:  
kans dat iemand een rode T-shirt draagt en kans dat iemand goed is in wiskunde
$$
P(rood En Wiskunde)
= P(rood) * P(wiskunde / rood)
= P(rood) * P(wiskunde)
$$
## SomRegel 
### Formule 
$$
P(A of B) = P(A) + P(B) - P(A en B)
$$
### VB: 
wat is de kans dat een willekeurig kind een meisje is OF een bril draagt (of allebei)
$$
P(meisje OF bril) = P(meisje) + P(bril) - P(meisje EN bril) = 0,4 + 0,1 - 0,08 = 0,42 = 42%
$$

## Regel van Bayes 
### Formule 
$$
P( A∣B)= P(B∣A)*P(A)/P(B)
$$

### VB
gegeven een tekst, wat is de kans dat deze spam is
$$
P(spam | woorden) = P(woorden | spam) * P(spam) / P(woorden)
$$
