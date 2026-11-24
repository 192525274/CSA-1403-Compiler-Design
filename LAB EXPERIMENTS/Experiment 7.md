## PROGRAM
```
#include <stdio.h>

int main() {
    printf("Grammar:\n");
    printf("S -> AaAb | BbBa\n");
    printf("A -> epsilon\n");
    printf("B -> epsilon\n\n");

    printf("FIRST(A) = { epsilon }\n");
    printf("FIRST(B) = { epsilon }\n");
    printf("FIRST(S) = { a, b }\n");

    return 0;
}
```
# OUTPUT
<img width="306" height="196" alt="image" src="https://github.com/user-attachments/assets/8971d6fe-ca1b-4be5-86ce-d3406b2fbe7b" />

