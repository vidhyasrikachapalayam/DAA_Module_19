# EX 1A Decimal to Binary using recursive function
## DATE: 
## AIM:
To write a program to create a recursive function to convert decimal number to binary number.

## Algorithm
1. Read an integer n.
2. Check base condition iff n <= 0, return 0.
3. Calculate n % 2, recursively call binary(n // 2).
4. Multiply the result of recursive call by 10 and add (n % 2) to it.
5. Print the final binary number.

## Program:

```
Program to implement decimal to binary using recursive function
Developed by: Vidhyasri.k
Register Number: 212222230170
```
```
def binary(n):
    if n<=0:
        return 0
    return n%2 +(10*binary(n//2))
n=int(input())
print(binary(n))
```

## Output:

![image](https://github.com/user-attachments/assets/29c4b7c9-1423-45ae-acea-43469f9385dd)

## Result:
Thus the program is written to convert the decimal number to binary number using recursive function was executed successfully.
