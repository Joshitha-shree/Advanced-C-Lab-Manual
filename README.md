# Advance c Lab Manual

# EXP-01 Dynamic Array Sum

# Aim:

To create an array dynamically, read values, calculate sum, and free memory.

# Algorithm

1.Start
2.Read integer n (size of array)
3.Allocate memory using malloc()
4.Check if memory allocation is successful
5.Read n elements into array
6.Initialize sum = 0
7.Traverse array from 0 to n-1
8.Add each element to sum
9.Print the sum
10.Free the allocated memory using free()
11.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    int arr[100];
    int sum=0;
    for(int i=0;i<=n;i++)
    {
        scanf("%d",&arr[i]);
        sum=sum+arr[i];
    }
    printf("%d",sum);
}
```

# Output:


<img width="1185" height="355" alt="image" src="https://github.com/user-attachments/assets/fb8ecd57-3464-412b-9303-1069d69899f8" />

# Result:

The program has been successfully created and verified.

# EXP-02 Square of Number using Function

# Aim:

To find the square of a number using function with arguments and return type.

# Algorithm:

1.Start
2.Define function square(n)
3.Return n * n
4.In main(), read input number
5.Call function and store result
6.Print the result
7.Stop.

# Program:

```
#include <stdio.h>
int main()
{
    float a;
    scanf("%f",&a);
    float b;
    b=a*a;
    printf("The square of %.f is : %.2f",a,b);
}
```

# Output:

<img width="1187" height="359" alt="image" src="https://github.com/user-attachments/assets/db122905-8a98-4df7-a51e-ec032e69ef73" />

# Result:

The program has been successfully created and verified.

# EXP-03 String Permutations (Lexicographical Order)

# Aim:

To print all permutations of strings in lexicographical order.

# Algorithm:

1.Start
2.Read integer n
3.Read n strings into array
4.Sort the array in lexicographical order
5.Print the current arrangement
6.Repeat until no next permutation:
7.Find largest index i such that a[i] < a[i+1]
8.If no such index → stop
9.Find largest index j such that a[j] > a[i]
10.Swap a[i] and a[j]
11.Reverse elements from i+1 to end
12.Print each permutation
13.Stop.

# EXP-04 Series using Recursion (9th Term)

# Aim:

To find the 9th term of series using recursion.

# Algorithm:

1.Start
2.Read value n (term number)
3.Read first three terms a, b, c
4.Define recursive function series(n)
5.Base case:
If n==1 return a
If n==2 return b
If n==3 return c
6.Recursive case:
7.Return series(n-1) + series(n-2) + series(n-3)
8.Call function for n=9
9.Print result
10.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int a,b,c,t,n;
    scanf("%d %d %d %d",&n,&a,&b,&c);
    for(int i=4;i<=n;i++)
    {
        t=a+b+c;
        a=b;
        b=c;
        c=t;
    }
    printf("%d",t);
}
```

# Output:

<img width="1193" height="291" alt="image" src="https://github.com/user-attachments/assets/319cd853-5553-4b53-b4fa-fc92d47dca2a" />

# Result:

The program has been successfully created and verified.

# EXP-05 Maximum of Four Numbers

# Aim:

To find the maximum of four numbers using function.

# Algorithm:

1.Start
2.Define function max_of_four(a,b,c,d)
3.Assume max = a
4.Compare b with max, update if greater
5.Compare c with max, update if greater
6.Compare d with max, update if greater
7.Return max
8.In main(), read four numbers
9.Call function and print result
10.Stop.

# Program:

```
#include<stdio.h>
int maxi(int a,int b,int c,int d)
{
    int max=(a>b && a>c && a>d)?a:(b>c && b>d)?b:(c>d)?c:d;
    return max;
}
int main()
{
    int a,b,c,d;
    scanf("%d %d %d %d",&a,&b,&c,&d);
    int res=maxi(a,b,c,d);
    printf("%d",res);
}
```

# Output:

<img width="1193" height="458" alt="image" src="https://github.com/user-attachments/assets/64e393a9-1bd6-4acd-ae23-b3c6ff021e07" />

# Result:

The program has been successfully and created and verified.
