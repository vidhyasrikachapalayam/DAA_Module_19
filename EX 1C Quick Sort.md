# EX 1C Quick Sort
## DATE:
## AIM:
To write a python program to implement quick sort using tha last element as pivot on the list of integers.

## Algorithm
1. Read the size n and the n elements of the array.
2. Call quickSort(arr, 0, n), which divides the array based on a pivot element.
3. Reorder elements so that values smaller than the pivot are on the left and larger ones on the right.
4. Reorder elements so that values smaller than the pivot are on the left and larger ones on the right.
5. Finally, place the pivot in its correct sorted position.
6. After all recursive calls complete, print the sorted array.

## Program:
```
Program to implement implement quick sort using the last element as pivot on the list of integers.
Developed by: Vidhyasri.K
Register Number: 212222230170 
```
```
def quickSort(arr,st,en):
    if en-st>1:
        p=partition(arr,st,en)
        quickSort(arr,st,p)
        quickSort(arr,p+1,en)
def partition(arr,st,en):
    pivot=arr[st]
    i=st+1
    j=en-1
 
    while True:
        while(i<=j and arr[i]<=pivot):
            i=i+1
        while(i<=j and arr[j]>=pivot):
            j=j-1
        if i<=j:
            arr[i],arr[j]=arr[j],arr[i]
        else:
            arr[st],arr[j]=arr[j],arr[st]
            return j


arr=[]
n=int(input())
for i in range(n):
    arr.append(int(input()))


quickSort(arr, 0, len(arr))
print("Sorted array is:")
for i in range(len(arr)):
    
    print(arr[i])
```

## Output:

![image](https://github.com/user-attachments/assets/21625f7f-703b-49d6-af41-2b56b7e96519)

## Result:
The program successfully sorts the input array using the QuickSort algorithm, arranging the elements in ascending order.
