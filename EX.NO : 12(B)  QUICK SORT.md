
# EX.NO : 12(B)  QUICK SORT 
 
# PROGRAM STATEMENT: 
 
To write the quickSort module of Quick Sort in CPP. 
 
# ALGORITHM:   
 
1. Start the program. 
2. If low < high, perform the following steps: 
a. Call the partition() function to find the pivot index pi. 
b. Recursively call quickSort() on the subarray to the left of pi (from low to pi-1). 
c. Recursively call quickSort() on the subarray to the right of pi (from pi+1 to high). 
3. End the program. 
 
# PROGRAM:
```
void quickSort(int array[], int low, int high)
{
    if(low<high)
    {
        int pi=partition(array,low,high);
        quickSort(array,low,pi-1);
        quickSort(array,pi+1,high);
    }
}
```

# output:

![image](https://github.com/user-attachments/assets/7bb39b52-fe4a-49f2-ae84-4bd4677c0a16)

# RESULT: 
 
Thus, the C++ program to write the quickSort module of Quick Sort in CPP is created successfully.
