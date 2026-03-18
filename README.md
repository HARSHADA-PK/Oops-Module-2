# Oops-Module-2
# Ex.No:2(A) CLASS AND OBJECT

## QUESTION:
Create a class Vehicle with attributes as number, type and owner.

## AIM:
To Create a class Vehicle with attributes as number, type and owner.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Import the package java.util.Scanner to read user input.
4.	Create a class Vehicle with data members: (number, type, owner).
5.	In the main() method, create a Scanner object.
6.	Create two objects of the Vehicle class.
7.	Read the details (number, type, owner) for both objects from user input.
8.	Display the details of both vehicles.

## PROGRAM:
```
/*
Program to implement a conditional statement using Java
Developed by: Harshada P K
RegisterNumber:  212224060097
*/
```

## SOURCE CODE:
```python
import java.util.Scanner;
class Vehicle
{
    String number;
    String type;
    String owner;
}
public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        Vehicle v1 = new Vehicle();
        v1.number = sc.next();
        v1.type = sc.next();
        v1.owner = sc.next();

        Vehicle v2 = new Vehicle();
        v2.number = sc.next();
        v2.type = sc.next();
        v2.owner = sc.next();

        System.out.println(v1.number + " | " + v1.type + " | " + v1.owner);
        System.out.println(v2.number + " | " + v2.type + " | " + v2.owner);
    }
}

```


## OUTPUT:
<img width="900" height="270" alt="image" src="https://github.com/user-attachments/assets/f8664cb3-2be8-4087-90ff-8070fabf217d" />


## RESULT:
Thus, a Java program to create a class Vehicle with attributes number, type, and owner was successfully implemented and executed.


# Ex.No:2(B) METHODS

## QUESTION:
Write a method int cube(int x) that calls a method int square(int x) internally to calculate the cube as x * square(x).

## AIM:
To write a Java program that defines a method cube(int x) which internally calls the method square(int x) to compute the cube of a number.

## ALGORITHM :
1. Define a class demo with two methods:

     square(int n) → returns n * n.
     cube(int n) → returns n * square(n) by calling the square() method internally.

2. In the main class, read an integer input from the user.

3. Create an object of the demo class.

4. Call the cube() method using the object and print the result.

5. End the program.





## PROGRAM:
```
/*
Program to implement a conditional statement using Java
Developed by: Harshada P K
RegisterNumber:  212224060097
*/
```

## SOURCE CODE:
```
import java.util.*;
public class main
{
    public static int square(int x)
    {
        return x*x;
    }
    public static int cube(int x)
    {
        return x*square(x);
    }
    public static void main(String[] args)
    {
        Scanner input=new Scanner(System.in);
        int x=input.nextInt();
        int res=cube(x);
        System.out.println(res);
    }
}
```


## OUTPUT:
<img width="392" height="243" alt="image" src="https://github.com/user-attachments/assets/aa929a40-c871-4a15-8d09-12604778a14b" />



## RESULT:
The program has been executed successfully and the desired output has been obtained.


# Ex.No:2(C) ACCESS SPECIFIERS

## QUESTION:
Write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## AIM:
To write a Java program to create a class called BankAccount with private instance variables accountNumber and balance. Provide public getter and setter methods to access and modify these variables.

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	Create the BankAccount class with private variables and public getter/setter methods.
4.	In main(), create a BankAccount object.
5.	Read the account number and balance from the user.
6.	Set these values using setter methods.
7.	Display the account details using the display() method.
8.	End the program.


