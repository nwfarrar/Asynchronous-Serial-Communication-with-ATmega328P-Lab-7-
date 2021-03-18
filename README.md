# Asynchronous-Serial-Communication-with-ATmega328P-Lab-7-
Using two ATmega328P chips, demonstrate asynchronous serial communication by following the instructions below.

Part 1 - Circuit:
Transmitter: Wire one ATmega328P as the transmitter chip. Connect a potentiometer or other analog sensor to analog pin PC0 of that chip such that the analog input varies from ~0 to ~5V.
Receiver: Wire the other ATmega328P as the receiver chip. Connect pins C0-C5 to LEDs that are in an active HIGH configuration.
Connect the Tx pin of the transmitter chip to the Rx pin of the receiver chip. Also connect the grounds of both circuits.

Part 2 - Schematic:
Sketch a schematic of your circuit that includes the LEDs, potentiometer, and corresponding ATmega328P pins, including the serial connections between them. This may be a hand sketch or a drawn sketch similar to those shown in the Lab 1 handout.

Part 3 - Programs:
Write programs for the respective chips such that the transmitter chip repeatedly reads the voltage from the analog sensor and transmits the upper eight bits (recall that the A/D converter is a 10-bit converter, so we’ll keep the upper 8 bits for transmission) to the receiver chip by asynchronous serial communication. (To be conservative in this demo you should include a delay of 50-250 msec after each transmission so that the receiver side has plenty of time to receive the data.) The receiver side must repeatedly receive the data and display it on the LEDs attached to the six bits on PortD (C0-C5). So when operating correctly, the receiver side will display the upper six bits of the 10-bit number that is captured by the A/D converter on the transmitter side.

Part 4 - Demonstration:
Demonstrate the proper functioning of your system by adjusting the potentiometer (or other analog sensor) on the transmitter side and observing the proper real-time changes in the LED display on the receiver side.
