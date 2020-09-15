# Tech-project
Tech Assignment #2

using System;

namespace Tech Project

{
    class Program
    {
        static void Main(string[] args)
        {
            
            Console.Write("Enter an Integer value between 1 and 25 to execute an iterative statement: ");
          
            try
            {
               
                string input = Console.ReadLine();
                
                int value_of_input = int.Parse(input);
                
                if ((value_of_input > 0) && (value_of_input <= 5))
                {
                    Console.WriteLine("Executing a For Loop!");
                    Console.WriteLine("The For Loop will iterate " + value_of_input.ToString() + " times.");
                   
                    for (int i = 0; i < value_of_input; i++)
                    {
                        Console.WriteLine("You have entered #. This is the current integer value in the loop: #: " + i.ToString());
                    }
                    Console.WriteLine("Press any key to exit the program ...");
                   
                    Console.ReadKey(true);
                }
              
                else if ((value_of_input > 5) && (value_of_input <= 10))
                {
                    Console.WriteLine("Executing a While Loop!");
                    Console.WriteLine("The While Loop will iterate " + value_of_input.ToString() + " times.");
                   
                    while (value_of_input > 0)
                    {
                        Console.WriteLine("You have entered #. This is the current integer value in the loop: # " + value_of_input.ToString());
                        value_of_input--;
                    }
                    Console.WriteLine("Press any key to exit the program ...");
                    Console.ReadKey(true);
                }
               
                else if ((value_of_input > 10) && (value_of_input <= 20))
                {
                    Console.WriteLine("Executing a Do While Loop!");
                    Console.WriteLine("The Do While Loop will iterate " + value_of_input.ToString() + " times.");
                  
                    do
                    {
                        Console.WriteLine("You have entered #. This is the current integer value in the loop: #" + value_of_input.ToString());
                        value_of_input--;
                    } while (value_of_input > 0);
                    Console.WriteLine("Press any key to exit the program ...");
                    Console.ReadKey(true);
                }
              
                else
                {
                    Console.WriteLine("Please enter an integer between 1 and 25 and try again ...");
                    Console.WriteLine("Press any key to exit the program and try again ...");
                    Console.ReadKey(true);
                }
            } 
            catch
            {
                Console.WriteLine("Please enter an integer value and try running the program again ...");
                Console.WriteLine("Press any key to exit the program ...");
                Console.ReadKey(true);
            } 
        } 
    } 
} 
