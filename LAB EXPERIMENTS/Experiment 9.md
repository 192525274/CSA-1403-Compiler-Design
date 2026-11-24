## PROGRAM
```
#include <stdio.h>

int main() {
    printf("Original Grammar:\n");
    printf("S -> (L) | a\n");
    printf("L -> L,S | S\n\n");

    printf("After eliminating left recursion:\n");
    printf("S  -> (L) | a\n");
    printf("L  -> S L'\n");
    printf("L' -> , S L' | epsilon\n");

    return 0;
}
```
# OUTPUT
<img width="295" height="189" alt="image" src="https://github.com/user-attachments/assets/a8996df7-e637-401b-8cc3-d148fad5dfa2" />

