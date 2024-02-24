Hello! This is a project I wanted to make for a while to test my skills with STM.

The things I used are: STM32 board with NUCLEO-F091RC, NTC thermistor, red LED, blue LED, 2x 110 ohm resistors for LEDs, 10k ohm resistor for thermistor.

The code (you can find it in the files) uses ADC convertor to measure the voltage on the NTC thermistor, the value is then compared to 2000 (I didn't want to make a conversion from voltage to temperature because it was useless) and if the value is less than 2000 the blue LED turns on indicating that it's a low temperature in the room, else the red LED turns on indicating there is a higher temperature that the one used for reference (in my case 2000).

The B1 button on the board is used to raise the value of temperature by 100 mV (only the value is modified, not the voltage on the thermistor) and it can onyl be reset using the reset button on the board.

The IDE I used is STM32CubeIDE so I think it can work for you, too.

The pinout for the microcontroller: https://os.mbed.com/platforms/ST-Nucleo-F091RC/
