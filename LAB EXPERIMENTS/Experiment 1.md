## PROGRAM
```
#include <stdio.h>
#include <ctype.h>
#include <string.h>

int main() {
    char s[200];
    int i = 0;

    printf("Enter a C statement: ");
    fgets(s, sizeof(s), stdin);

    while (s[i] != '\0') {
        if (isspace(s[i])) {
            i++;
        }
        else if (isalpha(s[i]) || s[i] == '_') {
            printf("Identifier: ");
            while (isalnum(s[i]) || s[i] == '_')
                printf("%c", s[i++]);
            printf("\n");
        }
        else if (isdigit(s[i])) {
            printf("Constant: ");
            while (isdigit(s[i]) || s[i] == '.')
                printf("%c", s[i++]);
            printf("\n");
        }
        else if (strchr("+-*/=%", s[i])) {
            printf("Operator: %c\n", s[i++]);
        }
        else {
            i++;
        }
    }

    return 0;
}

```
# OUTPUT
<img width="299" height="182" alt="image" src="https://github.com/user-attachments/assets/7db22a4a-05cf-4e89-a196-7e4089b8fab6" />

