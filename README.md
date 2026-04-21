# NUBER-PATTERN
To make a right angle  triangle, pyramid, inverted triangle
#include <stdio.h>

int main()
{
    int choice, n, i, j;

    printf("Number Pattern Generator\n");
    printf("1. Right Angle Triangle\n");
    printf("2. Number Pyramid\n");
    printf("3. Inverted Triangle\n");
    printf("4. Repeated Number Pattern\n");

    printf("Enter your choice: ");
    scanf("%d", &choice);

    printf("Enter number of rows: ");
    scanf("%d", &n);

    switch(choice)
    {
        case 1:
            for(i = 1; i <= n; i++)
            {
                for(j = 1; j <= i; j++)
                    printf("%d ", j);
                printf("\n");
            }
            break;

        case 2:
            for(i = 1; i <= n; i++)
            {
                for(j = 1; j <= i; j++)
                    printf("%d ", i);
                printf("\n");
            }
            break;

        case 3:
            for(i = n; i >= 1; i--)
            {
                for(j = 1; j <= i; j++)
                    printf("%d ", j);
                printf("\n");
            }
            break;

        case 4:
            for(i = 1; i <= n; i++)
            {
                for(j = 1; j <= i; j++)
                    printf("%d ", i);
                printf("\n");
            }
            break;

        default:
            printf("Invalid choice");
    }

    return 0;
}
