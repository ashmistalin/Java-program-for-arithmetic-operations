# Java-program-for-arithmetic-operations

## AIM:
To write a java program to print all the basic arithmetic operations.

## PROCEDURE:
1. Import the Scanner class from the java.util package to get user input from the console.
2. Declare a class named MathOperation, and declare the main method within the MathOperation class.
3. Create a Scanner object named 'sc' to get input from the user.
4. Use the nextInt() method of the Scanner class to read the integer entered by the user and store it in the variable 'num1' and 'num2'.
5. Calculate the sum, difference,product, division and remainder for the given input and print the output.
6. Close the Scanner object using the close() method.
7. End the main method, and then the math operatoion class.

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


# Implementation-of-SVM-For-Spam-Mail-Detection

## AIM:
To write a program to implement the SVM For Spam Mail Detection.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import the required library packages.
2. Import the dataset to operate on.
3. Split the dataset into required segments.
4. Predict the required output.
5. Run the programm. 

## Program:
```
/*
Program to implement the SVM For Spam Mail Detection..
Developed by: ASHMI.S
RegisterNumber:  212221040021
*/
import pandas as pd
data = pd.read_csv("/content/spam.csv",encoding = 'latin-1')
data.head()
data.info()
data.isnull().sum()
x = data["v1"].values
y = data["v2"].values
from sklearn.model_selection import train_test_split
x_train,x_test,y_train,y_test = train_test_split(x,y,test_size = 0.2,random_state = 0)
from sklearn.feature_extraction.text import CountVectorizer
cv = CountVectorizer()    
x_train = cv.fit_transform(x_train)
x_test = cv.transform(x_test)
from sklearn.svm import SVC
svc = SVC()
svc.fit(x_train,y_train)
y_pred = svc.predict(x_test)
y_pred
from sklearn import metrics
accuracy = metrics.accuracy_score(y_test,y_pred)
accuracy
```

## Output:
## HEAD:
![GITHUB LOGO](s1.png)
## INFO:
![GITHUB LOGO](s2.png)
## ISNULL:
![GITHUB LOGO](s3.png)
## SVC PREDICT:
![GITHUB LOGO](s4.png)
## ACCURACY:
![GITHUB LOGO](s5.png)

## Result:
Thus the program to implement the SVM For Spam Mail Detection is written and verified using python programming.

