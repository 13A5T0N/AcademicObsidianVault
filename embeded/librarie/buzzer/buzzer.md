# enable 
```c
void enableBuzzer() { DDRD |= (1 << PD3); } // buzzer hangt op PD3
```

# play 
```c
void playTone(float frequency, uint32_t duration)

{

    uint32_t periodInMicro = (uint32_t)(1000000 / frequency); // we berekenen de periode in microseconden uit de frequency

    uint32_t durationInMicro = duration * 1000;               // we willen duration in microseconden

    for (uint32_t time = 0; time < durationInMicro; time += periodInMicro)

    {

        PORTD &= ~(1 << PD3);         // aanzetten van de buzzer

        _delay_us(periodInMicro / 2); // helft van de periode wachten

        PORTD |= (1 << PD3);          // afzetten van de buzzer

        _delay_us(periodInMicro / 2); // weer helft van de periode wachten

    }

}
```
