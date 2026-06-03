# Advance C Lab Manual

# EXP-01 Delete Element in Queue using Linked List (Dequeue)

# Aim:

To write a function to delete an element from a queue implemented using a linked list.

# Algorithm:

1.Start
2.Check if front == NULL
If true, print "Queue Underflow"
Else:
Store front in a temporary node temp
Move front = front->next
If front == NULL, set rear = NULL
Free temp
3.Stop.

# Program:

```
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void dequeue()
{
    if(front==NULL)
    {
        printf("Queue is Empty!!!\n");
        return;
    }
    front=front->next;
}
```

# Output:

<img width="1185" height="864" alt="image" src="https://github.com/user-attachments/assets/636d21a3-0cb2-429c-847f-f6923c26172a" />

# Result:

The program has been successfully created and verified.

# EXP-02 Insert Element in Queue using Linked List (Enqueue)

# Aim:

To write a function to insert elements into a queue using a linked list.

# Algorithm:

1.Start
2.Create a new node
3.Assign data to the node
Set new->next = NULL
If rear == NULL:
Set front = rear = new
Else:
Set rear->next = new
Move rear = new
4.Stop.

# Program:

```
struct Node
{
   int data;
   struct Node *next;
}*front=NULL,*rear=NULL;
void enqueue(int data)
{
    struct Node *newnode=malloc(sizeof(struct Node));
    newnode->data=data;
    newnode->next=NULL;
    if(front==NULL)
    {
        front=rear=newnode;
        return;
    }
    rear->next=newnode;
    rear=newnode;
}
```

# Output:

<img width="1182" height="640" alt="image" src="https://github.com/user-attachments/assets/b6490a0b-b7fb-4212-82c7-b3fda1b996bb" />

# Result:

The program has been successfully created and verified.

# EXP-03 Push Element in Stack using Linked List

# Aim:

To write a function to push an element into a stack using a linked list.

# Algorithm:

1.Start
2.Create a new node
3.Assign data to the node
Set new->next = head
Update head = new
4.Stop.

# Program:

```
struct Node   
{  
float data;  
struct Node *next;  
}*head;
void push(int data)  
{  
    struct Node *newnode=malloc(sizeof(struct Node));
    newnode->data=data;
    newnode->next=head;
    if(head==NULL)
    {
        head=newnode;
        return;
    }
    head=newnode;
}
```

# Output:

<img width="1185" height="678" alt="image" src="https://github.com/user-attachments/assets/75405d11-f338-430a-9f98-d6c8788e4dc3" />

# Result:

The program has been successfully created and verified.

# EXP-04 Addition of Two Numbers using Pointers

# Aim:

To write a C program to add two numbers using pointers.

# Algorithm:

1.Start
2.Declare two integers x and y
3.Declare pointers p and q
4.Assign addresses:
p = &x
q = &y
5.Read values of x and y
6.Calculate sum:
sum = *p + *q
7.Print sum
8.Stop.

# Program:

```
#include<stdio.h>
int main()
{
    int x,y,z;
    scanf("%d %d",&x,&y);
    z=x+y;
    printf("%d",z);
}
```

# Output:

<img width="1184" height="358" alt="image" src="https://github.com/user-attachments/assets/c7a53e7e-2b75-407a-99eb-52abdeb2cf71" />

# Result:

The program has been successfully created and verified.

# EXP-05 Pop Element from Stack using Linked List

# Aim:

To write a function to remove (pop) an element from a stack using a linked list.

# Algorithm:

1.Start
2.Check if head == NULL
If true, print "Stack Underflow"
Else:
Store head in temporary node temp
Move head = head->next
Free temp
3.Stop.

# Program:

```
struct Node   
{  
int data;  
struct Node *next;  
}*head;  
void pop()  
{ 
    if(head==NULL)
    {
        printf("stack is empty");
        return;
    }
    head=head->next;
}
```

# Output:

<img width="1188" height="411" alt="image" src="https://github.com/user-attachments/assets/2cd6c008-59b3-4008-b3b3-8d7467550b9a" />

# Result:

The program has been successfully created and verified
