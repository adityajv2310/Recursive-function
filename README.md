# Recursive-function

## Aim: 
To write a C# program to reverse a number using recursive function.

## Algorithm:

## Program:
```C#
using System;

namespace Recursive_Function
{
    class Program
    {
        public static int m, reverse = 0;
        public static int Recur(int number)
        {
            
            if (number > 0)
            {
                Program.m = number % 10;
                Program.reverse = Program.reverse * 10 + m;
                number = number / 10;
                return Recur(number);
            }
            return Program.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(Recur(num));
        }
    }
}
```
## Output:
![Online C# Compiler - online editor - Google Chrome 28-05-2022 11_23_19 (2)](https://user-images.githubusercontent.com/75235386/170812278-df09b500-f38c-4ebc-ac06-cbae493c8897.png)

## Result:
Thus, a C# program to reverse a number using recursive function was executed successfully.
