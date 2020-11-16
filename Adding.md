#include <stdio.h>
#include <stdlib.h>

int main()
{
    int sum=0;
    int numbers[2];

    FILE *fpointer;
    fpointer = fopen("text.txt", "a+");

    fscanf(fpointer, "%d", &numbers[0]);
    fscanf(fpointer, "%d", &numbers[1]);
    sum = numbers[0]+numbers[1];
    fprintf(fpointer, "\nThe sum = %d",sum);

    fclose(fpointer);
}
