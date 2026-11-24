## PROGRAM
```
#include <stdio.h>
#include <ctype.h>

int main() {
    char s[300];
    int i = 0;

    printf("Enter input: ");
    fgets(s, sizeof(s), stdin);

    while (s[i]) {
        if (isspace(s[i])) {
            i++;
        }
        else if (s[i] == '/' && s[i + 1] == '/') {
            break;
        }
        else if (s[i] == '/' && s[i + 1] == '*') {
            i += 2;
            while (s[i] && !(s[i] == '*' && s[i + 1] == '/'))
                i++;
            i += 2;
        }
        else {
            printf("%c", s[i++]);
        }
    }
```
# OUTPUT
<img width="287" height="182" alt="image" src="https://github.com/user-attachments/assets/226e710c-dc12-459f-a335-9468635d006b" />


    return 0;
}
