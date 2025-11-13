# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:

#include <stdio.h>

int main() {
   char a,b,c;
   printf("enter charcater:");
   scanf("%c %c %c",&a,&b,&c);
   printf("%c\n%c\n%c\n",c,b,a);

    return 0;
}


## OUTPUT:
<img width="1742" height="661" alt="image" src="https://github.com/user-attachments/assets/866663f1-1fbb-4406-9114-f5a36fc15cd7" />


















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:

#include <stdio.h>

int main() {
    int a;
   scanf("%d",&a);
if(a>0)
{
    printf("A is positive");
}
else
{
    printf("A is negative");
}

    return 0;
}


# OUTPUT:
<img width="1656" height="880" alt="image" src="https://github.com/user-attachments/assets/03b51919-395c-47a9-b83a-f8ecd2e7dfa0" />












# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:

#include <stdio.h>

int main() {
       float num1,den1;
       scanf("%f %f",&num1,&den1);
       float dec1=num1/den1;
       
       float num2,den2;
       scanf("%f %f",&num2,&den2);
       float dec2=num2/den2;
       
       (dec1>dec2)?printf("second fraction is minimum"):printf("first fraction is minimum");

    return 0;
}


## OUTPUT:
<img width="1830" height="861" alt="image" src="https://github.com/user-attachments/assets/ef6519f5-ac5c-4ce4-a844-8b808ba3ea08" />










## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:

#include <stdio.h>

int main() {
      int a;
      scanf("%d",&a);
      if(a==1)
      {
          printf("The input value is equal to 1");
          
      }
      else
      {
          printf("The input value is not equal to 1");
      }
      

    return 0;
}


## OUTPUT:

<img width="1796" height="866" alt="image" src="https://github.com/user-attachments/assets/7e87ad29-1f6d-43f0-af10-a71096b6a589" />









	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:

#include <stdio.h>

int main() {
    int m1,m2,m3;
    float tot,per;
    printf("Enter marks for Three(3) subjects:\n");
    scanf("%d %d %d",&m1,&m2,&m3);
    tot=(float)m1+m2+m3;
    per=(float)tot/3;
    printf("The total marks is: %.2f, and the Percetnage is: %.2f\n",tot,per);
    if(m1>=40 && m2>=40 && m3>=40){
        if(per>=60){
            printf("Division = First");
        }
        else if(per>=48){
            printf("Division = Second");
        }
        else if(per>=36){
            printf("Division = Pass");
        }
        else{
            printf("Division = Fail");
        }
    }else{
        printf("Marks are not sufficient");
    }

    return 0;
}


## OUTPUT:
<img width="1146" height="435" alt="image" src="https://github.com/user-attachments/assets/3c9865b4-e0e5-4a8c-bf83-baf575cd148b" />


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.
