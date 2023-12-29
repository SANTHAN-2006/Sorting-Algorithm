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
i)	#Selection Sort
```
''' 
Program to sort the elements in the list using the Selection Sort algorithm.
Developed by: K Santhan Kumar
RegisterNumber: 212223240065
'''
def selection_sort(nums):
    for i in range(len(nums)):
        lowest_index_value=i
        for j in range(i+1,len(nums)):
            if nums[j]<nums[lowest_index_value]:
                lowest_index_value=j
        nums[i],nums[lowest_index_value] = nums[lowest_index_value],nums[i]
        
        
list_of_nums = eval(input())
selection_sort(list_of_nums)
print(list_of_nums)
```
ii)	#Insertion Sort
```
''' 
Program to sort the elements in the list using the Insertion Sort algorithm.
Developed by: K Santhan Kumar
RegisterNumber: 212223240065
'''
def insertion_sort(nums):
    for i in range(1,len(nums)):
        items = nums[i]
        j=i-1
        while j>=0 and nums[j]>items:
            nums[j+1]=nums[j]
            j-=1
        nums[j+1]=items

list_of_nums=eval(input())
insertion_sort(list_of_nums)
print(list_of_nums)
```

## Output:
i)
![image](https://github.com/SANTHAN-2006/Sorting-Algorithm/assets/80164014/af92ce4d-4e52-4dc5-b097-1332791dd762)

ii)
![image](https://github.com/SANTHAN-2006/Sorting-Algorithm/assets/80164014/4ba71a19-0bcd-4e77-9ca0-9a4fa4dd60b8)

## Result:
Thus the program is written to perform selection sort and insertion sort using python programming.
