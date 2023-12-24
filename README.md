# Selection sort and Insertion sort
## Aim:
To write a program to perform selection sort and insertion sort using python programming.
## Equipment’s required:
1.	Hardware – PCs
2.	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
## Selection Sort Algorithm:
1.	Set the first unsorted element as the minimum
2.	For each of the unsorted elements, check if the element < current minimum.
3.	If yes, set the element as the new minimum.
4.	Swap minimum with first unsorted position.
5.	Repeat the steps 2 and 3 for all the elements in the array.
## Insertion Sort Algorithm:
1.	Set the first element as sorted element j.
2.	For each unsorted element X, check if current sorted element j >X.
3.	If yes, move sorted element to the right by 1.
4.	Break the loop and insert X.
5.	Repeat the steps 2 to 4 for sorting all the elements in the array.
## Program:
# Program to sort the elements in the list using the Selection Sort algorithm.
# Developed by: MARXIN LIJO M
# RegisterNumber: 23013468
# i) Selection Sort
```
def selection_sort(arr):
    # write your code here using selection sort
    n=len(arr)
    for i in range(n):
       min=i
       for j in range(i+1,n):
          if arr[j]<arr[min]:
              min=j
       arr[i],arr[min]=arr[min],arr[i]
    
list_of_nums = eval(input())
# use the selection sort function
# print the sorted list
selection_sort(list_of_nums)
print(list_of_nums)
```
# ii)	Insertion Sort
```
def selection_sort(arr):
    # write your code here using selection sort
    n=len(arr)
    for i in range(1,n):
       key=arr[i]
       j=i-1
       while j>=0 and key<arr[j]:
           arr[j+1]=arr[j]
           j-=1
       arr[j+1]=key
list_of_nums = eval(input())
# use the selection sort function
# print the sorted list
selection_sort(list_of_nums)
print(list_of_nums)
```
## Output:
![Screenshot 2023-12-24 211251](https://github.com/MARXINLIJO/Sorting-Algorithm/assets/145742540/7d0c452a-00c2-48ef-a430-472299246b6b)
![Screenshot 2023-12-24 211303](https://github.com/MARXINLIJO/Sorting-Algorithm/assets/145742540/4e8b8c05-3c9a-4ce0-9529-2164eab4a7c6)
## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
