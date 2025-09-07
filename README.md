## Hi this is a c# based calculator

using System; // Import the System namespace for console input/output and basic functions

class Program
{
    static void Main()
    {
        // Ask the user for the first number
        Console.Write("Number 1: ");
        double a = Convert.ToDouble(Console.ReadLine()); // Read input from console and convert it to a double

        // Ask the user for the second number
        Console.Write("Number 2: ");
        double b = Convert.ToDouble(Console.ReadLine()); // Convert the input to a double

        // Ask the user for an operation (+, -, *, /)
        Console.Write("Operation (+ - * /): ");
        string op = Console.ReadLine(); // Read the operation as a string

        double res = 0; // Variable to store the result

        // Check which operation the user entered and calculate the result
        if (op == "+") 
            res = a + b; // Addition
        else if (op == "-") 
            res = a - b; // Subtraction
        else if (op == "*") 
            res = a * b; // Multiplication
        else if (op == "/") 
            res = a / b; // Division
        else 
            Console.WriteLine("Invalid operation"); // Handle invalid operation input

        // Print the result to the console
        Console.WriteLine("Result: " + res);
    }
}
