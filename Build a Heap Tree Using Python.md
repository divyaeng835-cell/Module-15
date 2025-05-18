# Ex. No: 15D - Build a Heap Tree Using Python

## AIM:
To write a Python program to build a heap tree using appropriate Python package and function.

## ALGORITHM:

1. **Start the program.**
2. Import the `heapq` module.
3. Define a function `heaptree(li)` that takes a list `n` as input.
4. Use `heapq.heapify(li)` to convert the list into a min-heap.
5. Print the created heap.
6. **End the program.**


## PROGRAM:

```
import heapq
def heapoprn(li):
    heapq.heapify(li)
    print ("The created heap is : ",li)
    print("The 3 smallest numbers in Heap are : ",end="")
    print(heapq.nsmallest(3, li))

```

## OUTPUT
![Screenshot 2025-05-18 173515](https://github.com/user-attachments/assets/f7c53f0f-99cf-4ff6-a2c1-9aca8e11daed)
## RESULT
Thus the Python program to build a heap tree using appropriate Python package and function has been implemented and executed.
