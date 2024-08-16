This project implements a directional light system for a vehicle using an STM32 microcontroller. The system has three main lights: left directional light (D3), right directional light (D4) and emergency or parking lights, controlled by three buttons.

Left light (D3): Activated by pressing button S1. A single press causes the light to flash three times; pressing twice or more times quickly activates the light indefinitely. If the right light is active, it is deactivated when this button is pressed.

Right Light (D4): Functions similarly to the left light, activated by button S2, and also flashes three times or indefinitely depending on the number of presses.

Emergency Lights: Activated by button S3, causing both directional lights to flash simultaneously indefinitely, indicating an emergency situation. The emergency lights are deactivated if either directional button is pressed.

The system includes a UART interface that sends messages to the computer when the buttons are pressed, providing real-time feedback. The lights flash at a frequency of 2 Hz (250 ms per cycle), and the code uses a circular buffer to handle efficient UART communication .

