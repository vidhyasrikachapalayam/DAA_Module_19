# EX 1B Merge Sort
## DATE:
## AIM:
To write a python program to sort the first half of the list using merge sort.

## Algorithm
1. Read n elements from the user and store them in an array arr.
2. Recursively split the array into two halves L (left) and R (right) until each subarray contains one element.
3. Recursively apply merge sort only on the right half R (Note: the left half is not sorted due to a missing mergeSort(L)).
4. Merge the sorted subarrays L and R back into the original array arr in sorted order.
5. Print the original and the final sorted array using the printList function.

## Program:
```
Program to implement Merge Sort
Developed by: Vidhyasri.k
Register Number: 212222230170
```
```
def mergeSort(arr):
    if len(arr) > 1:
        mid = len(arr) // 2
        L = arr[:mid]
        R = arr[mid:]
        
        mergeSort(R) 
        
        i = j = k = 0
        
        while i < len(L) and j < len(R):
            if L[i] < R[j]:
                arr[k] = L[i]
                i += 1
            else:
                arr[k] = R[j]
                j += 1
            k += 1
       
        while i < len(L):
            arr[k] = L[i]
            i += 1
            k += 1
        
        while j < len(R):
            arr[k] = R[j]
            j += 1
            k += 1

def printList(arr):
    for i in range(len(arr)):
        print(arr[i], end=" ")
    print()


n = int(input())
arr = []
for i in range(n):
    l = int(input())
    arr.append(l)

print("Given array is")
printList(arr)

mergeSort(arr)

print("\nSorted array is")

printList(arr)
```

## Output:

![image](https://github.com/user-attachments/assets/af0cfa5e-0a80-4eba-8679-4766d8ab44c5)

## Result:
The program successfully sorts the first half of the given array using merge sort. where only the first half is sorted, and the second half remains unchanged.
