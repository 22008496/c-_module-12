
# EX.NO : 12(D)  BINARY SEARCH ALGORITHM 
 
# PROGRAM STATEMENT: 
 
To write the Binary Search Module of Binary Search Algorithm in CPP. 
 
ALGORITHM:   
 
1. Start the program. 
2. Initialize beg = 0 and end = n. 
3. While beg <= end, perform the following: 
a. Calculate the middle index mid = (beg + end) / 2. 
b. If a[mid] == search, print "Element found at position mid + 1", and return 1 (indicating the element was found). 
c. If a[mid] > search, update end = mid - 1 to search the left half. 
d. Otherwise, update beg = mid + 1 to search the right half. 
4. If the loop ends without finding the element, return 0 (indicating the element was not found). 
5. End the program. 
 
# PROGRAM: 
```
int BS(int a[], int n, int search){
    int beg=0, end=n, mid;
    
    while(beg<=end)
    {
        mid=(beg+end)/2;
        if(a[mid]==search)
        {
            printf("Element found at %d position",mid + 1);
            return 1;
            break;
        }
        else if(a[mid] > search)
            end=mid-1;
        else
            beg=mid+1;
    }
    
    return 0;
}
```

# output:

![image](https://github.com/user-attachments/assets/494c3766-f474-4c0c-a764-d70ef843d87b)

# RESULT: 
 
Thus, the C++ program to write the Binary Search Module of Binary Search Algorithm in CP is created successfully.
