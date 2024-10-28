Input:

using System;

class Program // Changed from "class void Main()" to "class Program"
{
    static void Main() // Changed to "static void Main()"
    {
        // Read the number of test cases
        int T = Convert.ToInt32(Console.ReadLine());
        
        for (int i = 0; i < T; i++)
        {
            // Read input values for X and Y
            string[] input = Console.ReadLine().Split();
            int X = Convert.ToInt32(input[0]);
            int Y = Convert.ToInt32(input[1]); // Fixed "Covert" to "Convert"
            
            // Compare X and Y and print the appropriate message
            if (X < Y)
                Console.WriteLine("FIRST");
            else if (X > Y)
                Console.WriteLine("SECOND"); // Fixed "Writeline" to "WriteLine"
            else 
                Console.WriteLine("ANY");
        }
    }
}

Output: 
3
500 700
FIRST
600 600
ANY
800 300 
SECOND
