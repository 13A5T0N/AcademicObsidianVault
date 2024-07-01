# number 
```c
// Functie om een specifieke LED uit te zetten op basis van het LED-nummer

void lightDownLed(int ledNumber)

{

    if (ledNumber < 0 || ledNumber > 3) return; // Controleer of het LED-nummer binnen het bereik ligt

    PORTB |= (1 << (PB2 + ledNumber)); // Zet de betreffende pin hoog (1) om de LED uit te zetten

}
```

# byte
```c
// Functie om een combinatie van LEDs uit te zetten op basis van de gegeven byte

void lightDownLeds(uint8_t leds)

{

    PORTB |= leds; // Zet de betreffende pinnen hoog (1) om de opgegeven LEDs uit te zetten

}
```

# allemaal 
```c
// Functie om een combinatie van LEDs uit te zetten op basis van de gegeven byte

void lightDownAllLeds()

{

    PORTB |= 0b00111100; // Zet alle pinnen van de LED-uitvoer hoog (1) om alle LEDs uit te zetten

}
```
