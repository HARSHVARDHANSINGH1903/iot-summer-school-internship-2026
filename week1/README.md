# Dynamic LED Blink System

## Hardware Required
* Arduino Uno (or compatible microcontroller)
* 1x 5mm LED (Any color)
* 1x 220Ω Resistor
* 1x 10kΩ Potentiometer
* Breadboard and Jumper Wires

## Circuit Diagram Description
1. **LED:** Connect the anode (longer leg) to digital pin 13. Connect the cathode (shorter leg) through a 220Ω resistor to the GND pin.
2. **Potentiometer:** Connect the outer left terminal to 5V. Connect the outer right terminal to GND. Connect the middle wiper terminal to analog pin A0.

## How to Upload Code
1. Open the Arduino IDE.
2. Connect your Arduino board to your computer via USB.
3. Navigate to `Tools > Board` and select your specific board (e.g., Arduino Uno).
4. Navigate to `Tools > Port` and select the active COM port.
5. Open the `blink.ino` file, click the **Verify** (checkmark) button, and then click **Upload** (right arrow).

## Expected Output
Once uploaded, the LED will begin to blink. Opening the Serial Monitor (set to 9600 baud) will display the current blink count. Turning the potentiometer knob will dynamically increase or decrease the blinking speed in real-time.

## Troubleshooting Tips
* **LED not lighting up:** Check the polarity of the LED; it may be plugged in backward. Ensure the resistor is properly seated.
* **Code fails to upload:** Verify that the correct board and COM port are selected in the Arduino IDE Tools menu. Ensure the USB cable supports data transfer, not just power.
* **Blink speed does not change:** Ensure the middle pin of the potentiometer is firmly connected to A0, and the outer pins are receiving 5V and GND.




Q9)
git clone: Downloads a complete, independent copy of a remote repository from GitHub to your local computer.
When to use: Only once, when you are first setting up a project on a new machine.
git fetch: Downloads the latest updates and history from the remote repository but does not modify or merge them into your current working files.
When to use: When you want to safely check what changes your teammates have made before deciding to integrate them.
git pull: Downloads the latest updates from the remote repository and immediately merges them into your local files (fetch + merge).
When to use: When you want to quickly update your local workspace to match the latest version on GitHub.


Q10)
What is it? A .gitignore file is a plain text file that tells Git exactly which files or folders it should ignore. This prevents temporary files, compiled binaries, or sensitive passwords from being accidentally uploaded to your public repository.
The requested .gitignore content:

# Compiled output files
*.hex
*.elf

# OS-specific files
.DS_Store
Thumbs.db

# IDE config folders
.vscode/
build/
