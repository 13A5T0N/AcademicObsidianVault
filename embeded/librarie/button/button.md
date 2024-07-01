```c
// Functie om een knop in te schakelen

void enableButton(int number){

    // Configureer de pin als ingang door de betreffende bit te resetten

    // Het bitnummer wordt berekend door PC1 op te tellen bij het nummer van de knop

    DDRC &= ~(1 << (PC1 + number));

  

    // Activeer de pull-up weerstand voor de betreffende pin

    PORTC |= (1 << (PC1 + number));

}
```

# pushed
```c
// Functie om te controleren of een knop is ingedrukt

int buttonPushed(int button)

{

  uint8_t buttonBit = (1 << (PC1 + button));

  if (~PINC & buttonBit)

  {

    // printString("button pushed!");

    return 1;

  }

  else

  {

    // printString("button NOT pushed!");

    return 0;

  }

}
```
De bitwise NOT-operator `~` keert alle bits om. Bijvoorbeeld, als `PINC` gelijk is aan `0b00001111`, dan is `~PINC` gelijk aan `0b11110000`

