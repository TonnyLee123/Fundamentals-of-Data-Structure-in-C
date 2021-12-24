```c
void push(int);
void pop();
int Top();
void print();
#include <stdio.h>
int a[5];
int top = -1;
int main()
{
    push(2);
    print();
    push(4);
    print();
    push(6);
    print();
    pop();
    print();
    push(99);
    print();
    
    return 0;
}

void push(int x)
{   
    // 檢查stack是否已滿
    if(top == 5 - 1)
    {
        printf("Error: stack overflow\n");
        return; //return?
    }
    top = top + 1;
    a[top] = x;
}

void pop()
{   
    // 檢查是否為 empty stack
    if(top == -1){
        printf("Error: no element to pop\n");
        return; 
    }
    top = top - 1;
}

int Top()
{
    return a[top];
}
void print()
{   
    int i;
    for(i=0; i<=top; i++)
        printf("%d ", a[i]);
    printf("\n");
}
```
https://www.youtube.com/c/crashcourse/videos  
https://www.youtube.com/watch?v=HtSuA80QTyo  
https://www.youtube.com/watch?v=A3ZUpyrnCbM&list=PLBZBJbE_rGRV8D7XZ08LK6z-4zPoWzu5H&index=12
