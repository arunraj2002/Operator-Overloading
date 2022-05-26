# Operator-Overloading

## Aim:
 To write a C# program to find the volume of a box using operator overloading
 
## Algorithm:

 
 
## Program:
```c#
using System;
namespace ConsoleApp1
{
    class box
    {
        public int l, b, h,vol;
        public static box operator+(box b1,box b2)
        {
            box b3 = new box();
            b3.l = b1.l + b2.l;
            b3.b = b1.b + b2.b;
            b3.h = b1.h + b2.h;
            b1.vol = b1.l * b1.b * b1.h;
            b2.vol = b2.l * b2.b * b2.h;
            b3.vol = b3.l * b3.b * b3.h;
            return b3;
        }
        public static void Main()
        {
            box b1 = new box();
            Console.WriteLine("Enter the Length of Box1");
            b1.l = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the Breadth of Box1");
            b1.b = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the Height of Box1");
            b1.h = Convert.ToInt32(Console.ReadLine());
            box b2 = new box();
            Console.WriteLine("Enter the Length of Box2");
            b2.l = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the Breadth of Box2");
            b2.b = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Enter the Height of Box2");
            b2.h = Convert.ToInt32(Console.ReadLine());
            box b4 = new box();
            b4 = b1 + b2;
            Console.WriteLine("Volume of Box1");
            Console.WriteLine(b1.vol);
            Console.WriteLine("Volume of Box2");
            Console.WriteLine(b2.vol);
            Console.WriteLine("Volume of Box3");
            Console.WriteLine(b4.vol);

        }
    }
}
```
 
## Output:
![01](https://user-images.githubusercontent.com/75235747/170472618-37dedf7c-c13d-47ac-a10f-8b05337de812.PNG)

## Result:
