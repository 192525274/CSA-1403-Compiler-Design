## PROGRAM
```
#include <stdio.h>
#include <string.h>

struct symbol {
    char name[20];
    char type[20];
};

int main() {
    struct symbol table[20];
    int n = 0, i, choice;
    char name[20];

    while (1) {
        printf("\n1.Insert  2.Display  3.Search  4.Exit\n");
        printf("Enter choice: ");
        scanf("%d", &choice);

        if (choice == 1) {
            printf("Enter name and type: ");
            scanf("%s %s", table[n].name, table[n].type);
            n++;
        }
        else if (choice == 2) {
            printf("\nName\tType\n");
            for (i = 0; i < n; i++)
                printf("%s\t%s\n", table[i].name, table[i].type);
        }
        else if (choice == 3) {
            printf("Enter name: ");
            scanf("%s", name);

            for (i = 0; i < n; i++) {
                if (strcmp(name, table[i].name) == 0) {
                    printf("Found: %s %s\n",
                           table[i].name, table[i].type);
                    break;
                }
            }

            if (i == n)
                printf("Not Found\n");
        }
        else
            break;
    }

    return 0;
}
```
# OUTPUT
<img width="352" height="269" alt="image" src="https://github.com/user-attachments/assets/8c5f6f6b-3dee-471a-b305-3f9c504ec5c7" />

