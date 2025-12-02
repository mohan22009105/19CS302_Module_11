## Task

# Write a function int max_of_four(int a, int b, int c, int d) which reads four arguments and returns the greatest of them.

# algorithim:

Start
Accept four integer inputs: a, b, c, and d.
Initialize max with a.
Compare max with b:
If b is greater than max, update max = b.
Compare max with c:
If c is greater than max, update max = c.
Compare max with d:
If d is greater than max, update max = d.
Return max as the largest number.
End

# program:
```
#include<stdio.h>
int compare(int a[4])
{
    int max=a[0];
    for(int i=0;i<4;i++)
    {
        if(a[i]>max)
        max=a[i];
    }
    return max;
}
int main()
{
    int a[4];
    for(int i=0;i<4;i++)
    scanf("%d",&a[i]);
    int d= compare(a);
    printf("%d",d);
}
```
# output:

<img width="814" height="374" alt="image" src="https://github.com/user-attachments/assets/0e3684a9-24b8-4d36-87fe-2cfa238c4d9d" />



# result:

Thus, the program is executed and verified successfully.
