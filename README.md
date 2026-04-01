4-Bit Binary Counter (Experiential Learning Project):
This project is a hardware-software integration that implements a 4-bit binary counter using an Arduino. It demonstrates the conversion of decimal increments into binary output displayed via LEDs.
Key Features:
*Binary Visualization: Uses 4 LEDs to represent numbers from 0 to 15 (2^4 - 1).
*Non-Blocking Debounce: Implements a millis() based debounce logic to ensure accurate button presses without pausing the processor.
*Bitwise Logic: Utilizes bit-shifting (val >> i) and bitwise AND (& 1) to map the counter value directly to specific hardware pins.
*Pull-up Configuration: Uses INPUT_PULLUP for the button to simplify the circuit by eliminating the need for external resistors.
#Hardware Components
i) Arduino Uno 
ii) 4x LEDs (Pins 3, 4, 5, 6)
iii) 1x Push Button (Pin 2)
iv) Resistors for LEDs
Technical ImplementationThe core logic resides in the updateLEDs function, which iterates through the 4-bit range. By shifting the counter value, the code checks if each specific bit is "high" or "low" and sets the corresponding LED state accordingly
