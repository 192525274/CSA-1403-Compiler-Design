## PROGRAM
```
#include <stdio.h>

int main() {
    printf("Original Grammar:\n");
    printf("S -> iEtS | iEtSeS | a\n");
    printf("E -> b\n\n");

    printf("After left factoring:\n");
    printf("S  -> iEtS S' | a\n");
    printf("S' -> eS | epsilon\n");
    printf("E  -> b\n");

    return 0;
}
```
# OUTPUT
<img width="313" height="188" alt="image" src="https://github.com/user-attachments/assets/2a89709f-0d09-4188-816d-b47d7a396f8d" />

