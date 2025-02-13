# Linear Search and Binary search
## Aim:
To write a program to perform linear search and binary search using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Linear Search:
1.	Start from the leftmost element of array[] and compare k with each element of array[] one by one.
2.	If k matches with an element in array[] , return the index.
3.	If k doesn’t match with any of elements in array[], return -1 or element not found.
## Binary Search:
1.	Set two pointers low and high at the lowest and the highest positions respectively.
2.	Find the middle element mid of the array ie. arr[(low + high)/2]
3.	If x == mid, then return mid.Else, compare the element to be searched with m.
4.	If x > mid, compare x with the middle element of the elements on the right side of mid. This is done by setting low to low = mid + 1.
5.	Else, compare x with the middle element of the elements on the left side of mid. This is done by setting high to high = mid - 1.
6.	Repeat steps 2 to 5 until low meets high
## Program:
i)	#Use a linear search method to match the item in a list.
```
''' 
Program for linear search method to match the item in a list
Developed by:GAYATHRI.K
RegisterNumber: 23013439
'''
def linearSearch(array,n,k):
   for i in range(0,n):
       if(array[i]==k):
           return i
   return -1        
array = eval(input())
k = eval(input()) 
n=len(array)
array.sort()
print(array)
result = linearSearch(array,n,k)
if result != -1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")


```
ii)	# Find the element in a list using Binary Search(Iterative Method).
```
''' 
Program to find the element in a list using Binary Search(Iterative Method)..
Developed by:GAYATHRI.K
RegisterNumber: 23013439
'''
def binarysearchIter(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return -1
    
array=eval(input())
array.sort()
k=eval(input())
result=binarysearchIter(array,k,0,len(array)-1)
print(array)
if result !=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")
   
    





```
iii)	# Find the element in a list using Binary Search (recursive Method).
```
''' 
Program to find the element in a list using Binary Search (recursive Method).
Developed by: GAYATHRI.K
RegisterNumber:23013439 
'''
def binarysearchIter(array, k, low, high):
    while low<=high:
        mid=(low+high)//2
        if array[mid]==k:
            return mid
        elif array[mid]<k:
            low=mid+1
        else:
            high=mid-1
    return  -1
    
    
    
array = eval(input())
array.sort()

k = eval(input()) 
result=binarysearchIter(array,k,0,len(array)-1)
print(array)
if result !=-1:
    print(f"Element found at index:  {result}")
else:
    print(f"Element not found")




```
## Sample Input and Output
![Screenshot 2023-12-25 090656](https://github.com/GAYATHRI-K06/Search-Algorithm/assets/145742742/b3f88464-f87c-4f8e-82bf-c797ac23bd8b)
![Screenshot 2023-12-25 090705](https://github.com/GAYATHRI-K06/Search-Algorithm/assets/145742742/34a00064-d513-4ad6-b548-3a7e62274c02)
![Screenshot 2023-12-25 090716](https://github.com/GAYATHRI-K06/Search-Algorithm/assets/145742742/ff3fff8f-fe6c-4d4f-8104-6109ab6b5595)


## Result
Thus the linear search and binary search algorithm is implemented using python programming.
