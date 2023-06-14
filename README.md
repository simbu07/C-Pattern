## Ex-3 Pattern
### Date: 4/4/2023
### Aim:
To write a C# program for a pascal's triangle.

### Equipment Required:
Microsoft Visual Studio 2022 (or Lower) or Any other C# compiler.

### Algorithm:
### Step 1:
Create a new Class named program.

### Step 2:
Declare two variables of int data type one to store the input from user for no.of rows snd another the value for printing.

### Step 3:
Get the number of rows from the user.

### Step 4:
Using for loop print the rows and columns and space.

### Step 5:
Check the first and last rows of the triange is 1 using if condition.

### Step 6:
Otherwise use else to print the inner value val = val * (i - j + 1) / j

### Step 7:
Print the program.

### Step 8:
End of the Program.

### Program:
```
Developed By: Silambarasan K
Reg No: 212221230101
```
```c#
using System;
namespace Pattern
{
    public class parogram
    {
        public static void Main(string[] args)
        {
            int row, c = 1;

            Console.Write("Enter number of rows: ");
            row = Convert.ToInt32(Console.ReadLine());

            for (int i = 0; i < row; i++)
            {
                for (int j = 1; j <= row - i; j++)
                    Console.Write(" ");
                for (int j = 0; j <= i; j++)
                {
                    if (j == 0 || i == 0)
                        c = 1;
                    else
                        c = c * (i - j + 1) / j;
                    Console.Write("{0} ", c);
                }
                Console.WriteLine();
            }
        }
    }
}
```
### Output:
![image](https://user-images.githubusercontent.com/93427246/227568743-34c1b25a-28e5-4130-8b58-b2a966e9a300.png)

### Result:
Hence, a C# program for a pascal's triangle is executed successfully.
