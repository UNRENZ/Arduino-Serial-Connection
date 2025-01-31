## Breadboard Diagram
![image](https://github.com/user-attachments/assets/73b1996a-f75d-4939-9c8d-7e1ecfdad674)

This Arduino program uses a photoresistor (LDR) connected to A0 to measure ambient light levels and control the blinking of an LED connected to pin 13. The program continuously reads the brightness value, maps it to a range of 0-255 (for LED control), and displays the mapped value on the Serial Monitor. If the brightness exceeds a threshold (220), the LED begins to blink at a rate of 100ms on and off.
The program also listens for serial input. If the word "stop" is sent from the Serial Monitor, it stops the blinking by setting the shouldBlink flag to false and turning the LED off.
