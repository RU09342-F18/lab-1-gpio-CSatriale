# Button Blink
Now that you have looked at blinking the LED from some built in delay, but what if we wanted to control the state of the LED by a button? You may think "Why would I need a Microcontroller to perform the job of a switch?". And that is where you come in. The bare minimum for this part of the lab is to essentially replicate a switch with your development board.

# YOU NEED TO CREATE THE FOLLOWING FOLDERS
* MSP430G2553
* MSP430F5529

## README
The code runs on both processors, MSP430G2553 and MSP430F5529. The code utilizes a while loop that is always true. Then an if statement checks the value of the button. The if statement ANDs the input with the button to set as a 1 or 0. If there is a 1, the button is not pressed because of a pull up resistor. If there is a 0 the button has been pressed. This satisfies the if statement to set the LED to 1.

## Extra Work
What can we do to make this a little bit more worthy of needing a microcontroller.

### Button Based Speed Control
Much like the UART controlled speed, what if you could cycle between speeds based on a button press? The speed could progress through a cycle of "Off-Slow-Medium-Fast" looping back when you hit the end.

### Color Change
What if upon a button press, the LED which was blinking changed. Some of the development boards contain two LEDs, so you could swap between a Red and a Green LED.
