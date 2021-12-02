# Blinky Project In Action

|ON|OFF|
|:--:|:--:|
|\"C:\Users\K.Anusha\Desktop\Simulation_ON.png"||\"C:\Users\K.Anusha\Desktop\Simulation_OFF.png"||

## Code 
```
	for(;;)
	{
        change_led_state(HIGH);
		delay_ms(LED_ON_TIME);
        change_led_state(LOW);
		delay_ms(LED_OFF_TIME);	
	}
```
