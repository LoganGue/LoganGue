#include <stdio.h>
#include <stdlib.h>

int main() {
    int c, n;

    printf("Four random numbers: \n");

    for (c = 1; c <= 4; c++) {
        n = rand() % 9 + 1;
        printf("%d\n", n);
    }

    return 0;
}
