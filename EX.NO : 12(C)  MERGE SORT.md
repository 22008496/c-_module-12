
# EX.NO : 12(C)  MERGE SORT 
 
# PROGRAM STATEMENT: 
 
To write the mergeSort Module of Merge Sort in CPP. 
 
 
# ALGORITHM:   
 
1. Start the program. 
2. If l < r, perform the following steps: 
a. Calculate the middle index m = l + (r - l) / 2. 
b. Recursively call mergeSort() on the left subarray (from l to m). 
c. Recursively call mergeSort() on the right subarray (from m + 1 to r). 
d. Call the merge() function to merge the two sorted subarrays (from l to m and from m+1 to r). 
3. End the program 
 
# PROGRAM:  
```
void mergeSort(int arr[], int l, int r)
{
    if (l < r) {
        // Same as (l+r)/2, but avoids overflow for
        // large l and h
        int m = l + (r - l) / 2;
  
        // Sort first and second halves
        mergeSort(arr, l, m);
        mergeSort(arr, m + 1, r);
  
        merge(arr, l, m, r);
    }
}
```

# output:

![image](https://github.com/user-attachments/assets/3d61634c-ebd5-4db6-a3b9-e3179c806167)

# RESULT: 
 
Thus, the C++ program To write the mergeSort Module of Merge Sort in CPP.is created successfully.
