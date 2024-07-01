# Enable 
## number
```c
// Functie om een specifieke LED te activeren op basis van het LED-nummer

void enableLed(int ledNumber)

{

    if (ledNumber < 0 || ledNumber > 3) return; // Controleer of het LED-nummer binnen het bereik ligt

    DDRB |= (1 << (PB2 + ledNumber)); // Zet de betreffende pin als uitvoer (1) voor de opgegeven LED

}
```
# byte
```c
// Functie om een combinatie van LEDs te activeren op basis van de gegeven byte

void enableLeds(uint8_t leds)

{

    DDRB |= leds; // Zet de betreffende pinnen als uitvoer voor de opgegeven LEDs

}
```

## All
```c
// Functie om alle LEDs te activeren

void enableAllLeds()

{

    DDRB |= 0b00111100; // Zet alle pinnen van de LED-uitvoer als uitvoer

}
```

ref:
- [[hardware]]
