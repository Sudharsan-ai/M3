# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <math.h>
void EMI(float p,float r,float t);
int main(){
    float p,r,t;
    printf("Enter the principal amount : ");
    scanf("%f",&p);
    printf("\nEnter the rate of interest(Annual interest) : ");
    scanf("%f",&r);
    printf("\nEnter the loan tenure : ");
    scanf("%f",&t);
    r = r/(100*12);
    t = t*12;
    EMI(p,r,t);
}

void EMI(float p,float r,float t){
    float amt = (p * r * pow(1+r,t))/(pow(1+r,t)-1);
    printf("\n\nEMI = %.2f",amt);
    
}


```

## OUTPUT

![image](https://github.com/user-attachments/assets/19ca4373-7ac4-4e67-89cd-76e589e0a530)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```
//Name: Sudharsan S 
//Reg no: 212224040334
#include <stdio.h>
void fib();
int main(){
    fib();
}
void fib(){
    int n,a=0,b=1,i=0;
    printf("Enter the value of n : ");
    scanf("%d",&n);
    printf("\n");
    for(;i<n;i++){
        printf("%d ",a);
        int c = a+b;
        a = b;
        b = c;
    }
    printf("\n\n");
    fib();
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/d08d43ce-bbc0-4eba-a915-d8f23d7264d5)

## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


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
```
//Name: Sudharsan S 
//Reg no: 212224040334
#include <stdio.h>
int main(){
    int n,i;
    printf("Enter the array length : ");
    scanf("%d",&n);
    int arr[n];
    printf("Enter the array elements : ");
    for(i=0;i<n;i++) scanf("%d",&arr[i]);
    printf("The last element of the given array : %d",arr[n-1]);
}

```
## OUTPUT

![image](https://github.com/user-attachments/assets/49104f79-7cec-429f-bab1-8754ce87ea76)


## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be positive increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```
//Name: Sudharsan S 
//Reg no: 212224040334
#include <stdio.h>
int main(){
    int n, c =0;
    printf("Enter the array length : ");
    scanf("%d",&n);
    int arr[n];
    printf("Enter the array elements : ");
    for(int i=0;i<n;i++){
        scanf("%d ",&arr[i]);
        if(arr[i]>=0) c++;
    }
    printf("\n\n");
    printf("The number of positive elements in the given array is: %d\n",c);
}

```

## OUTPUT

![image](https://github.com/user-attachments/assets/ce4edb36-ac7f-431c-800d-adb10b5941d4)




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
```
//Name: Sudharsan S 
//Reg no: 212224040334
#include <stdio.h>
int main(){
    int n, c =0;
    printf("Enter the array length : ");
    scanf("%d",&n);
    int arr[n];
    printf("Enter the array elements : ");
    for(int i=0;i<n;i++){
        scanf("%d ",&arr[i]);
        }
        printf("\nThe updated array is : ");
    for(int i=0;i<n;i++){
        if(arr[i]%2==0) printf("E ");
        else printf("%d ",arr[i]);
       
    }
  
    
}

```
## Output:
 
![image](https://github.com/user-attachments/assets/b422114c-1e16-41ac-87d1-a1c1533212e9)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



