# EX 1D Linear search
## DATE:
## AIM:
To write a python program for a search function with parameter list name and the value to be searched on the given list of int values.

## Algorithm
1. Read an integer s (number of elements in the list).
2. Take s inputs from the user and store them in List.
3. Input the element n to be searched in the list.
4. Traverse each element i in List.
5. If the loop completes without finding n, print "Not Found"

## Program:
```
Program to implement a search function with parameter list name and the value to be searched on the given list of int values.
Developed by: Vidhyasri.K
Register Number: 212222230170
```
```
def search(List,n):
    for i in List:
        if i==n:
            print("Found")
            break
    else:
        print("Not Found")
s=int(input())
List=[input() for i in range(s)]
n=input()
```

## Output:

![image](https://github.com/user-attachments/assets/d349a000-a473-435d-8eb7-4110f5bf349a)

## Result:
The program was executed successfully, and it correctly checks if the input element is present in the list, printing "Found" if the element exists or "Not Found" if it does not.
