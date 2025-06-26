These are the code snippets from class

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
Printing String Literals and String Objects
```
String firstName = “Charles”;
String lastName = new String(“Babbage”);
String otherLiteral = “Charles”;
String otherObject= new String(“Babbage”);

System.out.println(firstName);
System.out.println(lastName);
```
print versus println
```
System.out.print(“a.Hello World”);
System.out.println(“b.Hello World”);
System.out.print(“c.Hello World”);
System.out.print(“d.Hello World”);
```
Escape sequences
```
System.out.print(“a.\”Hello World\” ”);
System.out.print(“b.\nHello World\n”);
System.out.print(“c.\\Hello World”);
```
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
## Arithmetic
```
System.out.println(5/0); //Arithmetic Exception
```
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

## Scanner
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
