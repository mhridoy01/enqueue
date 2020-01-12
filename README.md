# enqueue


#include<stdio.h>
#define success_value 9999
#define null_value -9999
#define max_size 5

int q[max_size];
int front;
int rear;
int length;

void initialize()
{
    front=0;
    rear=0;
    length=0;
}
int enqueue(int item)
{
    if(front==max_size)return null_value;
    q[front]=item;
    front++;
    length++;
    return success_value;
}
void print()
{
    int i;
    for(i=0;i<front;i++)
    {
        printf("%d ",q[i]);
    }
    printf("\n");
}
int main()
{
    int temp;
    int input;
    scanf("%d",&input);
    temp= enqueue(input);
    scanf("%d",&input);
    temp= enqueue(input);
    scanf("%d",&input);
    temp= enqueue(input);
    scanf("%d",&input);
    temp= enqueue(input);
    scanf("%d",&input);
    temp= enqueue(input);

    print();
    return 0;
}
