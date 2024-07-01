# number
```c
// Functie om een specifieke LED aan te zetten op basis van het LED-nummer

void lightUpLed(int ledNumber)

{

    if (ledNumber < 0 || ledNumber > 3) return; // Controleer of het LED-nummer binnen het bereik ligt

    PORTB &= ~(1 << (PB2 + ledNumber)); // Zet de betreffende pin laag (0) om de LED aan te zetten

}
```


## Byte
```c
// Functie om een combinatie van LEDs aan te zetten op basis van de gegeven byte

void lightUpLeds(uint8_t leds)

{

    PORTB &= ~leds; // Zet de betreffende pinnen laag (0) om de opgegeven LEDs aan te zetten

}
```

## allemaal 
```c
// Functie om alle LEDs aan te zetten

void lightUpAllLeds()

{

    PORTB &= ~(0b00111100); // Zet alle pinnen van de LED-uitvoer laag (0) om alle LEDs aan te zetten

}
```
