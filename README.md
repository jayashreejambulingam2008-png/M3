# EX-11-EMI-CALCULATOR

## AIM
Write a program to prepare EMI calculation for 2000000 ,8.24,6Years using function with return type without arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(p*r*pow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include<math.h>
float calculate_EMI(){
    float P=2000000,R=8.24,T=6,emi;
    R=R/(12*100);
    T=T*12;
    emi=(P*R*pow(1+R,T)) / (pow(1+R,T)-1);
    return emi;
}
int main(){
    float emi;
    emi=calculate_EMI();
    printf("Monthly EMI is= %.3f",emi);
    return 0;
}
```
## OUTPUT
<img width="982" height="208" alt="image" src="https://github.com/user-attachments/assets/4d5580d3-e800-41fe-9acf-da9484d602d6" />





## RESULT

Thus the program to prepare EMI calculation for 2000000 ,8.24,6Years using function with return type without arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 11.

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
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    int a=0,b=1,next;
    for(int i=1;i<=n;i++){
        printf("%d ",a);
        next=a+b;
        a=b;
        b=next;
        }return 0;
}
```
## OUTPUT
<img width="983" height="207" alt="image" src="https://github.com/user-attachments/assets/4f2c2af2-907c-4d91-86ef-87e63598e2bf" />








## RESULT
Thus the program to generate the Fibonacci series for the value 11 has been executed successfully.
 
 


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
#include <stdio.h>

int main()
{
    int n, i;
    scanf("%d",&n);
    int a[n];
    for(i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
}
    for(i=0;i<n;i++) {   
        printf("%d ",a[i]);
    }

    return 0;
}
```
## OUTPUT
<img width="977" height="470" alt="image" src="https://github.com/user-attachments/assets/0d00070c-a2d9-42ab-96c2-bd313d2c3cc3" />









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements and negative elements in an array.

## ALGORITHM
1. Start
2. Read the value of n (number of elements in the array).
3. Declare an array arr[n] and integer variables i, positive = 0, negative = 0.
4. Read n elements from the user and store them in the array arr.
5. Repeat for each element in the array (from i = 0 to n - 1):
If arr[i] > 0 then
→ Increment positive by 1.
Else 
→ Increment negative by 1.
6. Display the value of positive as the count of positive numbers.
7. Display the value of negative as the count of negative numbers.
8. Stop

## PROGRAM
```
#include<stdio.h>
int main(){
    int n,i,positive=0,negative=0;
    scanf("%d",&n);
    int arr[n];
    for(i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(i=0;i<n;i++){
        if(arr[i]>0)
        positive++;
        else
        negative++;
    }
    printf("count  of positive numbers  in array: %d\n",positive);
    printf("count  of negative numbers  in array: %d",negative);
    return 0;
}
```

## OUTPUT
<img width="973" height="240" alt="image" src="https://github.com/user-attachments/assets/a8d085fb-4c5b-436c-99f5-4299131b57cd" />





## RESULT
Thus the program to count total number of positive elements and negative elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Odd Elements With 'O' In One Dimensional Array

## Aim:
To write a C program to replace all odd elements with 'O' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is odd (i.e., if the element modulo 2 not equals 0).
3.	Replace even elements with 'O':
     If an element is odd, replace that element with the character 'O'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```
#include<stdio.h>
int main(){
    int n;
    scanf("%d",&n);
    int a[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&a[i]);
    }
    for(int i=0;i<n;i++){
        if(a[i]%2!=0){
            printf("O ");
        }else{
            printf("%d ",a[i]);
        }
    }return 0;
}
```
## Output:
<img width="976" height="232" alt="image" src="https://github.com/user-attachments/assets/53c9b28d-4d93-446d-bfd7-9bf88a8fa3c3" />
 


## Result:

Thus, the program to replace all odd elements with 'O' in one dimensional array was verified successfully.



