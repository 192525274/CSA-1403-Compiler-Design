## PROGRAM
```
#include <stdio.h>

int main() {
    printf("Grammar:\n");
    printf("S -> AaAb | BbBa\n");
    printf("A -> epsilon\n");
    printf("B -> epsilon\n\n");

    printf("FOLLOW(S) = { $ }\n");
    printf("FOLLOW(A) = { a, b }\n");
    printf("FOLLOW(B) = { a, b }\n");

    return 0;
}
```
# OUTPUT
<img width="308" height="203" alt="image" src="https://github.com/user-attachments/assets/cc8eb4b6-58bf-462c-be9c-53f5cb6e84ec" />

