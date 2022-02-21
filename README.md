#include <stdio.h> // input/output layout
#include <stdlib.h> // standard library

void copy_files(FILE* in, FILE* out) // void means it does not return the value
{
    int c; //integer c

    //copy all characters in the file
    while ((c = getc(in)) != EOF)
        putc(c, out);

    int main(); { // return integers in the output // main function
    int c, n; // integers

    printf("Four random numbers for 2 Factor Authentication: \n"); // This is a union I built previously because it only stores one variable/ outcome at once (the 4 digit code)
    // printf is also a function, it manages the complexity of information by giving a quick and easy explanantion

    for (c = 1; c <= 4; c++) { // input that determines the output
        n = rand() % 9 + 1;
        printf("%d\n", n);
    }
    {
        char customer_satisfaction[30], ans; // declare character type variable as yes or no

        printf("Thank you for verifying \n"); // the user will see this after receving their first initial code

        printf("Did you get your number? (Y/N)\n"); // This is a union because even though there are two possible outputs (Y/N), there is only one variable given
        scanf_s("%c", ans); // scanf is a user defined function. the user decides if they got their code or not
        // added "_s" to "scanf" for security pruspoes, will run the same for the user

        if (ans == 'Y')
        {
            printf("Great, you may now close the browser \n"); // if they did get their code they will get the following message
        // the user is good to go
        }
        if (ans == 'N') // This is a structure because this line of code contains multiple variables. It will send a message, send a code, and print the code
        // If the choose "N" for no, they did not get their code and will receive the following message
        {
            printf("Requesting code again \n"); // their next step if they need a new code
            for (c = 4; c <= 16; c++) {
                n = rand() % 8 + 3;
                printf("%d\n", n);
            // the user gets a new code
        }
        // Copy all characters fro the input file to the output file
            copy_files(in, out)
                printf("File has been copied. \n");

         // clean up and close all the open files
            fclose(in);
            fclose(out);
        }

    return 0; // code complete, execute code
}
