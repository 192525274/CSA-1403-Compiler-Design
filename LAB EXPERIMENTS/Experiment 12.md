## PROGRAM
```
#include <stdio.h>

char s[50];
int i = 0;

void E();
void T();
void F();

void E() {
    T();

    while (s[i] == '+') {
        i++;
        T();
    }
}

void T() {
    F();

    while (s[i] == '*') {
        i++;
        F();
    }
}

void F() {
    if (s[i] == 'i') {
        i++;
    }
    else if (s[i] == '(') {
        i++;
        E();

        if (s[i] == ')')
            i++;
    }
}

int main() {
    printf("Enter expression: ");
    scanf("%s", s);

    E();

    if (s[i] == '\0')
        printf("Accepted\n");
    else
        printf("Rejected\n");

    return 0;
}
```
# OUTPUT
<img width="296" height="146" alt="image" src="https://github.com/user-attachments/assets/5c3d9edf-48a5-41a2-839a-472d65c2d7bb" />

