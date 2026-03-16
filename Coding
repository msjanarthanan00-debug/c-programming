#include <stdio.h>
#include <string.h>
#include <ctype.h>

void main() {
    char str[100], temp[100];
    int ch;

    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    str[strcspn(str, "\n")] = '\0';

    do {
        printf("\n--- STRING OPERATIONS ---\n");
        printf("1.Length  2.Copy  3.Concat  4.Compare\n");
        printf("5.Reverse 6.Upper 7.Lower  8.Exit\n");
        printf("Enter choice: ");
        scanf("%d", &ch); getchar();

        switch (ch) {
            case 1: printf("Length: %lu\n", strlen(str)); break;
            case 2: strcpy(temp, str); printf("Copied: %s\n", temp); break;
            case 3:
                printf("Enter string: "); fgets(temp, sizeof(temp), stdin);
                temp[strcspn(temp, "\n")] = '\0';
                strcat(str, temp); printf("Concatenated: %s\n", str); break;
            case 4:
                printf("Enter string: "); fgets(temp, sizeof(temp), stdin);
                temp[strcspn(temp, "\n")] = '\0';
                printf("Compare result: %d\n", strcmp(str, temp)); break;
            case 5: strrev(str); printf("Reversed: %s\n", str); break;
            case 6:
                for (int i=0; str[i]; i++) str[i] = toupper(str[i]);
                printf("Uppercase: %s\n", str); break;
            case 7:
                for (int i=0; str[i]; i++) str[i] = tolower(str[i]);
                printf("Lowercase: %s\n", str); break;
            case 8: printf("Exiting...\n"); break;
            default: printf("Invalid choice!\n");
        }
    } while (ch != 8);
}
