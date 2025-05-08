#include <stdio.h>

int main() {
    // Define a string
    char *str = "\\Hello World";

    // Print the original string
    printf("Original string: %s\n", str);
    printf("AND and XOR with 127:\n\n");

    // Loop through each character in the string
    int i;
    for ( i = 0; str[i] != '\0'; i++) {
        char ch = str[i];              // Current character
        int and_result = ch & 127;     // AND operation with 127
        int xor_result = ch ^ 127;     // XOR operation with 127

        // Print results
        printf("Character: %c\tAND: %d\tXOR: %d\n", ch, and_result, xor_result);
    }

    return 0;
}
