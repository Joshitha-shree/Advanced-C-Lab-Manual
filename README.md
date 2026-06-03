# Advance C Lab Manual

# EXP-01 Stack Display Using Array

# Aim:

To write a function to display elements of a stack implemented using an array.

# Algorithm
1.Start
2.Initialize top = -1
3.Check if top == -1
4.If true, print "Stack is empty"
5.Else, repeat from i = top to 0:
6.Print stack[i]
7.Stop.

# Program:

```
int top=-1;
float stack[100];
void display()
{
    if(top==-1)
    {
        printf("no elements");
        return;
    }
    for(int i=top;i>=0;i--)
    {
        printf("%.1f\n",stack[i]);
    }
}
```

# Output:

<img width="1182" height="640" alt="image" src="https://github.com/user-attachments/assets/d62feb06-c6ff-428f-97e4-ab2a9833857c" />

# Result:

The program has been successfully created and verified.

# EXP-02 Queue Insertion (Enqueue) Using Array

# Aim:

To write a function to insert elements into a queue using an array.

# Algorithm:

1.Start
2.Initialize front = -1, rear = -1
3.When inserting an element:
4.If rear == MAX-1, print "Queue Overflow"
Else:
If front == -1, set front = 0
Increment rear
7.Insert element at queue[rear]
8.Stop.

# Program:

```
int queue[50];
int top=-1,rear,front;
void enqueue(int data)
{
    if(front==-1)
    {
        front=0;
    }
    rear++;
    queue[rear]=data;
}
```

# Output:

<img width="1187" height="574" alt="image" src="https://github.com/user-attachments/assets/4309a1fc-c4b7-49af-b7a2-0cd3beaf0537" />

# Result:

The program has been successfully created and verified.

# EXP-03 Stack Push Operation Using Array

# Aim:

To write a function to push an element into a stack using an array.

# Algorithm:

1.Start
2.Initialize top = -1
3.When pushing an element:
4.If top == MAX-1, print "Stack Overflow"
Else:
Increment top
Assign stack[top] = element
5.Stop.

# Program:

```
int size=3,top=-1;
char stack[100];
void push (char data)
{
    if(top==size-1)
    {
        printf("stack is full\n");
        return;
    }
    stack[++top]=data;
}
```

# Output:

<img width="1189" height="665" alt="image" src="https://github.com/user-attachments/assets/2afaa10c-d15f-434b-94eb-54256e6ed345" />

# Result:

The program has been successfully created and verified.

# EXP-04 Addition Table Using For Loop

# Aim:

To write a C program to print the addition table of a given number using a for loop.

# Algorithm:

1.Start
2.Read the number n
3.Use a for loop from i = 1 to n:
4.Print n + i
5.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    int sum=0;
    for(int i=a;i<11;i++)
    {
        sum=sum+1;
        printf("%d ",sum);
    }
}
```

# Output:

<img width="1178" height="350" alt="image" src="https://github.com/user-attachments/assets/217596f5-aaf5-41c5-904f-2d4e99664244" />

# Result:

The program has been successfully created and verified.

# EXP-05 Queue Deletion (Dequeue) Using Array

# Aim:

To write a function to delete elements from a queue using an array.

# Algorithm:

1.Start
2.Check if front == -1 OR front > rear:
If true, print "Queue Underflow"
Else:
Remove element at queue[front]
3.Increment front
4.If front > rear:
Reset front = rear = -1
5.Stop.

# Program:

```
int queue[50];
int front, rear;
void dequeue()
{
    if(front==-1 && rear==-1)
    {
        printf("no elemets");
    }
    else if(front==rear)
    {
        front=-1;
        rear=-1;
    }
    else
    {
        ++front;
    }
}
```

# Output:

<img width="1190" height="765" alt="image" src="https://github.com/user-attachments/assets/89cde70a-8112-4aa3-9b08-a11c679b04d3" />

# Result:

The program has been successfully created and verified.
