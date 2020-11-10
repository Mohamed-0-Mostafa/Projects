# #include <stdio.h>
#include <stdlib.h>

int main()
{
    int num, sum=0, i;

    printf("Enter the number you want to check : \n");
    scanf("%d",&num);

    for(i=1 ; i<num; i++)
        {
            if (num % i == 0)
            {
                sum += i;
            }
        }

    if (sum == num)
    {
        printf("The number %d is perfect",num);
    }
    else
    {
        printf("The number %d is not perfect",num);
    }

    return 0;
}
