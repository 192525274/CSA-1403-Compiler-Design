## PROGRAM 
```
#include <stdio.h>

int main() {
    char ch;
    int spaces = 0, newlines = 0;

    printf("Enter text:\n");

    while ((ch = getchar()) != EOF) {
        if (ch == ' ' || ch == '\t')
            spaces++;

        if (ch == '\n')
            newlines++;
    }

    printf("Whitespaces = %d\n", spaces);
    printf("Newlines = %d\n", newlines);

    return 0;
}
```
# OUTPUT
<img width="259" height="153" alt="image" src="https://github.com/user-attachments/assets/a64da020-b393-4d24-a5d5-04b82f1fd811" />

