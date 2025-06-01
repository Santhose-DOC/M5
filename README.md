# NAME : SANTHOSE AROCKIARAJ J
# REGISTER NO: 212224230248 
# EX-21-POINTERS
# AIM:
Write a C program to convert a 23.65 into 25 using pointer

## ALGORITHM:
1.	Declare a double variable to hold the floating-point number (23.65).
2.	Declare a pointer to double to point to the address of the variable.
3.	Use the pointer to modify the value to 25.0.
4.	Print the modified value.

## PROGRAM:
```
#include <stdio.h>
int main() {
    float num = 23.65;
    float *ptr = &num;
    printf("Original number: %.2f\n", *ptr);
    *ptr = 25.0;
    printf("Modified number: %.2f\n", *ptr);
    return 0;
}
```
## OUTPUT:
 	

![437943069-04494f21-459e-4559-889a-bd8cbe17b24d](https://github.com/user-attachments/assets/7cd1448d-14a1-44f6-aa9f-003dd2a0ecec)










## RESULT:
Thus the program to convert a 23.65 into 25 using pointer has been executed successfully.
 
 


# EX-22-FUNCTIONS AND STORAGE CLASS

## AIM:

Write a C program to calculate the Product of first 12 natural numbers using Recursion

## ALGORITHM:

1.	Define a recursive function calculateProduct that takes an integer parameter n.
2.	Return n multiplied by the result of the calculateProduct function called with n - 1.
3.	Declare an integer variable n and an unsigned long long variable product.
4.	Initialize n with the value 12 (for the first 12 natural numbers).
5.	Call the calculateProduct function with n and store the result in the product variable.
6.	Print the result, indicating it is the product of the first 12 natural numbers.

## PROGRAM:
```
#include <stdio.h>
unsigned long long product(int n) {
    if (n == 1) {
        return 1;
    } else {
        return n * product(n - 1);
    }
}
int main() {
    int n = 12;
    unsigned long long result;
    result = product(n);
    printf("Product of first 12 natural numbers is: %llu\n", result);
    return 0;
}
```

## OUTPUT:
![437943195-f9b6bfcc-6e11-4fdb-80de-5dbd210335f8](https://github.com/user-attachments/assets/4bb1ef19-73d5-48f7-9fca-eb5e0a4d01b6)
         		
## RESULT:

Thus the program has been executed successfully.
 
 


# EX-23-ARRAYS AND ITS OPERATIONS

## AIM:

Write C Program to find Sum of each row of a Matrix

## ALGORITHM:

1.	Declare and initialize the matrix with the desired values.
2.	Create a loop to iterate through each row of the matrix.
3.	Inside the loop, calculate the sum of the elements in each row.
4.	Print the sum for each row.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m,n,i,j;
    scanf("%d %d",&m,&n);
    int arr[m][n];
    for (i=0;i<m;i++){
        for (j=0;j<n;j++){
            scanf("%d",&arr[i][j]);
        }
    }
    printf("Sum of each row:\n");
    for (i=0;i<m;i++){
        int sum=0;
        for (j=0;j<n;j++){
            sum+=arr[i][j];
        }
        printf("Row %d sum = %d\n",i+1,sum);
    }
    return 0;
}
```


## OUTPUT

![image](https://github.com/user-attachments/assets/0f599e63-e3cc-45ee-a117-47d8199ae119)


 
 

 ## RESULT
 Thus the program has been executed successfully.


# EX-24-STRINGS

## AIM:

Write C program for the below pyramid string pattern. Enter a string: PROGRAM Enter number of rows: 5 P R O G R A M P R O G R A M P R O G R A M

## ALGORITHM:

1.	Input the number of rows for the pyramid (e.g., num_rows).
2.	Initialize variables:i for the row count (starting from 1),j for the character count (starting from 1)
3.	Start a loop for i from 1 to num_rows (for each row of the pyramid).
4.	Calculate the midpoint position as midpoint = (2 * num_rows - 1) / 2.
5.	End the program.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m,n,i,j;
    scanf("%d %d",&m,&n);
    int arr[m][n];
    for (i=0;i<m;i++){
        for (j=0;j<n;j++){
            scanf("%d",&arr[i][j]);
        }
    }
    printf("Sum of each row:\n");
    for (i=0;i<m;i++){
        int sum=0;
        for (j=0;j<n;j++){
            sum+=arr[i][j];
        }
        printf("Row %d sum = %d\n",i+1,sum);
    }
    return 0;
}
```
## OUTPUT

![437943310-33d53f4c-6251-4fbe-8091-08b4d3bacfbd](https://github.com/user-attachments/assets/f5c550d2-5769-4822-b205-db42c9956d6a)



## RESULT

Thus the C program to String process executed successfully
 

 
.



# EX -25 –DISPLAYING ARRAYS USING POINTERS
## AIM

Write a c program to read and display an array of any 6 integer elements using pointer

## ALGORITHM
Step 1: Start the program.
Step 2: Declare the following:
•	Integer variable i for iteration.
•	Integer variable n to store the number of elements.
•	Integer array arr[10] to hold up to 10 elements.
•	Integer pointer parr and initialize it to point to the array arr.
Step 3: Read the value of n (number of elements) from the user.
Step 4: Loop from i = 0 to i < n:
•	Read an integer value and store it in the address parr + i using pointer arithmetic.
Step 5: Loop from i = 0 to i < n:
•	Print the element at *(parr + i) using pointer dereferencing.
Step 6: End the program.

## PROGRAM
```
#include <stdio.h>
int main() {
	int arr[10];
	int *parr;
	int i, n;

	parr = arr;
	scanf("%d", &n);

	if (n > 10) {
		printf("Please enter up to 10 elements only.\n");
		return 1;
	}
	for(i = 0; i < n; i++) {
		scanf("%d", (parr + i));
	}
	printf("The array elements are:\n");
	for(i = 0; i < n; i++) {
		printf("%d ", *(parr + i));
	}
	printf("\n");
	return 0;
}
```
## OUTPUT

 ![437943367-796a948f-7831-4981-90bb-77a091fcbf80](https://github.com/user-attachments/assets/a1efe747-e7f7-454b-96b8-f398cff8e70f)


## RESULT

Thus the C program to read and display an array of any 6 integer elements using pointer has been executed


