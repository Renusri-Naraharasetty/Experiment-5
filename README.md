# Experiment-5
## AIM:Write a python program for Binary Search and inspect for failures. 

# ALGORITHM

1.Start the program.

2. Get the list from the user
   
3. Get the element to be searched
   
4. Compare the mid element with the key, if same return the index
  
5. If key is greater, search it in the right side, else search it in the left side.
  
6. If not found return -1
  
7. Stop the program. 

 # PROGRAM
 ```python
def binary_search(arr,target):
    low,high=0,len(arr)-1

    while low<=high:
        mid=(low+high)//2
        if arr[mid]==target:
            return mid
        elif arr[mid]<target:
            low=mid+1
        else:
            high=mid-1
    return -1

arr=[2,8,54,48,85,96]
target=int(input("Enter the number to search :"))
result=binary_search(arr,target)

if result != -1:
    print(f"{target} found at index {result}")
else:
    print(f"{target} not found in the list")
```

 # OUTPUT
<img width="1489" height="186" alt="image" src="https://github.com/user-attachments/assets/fc419a53-c52c-499b-a0de-3736824de4a5" />


 # RESULT
 Thus, the python program of binary search is implemented and the output is verified successfully.

