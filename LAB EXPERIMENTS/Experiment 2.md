## PROGRAM
```
#include <stdio.h>
#include <string.h>

int main() {
    char s[200];

    printf("Enter a line: ");
    fgets(s, sizeof(s), stdin);

    if (strncmp(s, "//", 2) == 0 ||
        (strncmp(s, "/*", 2) == 0 && strstr(s, "*/") != NULL))
        printf("It is a comment.\n");
    else
        printf("It is not a comment.\n");

    return 0;
}
```
# OUTPUT
<img width="279" height="152" alt="image" src="https://github.com/user-attachments/assets/9654f4a0-80f3-4d8d-a10a-d3809302c56d" />

