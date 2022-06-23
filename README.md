## EX NO:09
## DATE:1.6.22
# <p align="center">Interface

## Aim:
  To write a C# program using interface concept

## Algorithm:
## Step 1:
Create an interface.

## Step 2:
Create a child class.

## Step 3:
Declare 2 functions deposit() and withdrawal() as abstract methods in the interface.

## Step 4:
Create those 2 functions in the child class and perform respective operation.

## Step 5:
Use while loop and and switch case to Get the choice from the user whether to perform withdrawal or deposit operation.

## Step 6:
After performing the functions display the remaining balance of the user.

## Program:
```
using System;
public interface Bank
{
    void deposit();
    void withdrawal();
}

public class Example : Bank
{
    int amount, ch, balance = 5000;
    public Example()
    {
        Console.WriteLine("1.Deposit\n2.Withdrawal");
        ch = Convert.ToInt32(Console.ReadLine());
        if (ch == 1)
        {
            deposit();
        }
        else
        {
            withdrawal();
        }
    }
    public void withdrawal()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance -= amount;
        Console.WriteLine(balance);
    }

    public void deposit()
    {
        int amount = Convert.ToInt32(Console.ReadLine());
        balance += amount;
        Console.WriteLine(balance);
    }
}

public class Hello
{
    public static void Main()
    {
        Example c = new Example();
        c.deposit();
        c.withdrawal();
    }
}
```

## Output:
![image](https://user-images.githubusercontent.com/75235090/172861194-bdf9e371-63d7-4eb4-96a6-cfd1dea1d4c5.png)


## Result:
Thus the C# program using interface concept has been implemented successfully
