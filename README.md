# Advance C Lab Manual

# EXP-01 Delete an Element in Doubly Linked List

# Aim:

To write a function to delete a node from a doubly linked list.

# Algorithm:

1.Start
2.Check if head == NULL
3.If true, print "UNDERFLOW"
Else:
Store head in a temporary pointer temp
Move head = head->next
4.If head != NULL, set head->prev = NULL
Free temp
Print "Node deleted"
5.Stop.

# Program:

```
struct Node
{
    struct Node *prev;
    struct Node *next;
    int data;
}*head;

void delete()
{
    struct Node *temp=head;
    if(head==NULL)
    {
        printf("UNDERFLOW");
        return;
    }
    temp=head;
    head=head->next;
    if(head!=NULL)
    {
        head->prev=NULL;
    }
    free(temp);
    printf("node deleted\n");
    
    
    
}
```

# Output:

<img width="1179" height="784" alt="image" src="https://github.com/user-attachments/assets/31642fdb-25e1-41cc-9c95-1f3b9a345943" />


# Result:

The program has been successfully created and verified.

# EXP-02 Traverse and Display Linked List

# Aim:

To write a function to traverse and display elements of a linked list.

# Algorithm:

1.Start
2.Check if head == NULL
3.If true, print "List is empty"
Else:
Set temp = head
While temp != NULL:
Print temp->data
Move temp = temp->next
4.Stop.

# Program:

```
struct Node{
    float data; 
    struct Node *next;
}*head;


void display()
{
    struct Node *temp=head;
    if(head==NULL)
    {
        return;
    }
    while(temp!=NULL)
    {
        printf("%.2f\n",temp->data);
        temp=temp->next;
    }
 
 
 
 }
```

# Output:

<img width="1186" height="642" alt="image" src="https://github.com/user-attachments/assets/e7befd7b-1840-48ed-8a9b-12e30a2fcf7d" />

# Result:

The program has been successfully created and verified.

# EXP-03 Print Numbers from M to N in Reverse Order

# Aim:

To write a C program to print numbers from M to N in reverse order.

# Algorithm:

1.Start
2.Read values M and N
3.Use a loop from i = N down to M:
Print i
4.Stop.
<img width="1181" height="316" alt="image" src="https://github.com/user-attachments/assets/cefb308f-8430-4e44-b279-ac55f574695e" />

# Program:

```
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    for(int i=b;i>=a;i--)
    {
        printf("%d ",i);
    }
}
```

# Output:

<img width="1181" height="316" alt="Screenshot 2026-04-26 213923" src="https://github.com/user-attachments/assets/f7174bf0-372e-4584-9bcd-856fbb115245" />

# Result:

The program has been succesfully created and verified.

# EXP-04 All Basic Operations in Doubly Linked List

# Aim:

To write functions to perform insertion, deletion, searching, and display in a doubly linked list.

# Algorithm:

# Insertion

1.Start
2.Create a new node
3.Assign data to the node
4.Set new->next = NULL
If head == NULL:
Set new->prev = NULL
Set head = new
Else:
Traverse to last node
Set last node’s next = new
Set new->prev = last node
5.Stop.

# Display:

1.Start
2.Set temp = head
While temp != NULL:
Print temp->data
Move temp = temp->next
3.Stop.

# Search:

1.Start
2.Set temp = head, pos = 1
While temp != NULL:
If temp->data == item:
Print position
3.Stop
Move temp = temp->next, increment pos
If not found, print "Item not found"
4.Stop.

# Deletion:

1.Start
2.If head == NULL:
Print "UNDERFLOW"
Else:
Delete first node (same as previous delete algorithm)
3.Stop.

# Program:

```
struct Node
{
    struct Node *prev;
    struct Node *next;
    float data;
}*head;

void display()
{
    
    
    
}

void insert(float data)
{
    
    
    
}

void search(float data)
{
    
    
    
}

void delete()
{
    
    
}
```

# Output:

<img width="1193" height="856" alt="image" src="https://github.com/user-attachments/assets/e39d8b57-8243-4b0b-8b65-8decff5e13a4" />

# Result:

The program has been successfully created and verified.

# EXP-05 Insert a Node in Linked List

# Aim:

To write a function to insert a node into a linked list.

# Algorithm:

1.Start
2.Create a new node
3.Assign data to the node
Set new->next = NULL
If head == NULL:
Set head = new
Else:
Traverse to last node
Set last node’s next = new
4.Stop.

# Program:

```
struct Node{
    int data; 
    struct Node *next;
}*head;


void insert(int data)
{
    struct Node *temp=head;
    struct Node *newnode=malloc(sizeof(struct Node));
    newnode->data=data;
    newnode->next=NULL;
    
    if(head==NULL)
    {
        head=newnode;
        return;
    }
    while(temp->next!=NULL)
    {
        temp=temp->next;
    }
    temp->next=newnode;
    
}
```

# Output:

<img width="1191" height="643" alt="image" src="https://github.com/user-attachments/assets/db5ced42-57e4-4e41-bb02-0cd7d3624f46" />

# Result:

The program has been sucessfully created and verified.
