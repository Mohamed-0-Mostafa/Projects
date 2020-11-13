#include <stdio.h>
#include <stdlib.h>

void main()
{
    int check,sum=0,minus=0,n=0,i,j;
    int numbers [20];
    int d_numbers [n];

    printf("Enter 20 numbers : \n");
    for (i=0; i<20; i++){
            scanf("%d", &check);
            for (j=0; j<i; j++){
                if (check == numbers[j]){
                    n++;
                    d_numbers[n-1]= check;
                    minus += d_numbers[n-1];
                    break;
                }
            }
            numbers[i]= check;
            sum += numbers[i];
    }
    printf("The numbers you entered : \n");
    for (i=0; i<20; i++){
        printf("%d\  ", numbers[i]);
    }
    printf("\n");
    printf("The numbers you duplicated : \n");
    for (i=0; i<n; i++){
        printf("%d\  ", d_numbers[i]);
    }
    sum -= minus;
    printf("\nThe summation of unique numbers = : %d", sum);
}
