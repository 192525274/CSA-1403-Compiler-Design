## PROGRAM
``` C PROGRAM
#include <stdio.h>

int main() {
    char op;

    printf("Enter an operator: ");
    scanf("%c", &op);

    if (op == '+' || op == '-' || op == '*' || op == '/')
        printf("Valid arithmetic operator\n");
    else
        printf("Invalid operator\n");

    return 0;
}
```
# OUTPUT
<img width="284" height="169" alt="image" src="https://github.com/user-attachments/assets/974c3945-3029-4909-bbb5-599e124eb4dc" />

