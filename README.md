# Advance C Lab Manual

# EXP-01 Hello World Program

# Aim:

To write a program to print "Hello, World!".

# Algorithm:

1.Start
2.Use print statement to display "Hello, World!"
3.Stop.

# Program:

```
#include <stdio.h>
int main()
{
    printf("Hello, World!");
}
```

# Output:

<img width="1180" height="264" alt="image" src="https://github.com/user-attachments/assets/420f9c9f-194c-4b35-ac5f-d8f5cdf46118" />

# Result:

The program has been successfully created and verified.

# EXP-02 Sum of Digits of a Five-Digit Number

# Aim:

To write a program to find the sum of digits of a given five-digit integer.

# Algorithm:

1.Start
2.Read integer n
3.Initialize sum = 0
4.Repeat until n > 0:
5.Get last digit: digit = n % 10
6.Add to sum: sum = sum + digit
7.Remove last digit: n = n / 10
8.Print sum
9.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    int c=0,f;
    while(a!=0)
    {
        f=a%10;
        c=c+f;
        a=a/10;
    }
    printf("%d",c);
}
```

# Output:

<img width="1183" height="356" alt="image" src="https://github.com/user-attachments/assets/7bbab3a4-e54b-45ca-aa9d-6acf9da64c61" />

# Result:

The program has been successfully created and verified.

# EXP-03 Number Pattern (Example: Input = 4)

# Aim:

To print a square number pattern from n to 1 in a symmetric format.

# Algorithm:

1.Start
2.Read integer n
3.Set size = 2*n - 1
Loop i from 0 to size-1:
Loop j from 0 to size-1:

4.Find minimum distance:

value = n - min(min(i, j), min(size-1-i, size-1-j))
5.Print value
6.Move to next line after each row
7.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    int size=2*a-1;
    for(int i=0;i<size;i++)
    {
        for(int j=0;j<size;j++)
        {
            int min=i<j?i:j;
            min=min<size-i?min:size-i-1;
            min=min<size-j?min:size-j-1;
            printf("%d ",a-min);
        }
        printf("\n");
    }
}
```

# Output:

<img width="1186" height="788" alt="image" src="https://github.com/user-attachments/assets/472afc47-affc-4ede-a79d-e5afae44b27b" />

# Result:

The program has been successfully created and verified.

# EXP-04 Number Pattern (Example: Input = 5)

# Aim:

To print a symmetric number pattern from n to 1 and back to n.

# Algorithm:

1.Start
2.Read integer n
3.Calculate size = 2*n - 1
4.For each row i from 0 to size-1:
5.For each column j from 0 to size-1:

# Compute:

1.value = n - min(min(i, j), min(size-1-i, size-1-j))
2.Print value
3.Print newline after each row
4.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    int size=2*a-1;
    for(int i=0;i<size;i++)
    {
        for(int j=0;j<size;j++)
        {
            int min=i<j?i:j;
            min=min<size-i?min:size-i-1;
            min=min<size-j?min:size-j-1;
            printf("%d ",a-min);
        }
        printf("\n");
    }
}
```

# Output:

<img width="1180" height="683" alt="image" src="https://github.com/user-attachments/assets/d551ab7c-e073-48a7-af8a-0bd317ce9e64" />

# Result:

The program has been successfully created and verified.

# EXP-05 Frequency of Digits in a String

# Aim:

To find and print the frequency of digits (0–9) in a given string.

# Algorithm:

1.Start
2.Read input string s
3.Initialize an array freq[10] = {0}
4.For each character ch in string:
If ch is a digit (0–9):
Convert to integer: digit = ch - '0'
Increment freq[digit]
5.Print all elements of freq from index 0 to 9
6.Stop.

# Program:

# Output:

# Result:

The program has been successfully created and verif
