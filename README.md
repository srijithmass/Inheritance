# <p align="center">Inheritance</p>

## Aim:
To write a C# program to print some messages using hierarchical inheritance.

## Algorithm:
### Step 1: 
Create a base class.

### Step 2:
Create two child class.

### Step 3:
Create a constructor in the base class and print a message.

### Step 4: 
Inside the base class create a display function.

### Step 5:
Create constructor in child classes to print the message.

### Step 6: 
Inside the child classes override the display functions.

### Step 7:
In the Main function, create an object for each child classes.

## Program:
Developed By: **SRIJITH R**

Register No.: **212221240054**
```c#
using System;

namespace exp8
{
    public class tyre
    {
        public tyre() {
            Console.WriteLine("Tyre - Vehicle");
        }
        public virtual void display()
        {
            Console.Write("Tyre is attached to ");
        }
    }

    public class car : tyre
    {
        public car() {
            Console.WriteLine("Car Constructor");
        }
        public override void display()
        {
            base.display();
            Console.WriteLine("Car");
        }
    }

    public class scooter : tyre
    {
        public scooter() {
            Console.WriteLine("Scooter Constructor");
        }
        public override void display()
        {
            base.display();
            Console.WriteLine("Scooter");
        }
    }
    public class main
    {
        public static void Main(string[] args)
        {
            car newcar = new car();
            newcar.display();
            Console.WriteLine();
            scooter newscooter = new scooter();
            newscooter.display();
        }
    }
}
```
## Output:
![image](https://github.com/ShafeeqAhamedS/Inheritance/assets/93427237/e766011c-8f01-4b3c-a00b-61dbcece09d8)

## Result
Thus, C# program to print some messages using hierarchical inheritance is implemented successfully.
