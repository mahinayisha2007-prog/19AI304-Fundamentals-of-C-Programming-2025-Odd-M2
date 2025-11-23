# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
## 3. Implementation of programs using conditional statements.
## 4. Implementation of programs using various control statements.
# Ex.No:6
  Build a C program to input a student’s marks in three subjects (Math, Science, and English). Calculate the average marks and determine the grade using nested if-else statements with safe floating-point comparisons based on the following grading criteria:
    
  A: 90 and above
  
  B: 75 to 89.99
  
  C: 50 to 74.99
  
  F: below 50
  
  The program should display the average marks up to two decimal places and the corresponding grade. 
  
# Date : 18-11-25
# Aim:
 To build a C program that receives inputs for a student’s marks in three subjects, calculates the average, and determines the grade using nested if-else statements with safe floating-point comparisons.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare float variables math, science, english to store marks of each subject.
### Step 4: 
  Declare a float variable average to store the average marks.
### Step 5: 
  Prompt the user to enter marks for Math, Science, and English.
### Step 6: 
  Read the input marks.
### Step 7: 
  Calculate the average marks using the formula:
   
  average=(math + science + english​)/3.0f
### Step 8: 
  Check if average is greater than or equal to 90.0f

  If yes, print Grade A.

  Else, proceed to Step 9.  
### Step 9:
  Check if average is greater than or equal to 75.0f

  If yes, print Grade B.

  Else, proceed to Step 10.
### Step 10:
  Check if average is greater than or equal to 50.0f

  If yes, print Grade C.

  Else, print Grade F.
### Step 11:
  Stop
# Program:
```
#include <stdio.h>

int main() {
float math, science, english, average;

printf("Enter Math marks: ");
scanf("%f", &math);

printf("Enter Science marks: ");
scanf("%f", &science);

printf("Enter English marks: ");
scanf("%f", &english);

average = (math + science + english) / 3.0f;

printf("Average Marks: %.2f\n", average);

if (average >= 90.0f) {
    printf("Grade: A\n");
} else {
    if (average >= 75.0f) {
        printf("Grade: B\n");
    } else {
        if (average >= 50.0f) {
            printf("Grade: C\n");
        } else {
            printf("Grade: F\n");
        }
    }
}

return 0;
}
```
# Output:

<img width="372" height="193" alt="517411484-6898c451-bbf1-4d37-8114-9787df8ac42f" src="https://github.com/user-attachments/assets/01344e36-f19d-4f59-a006-e0c96456defb" />
<img width="384" height="149" alt="517411861-d51f3f4a-77ed-4baf-b240-d7671f7d9abf" src="https://github.com/user-attachments/assets/1ddaf8fa-4960-4deb-b10b-a10c2f7dea28" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:7
  Develop a C program to display the multiplication table of a given number (15) up to 10.
# Date : 18-11-25
# Aim:
 To develop a C program that prints the multiplication table of the number 15 up to 10 using a for loop.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare an integer variable number and initialize it with 15.
### Step 4: 
  Declare another integer variable i to use as a loop counter.
### Step 5: 
  Use a for loop to iterate from i = 1 to i = 10.
  
  In each iteration:
  
  a. Multiply number by i.
  
  b. Print the result in the format: number x i = result.
### Step 6: 
  Stop

# Program:
```
#include <stdio.h>

int main() {
int num = 15;

for (int i = 1; i <= 10; i++) {
    printf("%d x %d = %d\n", num, i, num * i);
}

return 0;
}
```

# Output:

<img width="377" height="348" alt="517416804-74713f8d-6773-4384-af2c-afa7fc28fcb3" src="https://github.com/user-attachments/assets/dc8945ca-9ff8-4f9c-babd-f6606cd7af68" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:8
  Develop a C program to check whether a given number is prime or not.
# Date : 18-11-25
# Aim:
 To develop a C program that determines whether an input number is a prime number using a while loop.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare integer variables:
  
  n to store the number entered by the user.
  
  i to use as a counter (initialize to 2).
  
  f as a flag to indicate whether the number is divisible (initialize to 0).
### Step 4: 
  Read the value of n from the user.
### Step 5: 
  Use a while loop to iterate while i <= n-1:
  
  Check if n % i == 0:

  If yes, set f = 1 (number is not prime) and break the loop.
  
  Increment i by 1.
### Step 6: 
  After the loop:
  
  If f == 0, print that the number is prime.
  
  Else, print that the number is not prime.
### Step 7:   
  Stop
