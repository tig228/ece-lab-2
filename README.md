TINUOLA GBADAMOSI                                                                              DATE:09/18/2024                       LAST UPDATED: SEPTEMBER 18, 2024.

**INTRODUCTION:** The purpose of the lab is to understand the basics of how microcontrollers interact with the world: Digital input and output. Through this lab we will learn how to code in C to execute the blinking of the LED on the T1 Launchpad.

**RED LED AND GREEN LED**
We defined some variables and we made use of the P4DIR, P4REN, P4OUT, P2DIR, P2REN, and P2OUT registers. We also assigned imputs and outputs pins. The input pinS are the 4.1 and 2.3 pins while the output pinS, red and green LEDs are the 1.0 and 6.6 pins. We assigned code to the two buttons that if one is pressed(S1) the red LED should turn on and if the second button is pressed(S2) the green light should turn on. Both the Red and Green LEDs are dependent on the <msp430.h> library. For someone who wants to integrate this code make sure that the pins are named correctly.

**GPIO_driver(2).c**
The source file defines all the functions so that the code can be neater and calling the function is more easier because you can input values without having to write code all over. The source code controlls the pin. It depends on the <msp430.h> library.  

**GPIO_driver(2).h**
The header file declares all the functions that have been defined in the source code for the GPIO_driver. The code shows that the GPIO_driver initializes both the input and output pins.

**GPIO_driver(2).main.c**
This actually calls the function and here you can input values that can be run. It also depends on the <msp430.h> library.
