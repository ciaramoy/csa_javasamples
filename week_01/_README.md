These are the code snippets from class
## 1.2 Vars & DataTypes
Printing variables of different datatypes
```
int myInt = 30;
double myDouble = 2.5 ;
boolean myBoolean = true;

myDouble = 3.7;

System.out.println(“These are primitive types”);
System.out.println(myInt);
System.out.println(myDouble);
System.out.println(myBoolean);
```
Printing String Literals and String Objects: Reference types
```
String firstName = “Charles”;
String lastName = new String(“Babbage”);
String otherLiteral = “Charles”;
String otherObject= new String(“Babbage”);

System.out.println(firstName);
System.out.println(lastName);
```
## 1.3 Expressions and Output
Print vs. Println
```
System.out.print(“a.Hello World”);
System.out.println(“b.Hello World”);
System.out.print(“c.Hello World”);
System.out.print(“d.Hello World”);
```
### Escape sequences
```
System.out.print(“a.\”Hello World\” ”);
System.out.print(“b.\nHello World\n”);
System.out.print(“c.\\Hello World”);
```

### Arithmetic Expressions
Addition, Subtraction, Integer Division, Division, Modulus Division
```
System.out.println(5+5);
System.out.println(10-5);
System.out.println(5*5);

System.out.println(10/3);
System.out.println(10/3.0);
System.out.println(10.0/3);
System.out.println(10.0/3);

System.out.println(10%3);
System.out.println(10%4);
System.out.println(10%2);
System.out.println(10%7);
```
Arithmetic Exception
```
System.out.println(5/0); //Arithmetic Exception
```
### Compound Arithmetic Expressions
BODMAS PEMDAS GEMS. whatever you call it
```
double result = 10 - 3 * 3 / 2 + 6; 
System.out.println(result);
result = (10 - 3) * 3 / 2 + 6; 
System.out.println(result);
result = (10 - 3) * 3 / (2 + 6); 
System.out.println(result);
result = (10 - 3) * 3.0 / 2 + 6; 
System.out.println(result);
result = (10 - 3) * 3.0 / (2 + 6); 
System.out.println(result);
```
PEMDAS with Modulus division
```
double result = 10 - 3 * 3 % 2 + 6; 
System.out.println(result);
result = (10 - 3) * 3 % 2 + 6; 
System.out.println(result);
result = (10 - 3) * 3 % (2 + 6); 
System.out.println(result);
```
## 1.4 Assignment and Input
Empty Strings and Null
```
String string1 = "";
String string2 = new String("");
String string3 = new String();
String string4 = null;

System.out.println(string1);
System.out.println(string2);
System.out.println(string3);
System.out.println(string4);
```
Updating variables
```
double result = 10 - 3 * 3 % 2 + 6; 
System.out.println(result);
result = result + result;
System.out.println(result);
```

### Input with Scanner Class
```
import java.util.Scanner; // import the Scanner class 

class Main {
  public static void main(String[] args) {
    Scanner myObj = new Scanner(System.in);
    String userName;
    
    // Enter username and press Enter
    System.out.println("Enter username"); 
    userName = myObj.nextLine();   
       
    System.out.println("Username is: " + userName);        
  }
}
```
Scanning Integers
```
import java.util.Scanner; // import the Scanner class 

class MyProgram {
  public static void main(String[] args) {
    Scanner myObj = new Scanner(System.in);
    String userName;
    int myInt;
    
    System.out.println("Enter integer number");
    myInt = myObj.nextInt(); // DOES NOT CONSUME NEWLINE - \n
    //myObj.nextLine(); 
    System.out.println("Enter username"); 
    userName = myObj.nextLine();   
       
    System.out.println("Username is: " + userName);        
    System.out.println("Number is: " + myInt);        
  }
}
```
## 1.6 Compound Assignment Operators
Shortcuts
Adding
```
int num1= 10;
int num2= 10;

num1= num1 + 5;
num2+= 5;
System.out.println(num1);
System.out.println(num2);
```
Subtracting
```
int num1= 10;
int num2= 10;

num1= num1 - 2;
num2-= 2;
System.out.println(num1);
System.out.println(num2);
```
Modulus division
```
int num1= 10;
int num2= 10;

num1= num1 % 4;
num2%= 4;
System.out.println(num1);
System.out.println(num2);
```
Multiplication
```
int num1= 2;
int num2= 2;

num1= num1 * 4;
num2*= 4;
System.out.println(num1);
System.out.println(num2);
```
Division
```
int num1= 100;
int num2= 100;

num1= num1 / 2;
num2/= 2;
System.out.println(num1);
System.out.println(num2);
```
### Post increment and post decrement
```
int num1= 10;
int num2= 10;

num1++;
num2--;
System.out.println(num1);
System.out.println(num2);
```

## 1.5 Double vs Int
### Casting
__TRACE THROUGH THIS CODE ON PAPER__
Doing integer division with doubles
```
double num1 = 13.0;
double num2 = 2;
int num3 =  (int)num1/(int)num2;
System.out.println(num3);
```
Casting to integer after double division
```
double num1 = 13.0;
double num2 = 2;
int num3 =  (int) (num1/num2);
System.out.println(num3);
```
Truncating a double
```
double num1 = 13.9;
num1 = (int)num1;
System.out.println(num1);
```
Turning an integer into a double
```
System.out.println(13/5);
System.out.println((double)13/5);
```
Integer division
NOTE: order of operations
```
double num1 = 13.9;
num1 = (int)num1+11/2;
System.out.println(num1);
```
Regular division
NOTE: order of operations
```
double num1 = 13.9;
num1 = (int)num1+11.0/2.0;
System.out.println(num1);
```
Regular division and Truncation
NOTE: order of operations
```
double num1 = 13.9;
num1 = (int)num1+ (double)11/(double)2;
System.out.println(num1);
```
### Implicit Type Casting / Automatic Casting 
```
int num1 = 3;
double num2 = num1;
System.out.println(num2);
```
### Manual rounding
Rounding up towards positive infinity
```
double num = 3.5;
System.out.println((int) (num+0.5) );
```

Rounding down towards negative infinity
```
double num = -3.5;
System.out.println((int) (num-0.5));
```
### Range of Integers
```
System.out.println(Integer.MIN_VALUE);
System.out.println(Integer.MAX_VALUE);
System.out.println(Integer.MIN_VALUE - 1);
System.out.println(Integer.MAX_VALUE + 1);
```
### Floating Pt Error
eg1
```
double first = 0.1;
double second = 0.2;
double result = first + second;
System.out.println(result);
```
eg2
```
System.out.println(0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1+0.1);
System.out.println(0.3+0.3+0.3+0.1);
System.out.println(0.3+0.3+0.2+0.2);
System.out.println(0.2+0.2+0.2+0.2+0.2);
```