## print all the letters of the English alphabet.

# AIM:
To write a C program to print all the letters of the English alphabet.

# Algorithm
Start
Initialize a character variable ch with 'A'.
Loop from 'A' to 'Z':
Print the character.
Print a space after each character.
End the loop once 'Z' is printed.
End

# Program:

```
#include <stdio.h>

int main() {
    char ch;
    
    for (ch = 'A'; ch <= 'Z'; ch++) {
        printf("%c ", ch);
    }
    
    return 0;
}

```

# output:


<img width="567" height="153" alt="image" src="https://github.com/user-attachments/assets/7b068b1b-823f-4c13-8aee-57109a77a008" />

# result:

Thus the program was executed and the output was verified successfully.
