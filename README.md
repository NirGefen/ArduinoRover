# ArduinoRover
Arduino based rover with environmental sensors and RF communication.

The rover's arduino sends data that is collected from its sensors, using RF communication (NRF24 transceiver). 

A PC with another arduino and an NRF transceiver, runs the C# application.
The application receives the data from the arduino, parses the message and displays it. 
Asynchronously, it receives input from the user using the arrow keys, which designates the direction the rover should go. It then sends a message back to the arduino with the move data, which is sent to the rover using the NRF transciever.
