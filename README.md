# 8051-Calculator
This project aims to implement a basic calculator using a microcontroller, a keypad for input, and an LCD display for output. The calculator allows users to perform simple arithmetic operations such as addition, subtraction, multiplication, and division.

1. The code defines some constants using the EQU directive to assign specific port addresses to variables representing various components like the keypad, LCD bus, RS pin, EN pin, etc.

2. The program starts at the label "AGAIN" and enters an infinite loop.

3. Inside the loop, it calls the READ_KEY subroutine to read a key from the keypad.

4. It then initializes the LCD display by calling the LCD_INIT subroutine.

5. The program checks if the key pressed is 'C' (clear) and clears the display if true.

6. If the key is not 'C', it proceeds to perform the calculator operations.

7. It reads the first operand and stores it in memory.

8. It reads the operator (+, -, *, /) and stores it in memory.

9. It reads the second operand and stores it in memory.

10. It waits for the assignment operator (=) and prints it on the LCD display.

11. Depending on the operator, it performs addition (SUM), subtraction (SUB), multiplication (PRODUCT), or division (DIVISION) using separate subroutines.

12. The subroutines manipulate the operands and display the result on the LCD display.

13. The program includes additional subroutines for error handling, converting numbers to BCD (Binary Coded Decimal), clearing the display, and reading keys from the keypad.

14. It also includes subroutines for initializing the LCD display and sending commands or data to the LCD.

15. The program ends at the label "END."

Overall, this code represents a basic calculator program that takes input from a keypad, performs arithmetic operations on the operands, and displays the result on an LCD display.
The hardware components used in the project include a microcontroller, a keypad, and an LCD display. The microcontroller acts as the central processing unit and controls the overall operation of the calculator. The keypad provides input for numbers and operators, allowing users to enter the desired calculations. The LCD display is used to show the operands, operators, and the result of the calculations.

The software program, written in assembly language, runs on the microcontroller. It utilizes the input from the keypad to read the user's input, perform the necessary calculations, and display the results on the LCD display.

The program starts by initializing the necessary components and entering a loop to continuously read input from the keypad and update the display. The user can input numbers, operators, and the assignment operator (=) to perform calculations. The program handles various scenarios, such as clearing the display, validating the input, and performing the appropriate arithmetic operation based on the operator selected.

The calculator program supports basic error handling and provides feedback to the user in case of invalid input or mathematical errors. For example, if the user attempts to divide by zero, an error message is displayed on the LCD.

The LCD display is used to show the operands, operators, and the result of the calculations in a user-friendly format. The program converts the numerical values to the Binary Coded Decimal (BCD) format for proper display on the LCD.

Overall, this project demonstrates the implementation of a simple calculator using a microcontroller, keypad, and LCD display. It showcases the capabilities of the microcontroller to handle user input, perform calculations, and provide output on an external display.
