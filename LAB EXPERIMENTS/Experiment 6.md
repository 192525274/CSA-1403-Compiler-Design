## PROGRAM
```
#include <stdio.h>
#include <ctype.h>

int main() {
    char s[50];
    int i, valid = 1;

    printf("Enter identifier: ");
    scanf("%s", s);

    if (!(isalpha(s[0]) || s[0] == '_'))
        valid = 0;

    for (i = 1; s[i] != '\0'; i++) {
        if (!(isalnum(s[i]) || s[i] == '_')) {
            valid = 0;
            break;
        }
    }

    if (valid)
        printf("Valid Identifier\n");
    else
        printf("Invalid Identifier\n");

    return 0;
}
```
# OUTPUT
<img width="347" height="149" alt="image" src="https://github.com/user-attachments/assets/ed1104ff-81cd-4e4c-96e3-20d27f8e7a9b" />

