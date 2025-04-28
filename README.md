# EX-11-EMI-CALCULATOR

## AIM
To write a C program that converts a binary number to its decimal equivalent using a function without return type and without arguments.





## ALGORITHM
```
1.Start the program.
2.Declare a function binaryToDecimal() that:
Does not take any arguments.
Does not return any value (void).
Reads the binary number from the user.
Converts the binary number to its decimal equivalent using a loop.
3.Inside the function:
Initialize decimal = 0, base = 1, and remainder variables.
Extract each bit of the binary number (starting from the least significant bit) and compute its decimal equivalent.
Multiply the extracted bit by the appropriate power of 2 and add it to the decimal value.
4.Call the function from the main() function.
5.End the program.
```
## PROGRAM
```.py
#include <stdio.h>
#include <math.h>
void cal(){
    int num,val,sum=0,i=0,x;
    scanf("%d",&num);
    x=num;
    while(num!=0){
        val=num%10;
        if (val!=0){
            sum+=pow(2,i);
        }
        i++;
        num=num/10;
    }
    printf("%d in binary = %d in decimal",x,sum);
}
int main(){
    cal();
}
```


## OUTPUT

![image](https://github.com/user-attachments/assets/989ba644-73a7-40f2-bd91-59cae79432b8)




## RESULT
The program successfully converts a binary number to its decimal equivalent and prints the result.

 
 


# EX-12-FIBONACCI-SERIES
## AIM
The aim of this program is to print all the leap years from 1 to a given number N. Leap years are those years that meet the criteria of being divisible by 4 but not divisible by 100, unless they are also divisible by 400.


## ALGORITHM
```
1.Input: The program accepts an integer N, which is the upper limit up to which we need to find the leap years.
2.Check Leap Year: A year is a leap year if:
3.It is divisible by 4, and
It is not divisible by 100, unless it is also divisible by 400.
4.Iterate through years: Start from year 1 and iterate through each year up to N.
Print Leap Years: For each year, check if it's a leap year using the condition. If it is, print it.
Output: Display all leap years from 1 to N in a single line.
5.Steps:
Start.
Input N (the upper limit).
6.For each year from 1 to N:
7.Check if the year is a leap year.
If yes, print the year.
8.End.
```
## PROGRAM
```.py
#include <stdio.h>
int main(){
    int a,i;
    scanf("%d",&a);
    for (i=1;i<=a;i++){
        if (i%4==0){
            printf("%d ",i);
        }
    }
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/7a7629aa-51b2-403b-818a-9ce19bb4da91)







## RESULT
The leap years between 1 and 10 are 4 and 8 because:

4 is divisible by 4 and not by 100, so it's a leap year.

8 is divisible by 4 and not by 100, so it's a leap year.

Therefore, the program prints 4 8.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM

## OUTPUT









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM


## OUTPUT





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:

## Output:
 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



