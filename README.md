# Creating_Calculator_App_Using_CSharp
This is a simple Windows Forms calculator built in C# for basic arithmetic operations: addition, subtraction, multiplication, and division. It features a user-friendly GUI, error handling for division by zero, and reset functionality. Ideal for beginners learning event-driven programming and GUI development in C#.


Calculator Application in C#

This project is a simple Windows Forms Calculator application written in C#. The calculator performs basic arithmetic operations (addition, subtraction, multiplication, division) and supports input through a graphical user interface (GUI).
Features

    Basic arithmetic operations: +, -, *, /
    Input of numbers and decimal points
    Reset functionality
    Displays "DIV/Zero!" when attempting to divide by zero

Code Explanation

    Form Setup:
        The application extends the Form class and initializes the components in the constructor Form1().
        The Form1_Load method is empty but can be used to handle events when the form is loaded.

    Variables:
        input: Captures the current user input as a string.
        operand1 and operand2: Store the two numbers involved in the calculation.
        operation: Holds the selected arithmetic operator (+, -, *, /).
        result: Stores the result of the calculation.

    Number Button Clicks:
        Each button appends its corresponding number to the input string.
        Updates the textBox1 to display the current input.

    Operator Button Clicks:
        Buttons like eleven_Click (division), twelve_Click (multiplication), thirteen_Click (subtraction), and fourteen_Click (addition) store the current input into operand1, set the operation, and clear the input for the second number.

    Reset and Decimal Point:
        fifteen_Click: Resets all variables and clears the textBox1.
        sixteen_Click: Adds a decimal point to the input string.

    Equals Button:
        button17_Click: Executes the calculation when the equals button is clicked.
        Converts operand1 and operand2 to double using TryParse.
        Performs the operation based on the operation variable:
            Addition (+)
            Subtraction (-)
            Multiplication (*)
            Division (/) with zero-checking to prevent division by zero.
        Displays the result in textBox1 or "DIV/Zero!" for invalid division.

    Error Handling:
        Prevents crashes by handling division by zero.
        Properly resets variables for subsequent calculations.

Example Usage

    Run the application.
    Click numeric buttons to input numbers.
    Use operator buttons (+, -, *, /) to specify the operation.
    Click the equals button (=) to display the result.
    Use the clear button (C) to reset the calculator.
