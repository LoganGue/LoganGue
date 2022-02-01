#include <stdio.h>
#include <stdlib.h>

int main() {
    int c, n;

    printf("Four random numbers for 2 Factor Authentication: \n"); //printf is a function. This manages the complexity of information by giving a quick and easy explanation of the output

    for (c = 1; c <= 4; c++) {
        n = rand() % 9 + 1;
        printf("%d\n", n);
    }
    void main()
    {
        char customer_satisfaction[30], ans; // this is a pointer because the address of the variable is in another variable (whether the user says yes or no)
        float ans;

        printf("Thank you for verifying \n"); // the user will see this after receving their first initial code

        printf("Did you get your number? (Y/N)\n"); // this is a pointer because the address of the variable is in another variable (whether the user says yes or no)
        scanf("%c", ans); // scanf is a user defined function. The user decides if they got their code or not

        if (ans == 'Y') // if they did get their code they will get the following message
        {
            printf("Great, you may now close the browser \n"); // the user is good to go

        }
        if (ans == 'N') // if they did not get their code, they will get the following message
        {
            printf("Please request code again \n"); // their next step if they need a new code
        }
    }

    return 0; //end 
}
