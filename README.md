## Solving Codeforces problem 

I. Welcome for you with Conditions : https://codeforces.com/group/MWSDmqGsZm/contest/219158/problem/I 

```c
#include <stdio.h>

int main()
{
    int a, b;
    scanf("%d %d", &a, &b);

    if (a >= b)
    {
        printf("Yes");
    }
    else
    {
        printf("No");
    }

    return 0;
}
```
J. Multiples : https://codeforces.com/group/MWSDmqGsZm/contest/219158/problem/J


```c
#include <stdio.h>

int main()
{
    int a, b;
    scanf("%d %d", &a, &b);

    if (a%b == 0 || b%a == 0)
    {
        printf("Multiples");
    }
    else
    {
        printf("No Multiples");
    }
    return 0;
}
```

P. First digit ! https://codeforces.com/group/MWSDmqGsZm/contest/219158/problem/P


```c
#include <stdio.h>

int main()
{
    int x;
    scanf("%d", &x);

    // find the first digit as dividing int with int will be become int number even if it come fractional like 365/10 = 36.5 it will be 36

    //  for finding first digit 4569/1000 = 4

    int firstDigit = x / 1000;

    if (firstDigit % 2 == 0)
    {
        printf("EVEN");
    }
    else
    {
        printf("ODD");
    }
    return 0;
}
```
- eliminating last digit 

```c
#include <stdio.h>

int main()
{
    int x;
    scanf("%d", &x);


    int last_digit = x % 10;

    printf("%d \n", last_digit);

    if (last_digit % 2 == 0)
    {
        printf("EVEN");
    }
    else
    {
        printf("ODD");
    }
    return 0;
}
```

## Understanding character 

![alt text](image.png)

```c
#include <stdio.h>

int main()
{
    char c = 'B';
    printf("%c", c);
    printf("%d", c); // as memory stores asci value of the char it will show result as well asci value of b is 66

    // char keep 1 byte = 8 bit means 2 ^ 8 = 256 char we can store 
    return 0;
}
```
- value to char and char to value conversion can be done 


N. Char : https://codeforces.com/group/MWSDmqGsZm/contest/219158/problem/N


```c
#include <stdio.h>

int main()
{
    char x;
    scanf("%c", &x);

    if (x >= 'a' && x <= 'z')
    {
        x = x - 32;

        printf("%c", x);
    }
    else
    {
        x = x + 32;

        printf("%c", x);
    }

    return 0;
}
```

M. Capital or Small or Digit : https://codeforces.com/group/MWSDmqGsZm/contest/219158/problem/M

```c
#include <stdio.h>

int main()
{
    char ch;
    scanf("%c", &ch);

    if (ch >= '0' && ch <= '9')
    {
        printf("IS DIGIT");
    }
    else
    {
        printf("ALPHA \n");

        if (ch >= 'a' && ch <= 'z')
        {

            printf("IS SMALL");
        }
        else
        {
            printf("IS CAPITAL");
        }
    }
    return 0;
}
```

K. Max and Min : https://codeforces.com/group/MWSDmqGsZm/contest/219158/problem/K

```c
#include <stdio.h>

int main()
{
    int a, b, c;
    scanf("%d %d %d", &a, &b, &c);

    // min among them 
     if (a <= b && a <= c)
    {
        printf("%d ", a);
    }
    else if (b <= a && b <= c)
    {
        printf("%d ", b);
    }
    else if (c <= a && c <= b)
    {
        printf("%d ", c);
    }

    // max among them 
    if (a >= b && a >= c)
    {
        printf("%d", a);
    }
    else if (b >= a && b >= c)
    {
        printf("%d", b);
    }
    else if (c >= a && c >= b)
    {
        printf("%d", c);
    }

    return 0;
}
```


