#include <stdio.h>
#include <stdlib.h>

int main() {
    int c, n;

    printf("Four random numbers for 2 Factor Authentication: \n"); // This is a union I built previously because it only stores on variable/ outcome at once (the 4 digit code)

    for (c = 1; c <= 4; c++) {
        n = rand() % 9 + 1;
        printf("%d\n", n);
    }
    void main()
    {
        char customer_satisfaction[30], ans; 
        float ans;

        printf("Thank you for verifying \n"); 

        printf("Did you get your number? (Y/N)\n"); // This is a union because even though their are two possible outputs (Y/N), there is only one variable given
        scanf("%c", ans); 

        if (ans == 'Y') 
        {
            printf("Great, you may now close the browser \n"); 

        }
        if (ans == 'N') // This is a structure because this line of code contains multiple variables. It will send a message, send a code, and print the code
        {
            printf("Requesting code again \n"); 
            for (c = 4; c <= 9; c++) {
                n = rand() % 7 + 1;
                printf("%d\n", n);
        }
    }

    return 0;  
}
