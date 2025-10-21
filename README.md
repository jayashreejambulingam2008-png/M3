# EX-11-EMI-CALCULATOR

## AIM
To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM
1. Start the program.
2. Read principal amount, rate of interest and months.
3. Pass these values as arguments to function.
4. Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5. Display the result.
6. Stop the program.


## PROGRAM
```

#include <stdio.h>
#include <math.h>
void EMI(float p,float r, float m){
    r=r/(100*12);
    float result=(float)p*r*pow(1+r,m)/(pow(1+r,m)-1);
    printf("EMI is equal to %.2f",result);
}
int main() {
    float prin,rateofint,month;
    
    printf("Enter Principle, Rate of interest And Time to calculate EMI:\n");
    scanf("%f %f %f",&prin,&rateofint,&month);
    EMI(prin,rateofint,month);
    return 0;
}
   
```
## OUTPUT
<img width="1631" height="581" alt="image" src="https://github.com/user-attachments/assets/ffdccb49-0ddb-4ac8-82cd-72ad272db557" />






## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.
## ALGORITHM
1. Start the program.
2. Read number of terms to display.
3. Add the previous two terms and store it in new term.
4. Assign 2nd term to 1st term and 3rd term to 2nd term.
5. Repeat steps 3 and 4 n number of times.
6. Display the result.
7. Stop the program.

## PROGRAM
```

#include <stdio.h>
#include <math.h>

void fibo(int n){
    int a=0,b=1,sum=0;
    for(int i=0;i<n;i++){
        printf("%d ",a);
        sum=a+b;
        a=b;
        b=sum;
    }
}
int main() {
    int n;
    printf("Enter the no. of terms to printed in Fibonacci Series: \n");
    scanf("%d",&n);
    fibo(n);
    
    
    return 0;
}
```
## OUTPUT
<img width="1591" height="429" alt="image" src="https://github.com/user-attachments/assets/ac682ec8-9437-461c-921f-5b5098a4c8b9" />








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.


 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1. Start the program.
2. Read a variable.
3. Read the array values n number of times.
4. Print the last element.
5. Stop the program.

## PROGRAM
```

#include <stdio.h>

int main() {
    int n;
    printf("Enter the no. of terms to be stored in the array: \n");
    scanf("%d",&n);
    int arr[n];
    printf("\nEnter the elements of the array now\n");
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    printf("\nLast Element of the Array: %d",arr[n-1]);
    
    return 0;
}
```
## OUTPUT
<img width="1506" height="548" alt="image" src="https://github.com/user-attachments/assets/192ab0b7-6019-441d-8f11-4122af5c93d4" />










## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1. Start the program.
2. Read a variable.
3. Read the array values n number of times.
4. If the array value can be divided by 2 then increment count by 1.
5. Display result.
6. Stop the program.
## PROGRAM
```

#include <stdio.h>

int main() {
    int n;
    printf("Enter the no. of terms to be stored in the array: \n");
    scanf("%d",&n);
    int arr[n],count=0;
    printf("\nEnter the elements of the array now\n");
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
        if(arr[i]%2==0){
            count++;
        }
    }
    printf("\nTotal number of even numbers in the array is: %d",count);
    return 0;
}
```

## OUTPUT

<img width="1547" height="614" alt="image" src="https://github.com/user-attachments/assets/5c18d332-1fef-4092-952b-5a68252f09ab" />





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1. Input the array: Read the size of the array. Input the elements of the array.
2. Iterate through the array: For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3. Replace even elements with 'E': If an element is even, replace that element with the character 'E'.
4. Output the updated array: Print the updated array after replacements.

## Program:
```

#include <stdio.h>

int main() {
    int n;
    printf("Enter the no. of terms to be stored in the array: \n");
    scanf("%d",&n);
    int arr[n],count=0;
    printf("\nEnter the elements of the array now\n");
    for(int i=0;i<n;i++){
        scanf("%d",&arr[i]);
    }
    for(int i=0;i<n;i++){
        if(arr[i]%2==0){
            arr[i]='E';
        }
    }
     printf("\nThe elements of the array after updation are\n");
    for(int i=0;i<n;i++){
        if(arr[i]=='E'){
            printf("\'E\' ");
        }else{
        printf("%d ",arr[i]);}
    }
    return 0;
}
```
## Output:
<img width="1605" height="581" alt="image" src="https://github.com/user-attachments/assets/ecf9cab7-2f28-42c6-80ec-3cd548d6d86d" />

 


## Result:
Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.