# Program:
```
#include <stdio.h>

int main() {
int n, i, flag = 0;

printf("Enter a number: ");
scanf("%d", &n);

if (n <= 1) {
    printf("Not a prime number");
    return 0;
}

for (i = 2; i <= n/2; i++) {
    if (n % i == 0) {
        flag = 1;
        break;
    }
}

if (flag == 0)
    printf("Prime number");
else
    printf("Not a prime number");

return 0;
}
```

# Output:
<img width="494" height="118" alt="517420262-eb06a83c-afe1-44ae-82cd-f424e9c90644" src="https://github.com/user-attachments/assets/8778e8f7-ea26-41bc-943b-c329b7365dc8" />
<img width="287" height="58" alt="517420519-eabb44cb-bd6a-4180-a632-ace0ace04363" src="https://github.com/user-attachments/assets/14aae996-0e32-48c1-bc64-184c15bb65cd" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:9
  Generate the C code to display the pattern below.  
 ``` 
 12345  
 2   4  
 3   3  
 4   2  
 54321
 ```
# Date : 
# Aim:
 To build a C program that prints the required numeric pattern for a given value of n using nested loops.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare variables i, j, n, and k.
### Step 4: 
  Read the value of n from the user.
### Step 5: 
  Set i = 1.
### Step 6:  
  Repeat the following steps until i > n:
  
  Step 6.1: For j from i to n, print j if i == 1 or j == i, otherwise print a space.
  
  Step 6.2: Set k = j - 2.
  
  Step 6.3: For j from 1 to i - 1, print k if i == n or j == i - 1, otherwise print a space.
  
  Step 6.4: Decrease k after each print.
  
  Step 6.5: Move to the next line.
  
### Step 7: 
  Increase i and repeat Step 6.
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>

int main() {
int i, j;

for(i = 1; i <= 5; i++) {
    for(j = 1; j <= 5; j++) {
        if(i == 1)
            printf("%d", j);
        else if(i == 5)
            printf("%d", 6 - j);
        else {
            if(j == 1)
                printf("%d", i);
            else if(j == 5)
                printf("%d", 6 - i);
            else
                printf(" ");
        }
    }
    printf("\n");
}

return 0;
```

# Output:

<img width="142" height="158" alt="517421762-81e2bd12-9420-4139-846d-4cf1af8f038d" src="https://github.com/user-attachments/assets/af9664f0-8d03-4a6e-9a11-a0b42f9e28c2" />

# Result: 
  Thus, the program was implemented and executed successfully, and the required output was obtained.

  
# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M2
# IAPR-2- Module 2 - FoC
# Ex.No:10
  Generate the C code to display the pattern below.  
  
 0
 
 7  0  7
 
 6  7  0  7  6
 
 5  6  7  0  7  6  5
 
 4  5  6  7  0  7  6  5  4
 
 3  4  5  6  7  0  7  6  5  4  3
 
 2  3  4  5  6  7  0  7  6  5  4  3  2
 
 1  2  3  4  5  6  7  0  7  6  5  4  3  2  1

# Aim: 
  To formulate a C program to print a symmetric numeric pattern in which each row contains an increasing sequence of numbers from the row value up to 7, followed by 0 in the center, and then a decreasing sequence of numbers back to the row value.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare integer variables i and j.
### Step 4: 
  Print 0 on the first line.
### Step 5:
  Set i = 7.
### Step 6:
   Repeat Steps 6.1 to 6.4 while `i >= 1`:

   Step 6.1: For `j = i` to `7`, print `j`.

   Step 6.2: Print `0` in the center.

   Step 6.3: For `j = 7` down to `i`, print `j`.

   Step 6.4: Move to the next line.
### Step 7:
  Decrease i by 1 and go back to Step 6.
### Step 8:
  Stop
PROGRAM:
```
#include <stdio.h>

int main() {
int i, j;

for(i = 0; i <= 7; i++) {
    for(j = i; j >= 1; j--)
        printf("%d ", j);

    printf("%d ", 0);

    for(j = 1; j <= i; j++)
        printf("%d ", j);

    printf("\n");
}

return 0;
}
```
OUTPUT:

<img width="684" height="365" alt="517422931-278d999a-60e6-4757-bfee-5bdf1bb4090f" src="https://github.com/user-attachments/assets/bc04525d-081b-4c5f-aa82-b428dfdc8119" />

# Result:
  Thus, the program was implemented and executed successfully, and the required output was obtained.

