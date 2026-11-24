## PROGRAM
```
#include <stdio.h>
#include <string.h>

int main() {
    char input[50];

    printf("Enter input string: ");
    scanf("%s", input);

    if (strcmp(input, "id") == 0 ||
        strcmp(input, "id+id") == 0 ||
        strcmp(input, "id*id") == 0)
        printf("String is accepted\n");
    else
        printf("String is rejected\n");

    return 0;
}
```
# OUTPUT
<img width="364" height="142" alt="image" src="https://github.com/user-attachments/assets/09e6000e-7527-46da-a9e0-f4ee47c648e5" />

