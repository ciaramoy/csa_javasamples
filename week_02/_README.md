These are the code snippets from class
# 1.9
## void methods
```
class MyProgram {
  public static void main(String[] args) {
      add(10,2);
      subtract(10,2);
  }
  public static void add(int a, int b){
      int result = a + b;
      String statement = "The sum of " + a + " and " + b + ": " + result;
      System.out.println(statement);
  }
  public static void subtract(int a, int b){
      int result = a - b;
      String statement = "The difference of " + a + " and " + b + ": " + result;
      System.out.println(statement);
  }
}
```
## method with return values
```
class MyProgram {
  public static void main(String[] args) {
      int num1= 10;
      int num2= 2;
      
      int sum;
      int difference;
      
      sum = add(num1,num2);
      difference= subtract(num1,num2);
      
      System.out.println(sum);
      System.out.println(difference);
  }
  
  public static int add(int a, int b){
      int result = a + b;
      return result;
  }
  public static int subtract(int a, int b){
      int result = a - b;
      return result;
  }
}
```
## return types and parameters
```
class MyProgram {
  public static void main(String[] args) {
      
      String word= getSecret();
      System.out.println(word);
      
      double result = quadrupleIt(10);
      System.out.println(result);
      
      boolean answer= isLarger(3,4);
      System.out.println(answer);
      
  }
  public static String getSecret(){
      String secretMessage= "not so secret";
      return secretMessage;
  }
  
  public static double quadrupleIt(double num){
      num *= 4;
      return num;
  }
  
  public static boolean isLarger(int num1, int num2){
      if (num1>num2){
          return true;
      }
      return false;
  }
}
```