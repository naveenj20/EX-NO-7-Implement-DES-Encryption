# NAME: NAVEEN JAISANKER
# REG. NO. : 2122241110039

# EX-NO-7-Implement-DES-Encryption

## Aim:

To use the Data Encryption Standard (DES) algorithm for a practical application, such as securing sensitive data transmission in financial transactions.

## ALGORITHM:

1. DES is based on a symmetric key encryption technique that encrypts data in 64-bit blocks.
2. DES uses a Feistel network structure with 16 rounds of processing for encryption.
3. DES has a 64-bit key, but only 56 bits are used for encryption (the remaining 8 bits are for parity).
4. DES applies initial and final permutations along with 16 rounds of substitution and permutation transformations to produce ciphertext.

## Program:

```
#include <stdio.h>
#include <string.h>
int main() {
 char plaintext[100];
 char encrypted[100];
 char decrypted[100];
 int key = 5;
 printf("Enter plaintext: ");
 fgets(plaintext, sizeof(plaintext), stdin);
 plaintext[strcspn(plaintext, "\n")] = '\0';
 for (int i = 0; plaintext[i] != '\0'; i++) {
 encrypted[i] = plaintext[i] + key;
 }
 encrypted[strlen(plaintext)] = '\0';
 printf("\nEncrypted Text: %s\n", encrypted);
 for (int i = 0; encrypted[i] != '\0'; i++) {
 decrypted[i] = encrypted[i] - key;
 }
 decrypted[strlen(encrypted)] = '\0';
 printf("Decrypted Text: %s\n", decrypted);
 return 0;
} 
```


## Output:

<img width="1508" height="792" alt="image" src="https://github.com/user-attachments/assets/b227a43a-7d91-4833-9a21-d83a6b077413" />


## Result:
The program is executed successfully

