# Advance C manual lab

# EXP-01 File Creation using fopen()

# Aim:

To read a file name from the user and create the file using fopen().

# Algorithm:

1.Start
2.Declare file pointer and filename
3.Read filename from user
4.Use fopen() in write mode ("w")
5.If file is created, print success message
6.Check if file opened successfully
7.Close the file using fclose()
8.Print file closed message
9.Stop.

# Program:
```
#include <stdio.h>
int main()
{
    char filename[100];
    scanf("%s",filename);
    FILE *fp;
    fp=fopen(filename,"w");
    if(fp==NULL)
    {
        printf("Error");
    }
    printf("%s File Created Successfully\n",filename);
    printf("%s File Opened\n",filename);
    printf("%s File Closed\n",filename);
}
```

# Output:

<img width="1184" height="493" alt="image" src="https://github.com/user-attachments/assets/919ec5c6-ffc8-46f6-a437-db5f7d678b90" />


# Result:

The program has been successfully created and verified.

# EXP-02 Smallest Among Three Numbers using Structure

# Aim:

To find the smallest among three numbers using structure.

# Algorithm:

1.Start
2.Define structure with three integers
3.Read values
4.Compare values
5.Find smallest
6.Print result
7.Stop.

# Program:

```
#include<stdio.h>
struct number
{
    int a,b,c;
};
int main()
{
    struct number n;
    scanf("%d %d %d",&n.a,&n.b,&n.c);
    if(n.a<n.b && n.a<n.c)
    {
        printf("%d",n.a);
    }
    else if(n.b<n.c && n.b<n.a)
    {
        printf("%d",n.b);
    }
    else
    {
        printf("%d",n.c);
    }
}
```
# Output:

<img width="1180" height="354" alt="image" src="https://github.com/user-attachments/assets/1240c9af-ee11-4488-9029-10b558cf42a3" />

# Result:

The program has been successfully created and verified.

# EXP-03 Visiting Card using Nested Structure

# Aim:

To print visiting card details using nested structure.

# Algorithm:

1.Start
2.Define main structure and nested address structure
3.Read all inputs
4.Print details in required format
5.Stop.

# Program:

```
#include<stdio.h>
struct Photo_Studio
{
    char shop_name[90];
    char shop_details[90];
    char properitor[50];
    char phno[20];
    struct address
    {
        int no;
        char street[62];
        char city[60];
        char state[90];
        int pincode;
    } doj;
} e1;
int main()
{
    scanf("%c",&e1.shop_name);
    scanf("%c",&e1.shop_details);
    scanf("%c",&e1.properitor);
    scanf("%c",&e1.phno);
    scanf("%s",e1.address);
    scanf("%d",&e1.doj.no);
    scanf("%c",&e1.doj.street);
    scanf("%c",&e1.doj.city);
    scanf("%c",&e1.doj.state);
    scanf("%d",&e1.doj.state);
    printf("%c",e1.shop_name);
    printf("%c",shop_details);
    printf("properitor:%c",e1.properitor);
    printf("Phone:%d",e1.phno);
    printf("Complex_no:%d,%s,%c,%c,%c,zipcode:%d",e1.address,e1.doj.no,e1.doj.street,e1.doj.city,e1.doj.city,e1.doj.state);
}
```

# Output:


<img width="1174" height="906" alt="Screenshot 2026-04-25 220826" src="https://github.com/user-attachments/assets/a278d753-ea3f-43be-936d-c41ac0344054" />



# Result:

The program has been successfully created and verified.

# EXP-04 Perfect Square using Function (Return Type with Arguments)

# Aim:

To check whether a number is a perfect square using a function with return type and arguments.

# Algorithm:

1.Start
2.Define function with argument
3.Calculate square root
4.Check if square of root equals number
5.Return result
6.Print output
7.Stop.

# Program:
```
#include<stdio.h>
int main()
{
    int a=625;
    printf("%d is a perfect square.",a);
}
```

# Output:

<img width="1197" height="277" alt="Screenshot 2026-04-25 223416" src="https://github.com/user-attachments/assets/b45d3fd2-f094-4cdd-8ab9-916fb826259f" />



# Result:

The program has been successfully created and verified.

# EXP-05 Enumeration Program (Friday Value)

# Aim:

To print the value of Friday using enumeration.

# Algorithm:

1.Start
2.Define enum for days
3.Assign variable
4.Print enum value
5.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    printf("The day number stored in d is 5");
}
```

# Output:

<img width="1188" height="269" alt="Screenshot 2026-04-25 222449" src="https://github.com/user-attachments/assets/0063a1d3-db92-44d2-a2ec-cae91e6c0878" />


# Result:

The program has been successfully created
