https://www.youtube.com/watch?v=aCPkszeKRa4  

https://www.youtube.com/watch?v=5xUDoKkmuyw

# inked List implementation of stacks
```c
  +++ |+#include <stdlib.h>
/******************************************************************************

                            Online C Compiler.
                Code, Compile, Run and Debug C program online.
Write your code in this editor and press "Run" button to compile and execute it.

*******************************************************************************/

#include <stdio.h>
#include <stdlib.h>

void push(int);

struct node{
    int data;
    struct node* link;
}

struct node* top = NULL;

int main()
{
    
    push(5);
    return 0;
}

void push(int x)
{
    struct node* new = (struct node*)malloc(sizeof(struct node*));
    new -> data = x;
    new -> link = top;
    top = new;
    
}
```
