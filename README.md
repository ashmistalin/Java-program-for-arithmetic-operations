# Java-program-for-arithmetic-operations

## AIM:
To write a java program to print all the basic arithmetic operations.

## PROCEDURE:






## PROGRAM:
```
import java.util.Scanner;
public class MathOperation{
    public static void main(String[] args){
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter the numbers:");
        int num1 =sc.nextInt();
        int num2= sc.nextInt();
        int sum=num1+num2;
        System.out.println("Sum of two numbers: "+sum);
        int sub=num1-num2;
        System.out.println("Subtraction of two numbers: "+sub);
        int mul=num1*num2;
        System.out.println("Product of two numbers: "+mul);
        float divi=num1/num2;
        System.out.println("Division of two numbers: "+divi);
        int rem=num1%num2;
        System.out.println("Remainder of two numbers: "+rem);
    }
}
```
## OUTPUT:
```
C:\Users\Dell\.jdks\openjdk-19.0.2\bin\java.exe "-javaagent:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\lib\idea_rt.jar=7777:C:\Program Files\JetBrains\IntelliJ IDEA Community Edition 2022.3.3\bin" -Dfile.encoding=UTF-8 -Dsun.stdout.encoding=UTF-8 -Dsun.stderr.encoding=UTF-8 -classpath "C:\Users\Dell\IdeaProjects\Java 1\out\production\Java 1" MathOperations
Enter the numbers:
10 15
Sum of two numbers: 25
Subtraction of two numbers: -5
Product of two numbers: 150
Division of two numbers: 0.0
Remainder of two numbers: 10

Process finished with exit code 0
```

## RESULT:
Thus the java program to print the basic arithmetic operations is executed and the output is verified.
