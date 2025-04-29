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
void calculate_emi(float p, float r, int t) {
    float monthly_rate = r / 12 / 100;
    int months = t * 12;
    float emi = (p * monthly_rate * pow(1 + monthly_rate, months)) / (pow(1 + monthly_rate, months) - 1);
    printf("EMI: %.2f\n", emi);
}
int main() {
    float p, r;
    int t;
    printf("Enter loan amount: ");
    scanf("%f", &p);
    printf("Enter annual interest rate (in %): ");
    scanf("%f", &r);
    printf("Enter loan tenure (in years): ");
    scanf("%d", &t);
    calculate_emi(p, r, t);
    return 0;
}
```

## OUTPUT
![Screenshot 2025-04-29 184606](https://github.com/user-attachments/assets/3d35bb30-c88e-44eb-8cfd-202dd1051ce8)




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
#include <stdio.h>
int main() {
    int i, n, t1 = 0, t2 = 1, nextterm;
    scanf("%d", &n);
    printf("Fibonacci series : %d, %d", t1, t2);
    for (i = 3; i <= n; i++) {
        nextterm = t1 + t2;
        printf(", %d", nextterm);
        t1 = t2;
        t2 = nextterm;
    }
    return 0;
}
```
## OUTPUT
![Screenshot 2025-04-29 185338](https://github.com/user-attachments/assets/92a2c444-4dc8-4267-9269-a3705732043f)









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
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Last element: %d\n", arr[n - 1]);
    return 0;
}
```
## OUTPUT

![Screenshot 2025-04-29 185706](https://github.com/user-attachments/assets/3f0cd2bc-08e0-448c-ad41-673eb89c96a0)








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
```
#include <stdio.h>
int main() {
    int n, count = 0, x;
    printf("Enter n: ");
    scanf("%d", &n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &x);
        if (x % 2 == 0) count++;
    }
    printf("Even count: %d", count);
    return 0;
}
```

## OUTPUT

![Screenshot 2025-04-29 190408](https://github.com/user-attachments/assets/adb58721-9e19-42c5-b7e7-a2a2c9ec5f59)




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
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Original array: ");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    printf("Modified array: ");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }
    printf("\n");
    return 0;
}
```
## Output:
 
![Screenshot 2025-04-29 190843](https://github.com/user-attachments/assets/d2f8611a-0bed-4fea-ac75-5991aec6489c)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