## PROGRAM:
```
/*
Program to implement a conditional statement using Java
Developed by: Harshada P K
RegisterNumber:  212224060097
*/
```
## SOURCE CODE:
```
import java.util.*;
class BankAccount {
     private String accountNumber;
     private double balance;
     
     public String getAccountNumber() {
         return accountNumber;
     }
      public void setAccountNumber(String accountNumber) {
          this.accountNumber = accountNumber;
      }
       public double getBalance() {
           return balance;
          }
     public void setBalance(double balance) {
         this.balance = balance;
         }
    
}
public class main
{
    public static void main(String[] args)
    {
        Scanner input=new Scanner(System.in);
        BankAccount ob=new BankAccount();
        String num=input.nextLine();
        double bal=input.nextDouble();
        ob.setAccountNumber(num);
        ob.setBalance(bal);
        System.out.println("Account Number: "+ob.getAccountNumber());
        System.out.println("Balance: "+ob.getBalance());
    }
}

```


## OUTPUT:
<img width="822" height="373" alt="image" src="https://github.com/user-attachments/assets/53583a0e-fba0-4147-859c-0c12e07388b4" />


## RESULT:
Thus, the Java program demonstrating the use of access specifiers with private variables and public getter and setter methods was successfully executed.


# Ex.No:2(D) VARIABLE SCOPE AND CONSTRUCTOR

## QUESTION:
Write a class that uses a constructor to initialize variables and overrides toString() method.

## AIM:
To write a Java program that initializes object variables using a constructor and overrides the toString() method to display object details in a readable format.

## ALGORITHM :

1. Define a class Student with two instance variables:

     String name

     int age

2. Create a parameterized constructor to initialize these variables.

3. Override the toString() method to return the student details in a formatted string.

4. In the main() method:

    - Read the name and age from the user.

    - Create a Student object using the constructor.

5. Print the object, which automatically calls the overridden toString() method.

6. End the program.



## PROGRAM:
 ```
/*
Program to implement a conditional statement using Java
Developed by: Harshada P K
RegisterNumber:  212224060097
*/
```

## SOURCE CODE:

```
import java.util.*;
class student
{
    String name;
    int age;
    student(String name,int age)
    {
        this.name=name;
        this.age=age;
    }
    public String toString()
    {
        return "Student{name='"+name+"', age="+age+"}";
    }
}
public class main
{
    public static void main(String[] args)
    {
        Scanner input=new Scanner(System.in);
        String name=input.nextLine();
        int age=input.nextInt();
        student ob=new student(name,age);
        System.out.println(ob);
    }
}
```




## OUTPUT:
<img width="896" height="395" alt="image" src="https://github.com/user-attachments/assets/0b280b01-a09a-4749-b733-41411f01b00a" />




## RESULT:
The program has been executed successfully and the desired output has been obtained.


# Ex.No:2(E) ACCESS MODIFIERS

## QUESTION:
Define class Game with: Static variable maxScore = 500 Print max score via 3 different object references. Change via one object into 800, and print the output of previous maxScore and changed maxScore. 

## AIM:
To define class Game with: Static variable maxScore = 500 Print max score via 3 different object references. Change via one object into 800, and print the output of previous maxScore and changed maxScore. 

## ALGORITHM :
1.	Start the program.
2.	Import the necessary package 'java.util'
3.	In the main() method, create three objects of Game.
4.	Print maxScore using all three objects.
5.	Modify maxScore to 800 using one object.
6.	Print the updated value using all three objects.
7.	End the program.

## PROGRAM:
```
/*
Program to implement a conditional statement using Java
Developed by: Harshada P K
RegisterNumber:  212224060097
*/
```

## SOURCE CODE:
```
import java.util.*;
class game
{
    static int max=500;
}
public class main
{
    public static void main(String[] args)
    {
        game g1=new game();
        game g2=new game();
        game g3=new game();
        System.out.println(g1.max);
        System.out.println(g2.max);
        System.out.println(g3.max);
        
        g1.max=800;
        System.out.println(g1.max);
        System.out.println(g2.max);
        System.out.println(g3.max);
    }
}
```


## OUTPUT:
<img width="287" height="283" alt="image" src="https://github.com/user-attachments/assets/1c35e3a4-9e6b-4bdc-8371-bcb87e4f52ba" />


## RESULT:
Thus, the Java program demonstrating the use of the static access modifier with multiple object references was successfully executed.


