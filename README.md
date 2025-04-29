# EX-11-EMI-CALCULATOR

## AIM
To write a C program that converts a binary number to its decimal equivalent using a function without return type and without arguments.





## ALGORITHM
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

6.For each year from 1 to N:7.Check if the year is a leap year.

If yes, print the year.

8.End.

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
 
 


# EX-13- To read the elements of the n x n matrix and print the diagonal elements of the matrix
## AIM :
To write a C program to read the elements of an n x n matrix and print its diagonal elements.
## ALGORITHM :
1.Start the program.

2.Declare the matrix and necessary variables (n, loop counters).

3.Read the value of n (size of the matrix).

4.Use nested loops to read n x n matrix elements from the user.

5.Use a loop to print the main diagonal elements where row index = column index (i == j).

6.End the program.
## PROGRAM :
```.py
#include <stdio.h>
int main(){
    int a,b,i,j,stor[100][100];
    scanf("%d",&a);
    for (i=0;i<a;i++){
        for (j=0;j<a;j++){
            scanf("%d",&b);
            stor[i][j]=b;
            if (i==j){
                printf("a[%d][%d] is %d\n",i,j,stor[i][j]);
            }
        }
    }
}
```

## OUTPUT :
![image](https://github.com/user-attachments/assets/ec3222e3-c452-471f-a11d-c7bec7928e3f)


## RESULT
The program successfully reads a square matrix of order n x n and prints the elements present on its main diagonal.
# EX-14-To Print the Number of  Odd Numbers in an Array
## AIM : 
To write a C program to read elements of an array and print all the odd numbers from it.

## ALGORITHM :
1.Start the program.

2.Declare an array and necessary variables (size, counters, etc.).

3.Read the number of elements in the array.

4.Use a loop to read the array elements from the user.

5.Traverse the array and check each element:

6.If the element is odd (element % 2 != 0), print it.

7.End the program.

## PROGRAM : 
```.py
#include <stdio.h>
int main(){
    int i,stor[100];
    printf("Odd numbers in the array are - ");
    for (i=0;i<7;i++){
        scanf("%d",&stor[i]);
    }
    for (i=0;i<7;i++){
        if (stor[i]%2!=0){
            printf("%d ",stor[i]);
        }
    }
}
```

## OUTPUT :
![image](https://github.com/user-attachments/assets/a4f071c0-355b-49fb-ae72-61c049769fcf)





## RESULT :


The program successfully reads the elements of an array and prints all the odd numbers.





 
 


# EX -15 - To read the elements of the n x n matrix and check whether the first element is divisible by 5

## Aim:
To write a C program to read the elements of an n x n matrix and check if the first element (a[0][0]) is divisible by 5.

## Algorithm:
1.Start the program.

2.Declare the matrix and necessary variables (n for the size of the matrix).

3.Read the size of the matrix (n x n).

4.Use nested loops to read the elements of the matrix from the user.

5.Check if the first element a[0][0] is divisible by 5.

6.Print the result based on the check.

7.End the program.
## Program:
```.py
#include <stdio.h>
int main(){
    int a,i,j,b,stor[50][50],v;
    scanf("%d",&a);
    for (i=0;i<=a;i++){
        for (j=0;j<=a;j++){
            scanf("%d",&b);
            stor[i][j]=b;
        }
    }
    v=stor[0][0];
    if (v%5==0){
        printf("a[0][0] =%d is divisible by 5",v);
    }
    else{
        printf("a[0][0] =%d is not divisible by 5",v);
    }
    
}
```

## Output:
![image](https://github.com/user-attachments/assets/e841c6f7-25e8-4f9b-9f9a-62d615b4b91c)

 


## Result:
The program successfully checks whether the first element of the matrix (a[0][0]) is divisible by 5 and prints the result accordingly.



