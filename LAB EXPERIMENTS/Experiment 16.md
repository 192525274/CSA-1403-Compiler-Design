## PROGRAM
```
#include <stdio.h>

int main() {
    char a, b, op, c;

    printf("Enter three address code: ");
    scanf(" %c = %c %c %c", &a, &b, &op, &c);

    printf("\nMOV R0, %c\n", b);

    if (op == '+')
        printf("ADD R0, %c\n", c);
    else if (op == '-')
        printf("SUB R0, %c\n", c);
    else if (op == '*')
        printf("MUL R0, %c\n", c);
    else if (op == '/')
        printf("DIV R0, %c\n", c);

    printf("MOV %c, R0\n", a);

    return 0;
}
```
# OUTPUT
<img width="355" height="171" alt="image" src="https://github.com/user-attachments/assets/147e9f1f-3082-464c-bcaf-7f85426006c2" />

