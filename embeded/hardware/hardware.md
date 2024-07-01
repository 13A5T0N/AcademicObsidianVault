DDRX = Data Direction Register 
- hierin kunnen we aangeven of we een bepaalde pin voor input of voor output willen gebruiken

Portx  registrer = Pin Output Register 
-  hierin kunnen we effectief dan spanning aan of af zetten op de juiste pins

PINx register = Pin input Register
-  input effectief uit te lezen. Bevat een bepaalde bit een 1, dan wil dit zeggen dat er spanning op staat

struct = structures 
- manier om data te groeperen of wordt ook een recod genoemdmet onderliggende velden

# PIN

| Atmega328 Pins | Arduino numering | Multifunctional Shield |
| -------------- | ---------------- | ---------------------- |
| PB2            | 10               | led1                   |
| PB3            | 11               | led2                   |
| PB4            | 12               | led3                   |
| PB5            | 13               | led4                   |
| PC1            | A1               | button 1               |
| pc2            | A2               | button 2               |
| pc3            | A3               | button 3               |
| pd3            |                  | buzzer                 |
# DDRB
- een 8 bit register waarbij elk pin overeenkomt met een specifieke pin op 'PORTB'

| Bit   | 7   | 6   | 5   | 4   | 3   | 2   | 1   | 0   |
| ----- | --- | --- | --- | --- | --- | --- | --- | --- |
| value | 0   | 0   | 0   | 0   | 0   | 0   | 0   | 0   |
# DDRC
- gebruikt om de richting van PORTC-pinnen te configureren.
- **Bitwaarde `1`** stelt de pin in als uitvoer, **bitwaarde `0`** stelt de pin in als invoer.
```c
DDRC &= ~(1 << PC1); // configureer PC1 als input
```

```c
PORTC |= (1 << PC1); // zet pull-up weerstand aan op PC1
```

# DDRD
- om de richting van de pinnen van PORTD te configureren

# Bitwise 
bits in het `PORTB`-register worden aangepast op basis van de waarde van de `leds`-variabele.

- **`leds` variabele:** Dit is een variabele die een bitmask bevat. Het bitmask bepaalt welke bits van PORTB moeten worden gewist (op 0 worden gezet).

- **Bitwise NOT operator (`~`):** Deze operator neemt elk bit van de `leds`-variabele en keert het om. Dus 1 wordt 0 en 0 wordt 1. Bijvoorbeeld, als `leds` de waarde `0b00010000` heeft, dan wordt `~leds` `0b11101111`.

- **Bitwise AND operator (`&=`):** Deze operator voert een bitwise AND uit tussen de huidige waarde van `PORTB` en de omgekeerde waarde van `leds` (`~leds`).

- **Bitwise OR operator (`|=`):** Deze operator voert een bitwise OR uit tussen de huidige waarde van `PORTB` en het bitmask `0b00111100`

# geheugen 

- text = code
- data = variabelen met waarde 
- bss = variablen zonder waarde 
- stack = locale varaibelen en parameters 

heap
- voor dynamisch gealloceerde variabelen 
- malloc( memory allocation)
	- zoek n bytes in get geheugen 
	- wist alle gevonden bytes 
	- geeft pointer terug
- calloc( contiguous allocation)
	- geeft geheugen op plaast terug vrij 
	- geen garbage collector 