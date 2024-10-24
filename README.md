# Resistor Value Calculator with Nextion Display

This project is a **Resistor Value Calculator** developed using a Nextion touchscreen display. It allows users to input parameters (such as resistor bands) and calculates the resistance value in real time.

## Features

- **Intuitive User Interface**: The calculator features an easy-to-use, clean interface designed using the Nextion editor.
- **Real-time Calculation**: As users input resistor values, the calculator performs the necessary calculations instantly and displays the result.
- **Scalable Design**: The project is designed to be easily extended for additional functionality, such as adding different types of calculations or incorporating other sensor data.

## How It Works

1. **Input Fields**: Users input the number of resistor bands and the values of each band using the touchscreen.
2. **Calculations**: The calculator takes these values and performs calculations to determine the overall resistance.
3. **Display**: The result is displayed on the Nextion screen with clear formatting.

## Code Example

Here’s a code snippet demonstrating how the calculation is handled in the Nextion script:

```plaintext
TEMP1.val=N1.val*10  // Multiply N1.val by 10
TEMP2.val=TEMP1.val+N2.val
RESULT.val=TEMP2.val*N3.val

// Convert RESULT.val to a string with 'R ' prefix
covx RESULT.val,t0.txt,0,0
t0.txt="R "+t0.txt
