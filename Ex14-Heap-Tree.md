# Ex14 Heap Tree
## DATE:17/03/2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1. Start 
2. Find the index of the element num in the array. 
3. Swap the element to be deleted with the last element in the array. 
4. Decrease the array size (size) by 1. 
5. Start heapifying from the last non-leaf node (index size/2 - 1). 
6. Call heapify() to restore the heap property for each node. 
7. End

## Program:
```

Program to delete an element in a Heap Tree

Developed by: Shanmuga Vasanth M

RegisterNumber:  212223040191
```
```
void deleteRoot(int array[], int num) 
{ 
int i; 
for(i=0;i<size;i++) 
{ 
if(num==array[i]) 
{ 
break; 
} 
} 
swap(&array[i],&array[size-1]); 
size-=1; 
for(i=size/2-1;i>=0;i--) 
{ 
heapify(array,size,i); 
} 
}
```

## Output:

![437415338-6f7c138e-f362-4f98-b868-cb5eecaa33a7](https://github.com/user-attachments/assets/b1880cd7-b5b8-4bf3-972e-61861cbc8ac5)


## Result:

Thus, the function to delete an element in a Heap Tree is implemented successfully.
