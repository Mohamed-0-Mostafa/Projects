#include <stdio.h>
#include <stdlib.h>

void main()
{
    double pounds;
    double dollars;
    printf("Enter the amount in dollars:\n");
    scanf("%lf",&dollars);
    pounds=dollars*15.7;
    printf("%.2f dollars = %.2f pounds",dollars,pounds);

}
