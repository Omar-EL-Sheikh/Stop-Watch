# Stop-Watch
Description: A stop-watch system that counts time in seconds with pause, resume and reset buttons using ATmega32 microcontroller.

The application uses Timer1 on ATmega32 MC with CTC mode to count time. The six 7-segments display time in (hh:mm:ss) format using the Multiplexed Technique to keep all the 7-segments visually active at the same time.

External Interrupt INT0 is connected to a push button with a pull-up resistor and set up to be triggered with a falling edge to enable an ISR that will reset timer.

External Interrupt INT1 is connected to a push button with a pull-down resistor and set up to be triggered with a rising edge to enable an ISR that will pause timer.

External Interrupt INT2 is connected to a push button with a pull-up resistor and set up to be triggered with a falling edge to enable an ISR that will resume timer.

Programming Language(s): This project is written in C programming language.

Hardware Implementation: This project is implemented on ATmega32 MC with a frequency of 1Mhz connected to the following components:

6 Common Anode 7-segments
7447 Decoder
6 NPN BJT
3 Push Buttons
Drivers:

Timer
GPIO
External Interrupt
