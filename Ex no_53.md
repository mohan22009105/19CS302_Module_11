# EX 53 C program to remove duplicates in an array.

## AIM:
To write a C program to remove duplicates in an array.

## Algorithm

Start
Input the number of elements n.
Input n elements into the array.
Create an empty temporary array temp to store unique elements.
Initialize an index variable index = 0.
Loop through each element in the original array:
Check if the element already exists in temp.
If the element is not a duplicate, add it to temp and increment index.
Copy the elements from temp back to the original array.
Update n to the new size of the array.
Print the modified array without duplicates.
End
This step-by-step method ensures that duplicates are effectively removed while maintaining the order of unique elements. Let me know if you need optimizations! 🚀  

## Program:
```
#include <stdio.h>

void removeDuplicates(int arr[], int *n) {
    int temp[*n];
    int index = 0;

    for (int i = 0; i < *n; i++) {
        int duplicate = 0;
        for (int j = 0; j < index; j++) {
            if (arr[i] == temp[j]) {
                duplicate = 1;
                break;
            }
        }
        if (!duplicate) {
            temp[index++] = arr[i];
        }
    }

    for (int i = 0; i < index; i++) {
        arr[i] = temp[i];
    }

    *n = index;
}

int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n];
    printf("Enter the elements: ");
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    removeDuplicates(arr, &n);

    printf("Array after removing duplicates: ");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    
    return 0;
}
```

## Output:

<img width="455" height="251" alt="image" src="https://github.com/user-attachments/assets/3d55db70-0fb2-40ec-b4a7-68817ad461b0" />




## Result:
Thus the program was executed and the output was verified successfully.
