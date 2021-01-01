Here I added the code on basics of array in **Python**
The Topics are:

    *  Insertion and Deletion in Arrays 
    *  Array Rotation 
    *  Reversing an Array 
     
    


```python
#Insertion and Deletion in Arrays
arr=[1,2,3,4,5,60]
#insert
arr.append(100)
#deletion
arr.remove(4)
print(arr)
#another way to delete
arr.pop()
print(arr)
```

    [1, 2, 3, 5, 60, 100]
    [1, 2, 3, 5, 60]
    

##**Array Rotation**

**Algo**
Say, arr[] = [1, 2, 3, 4, 5, 6, 7], K = 2
  * Store first K elements in a temp array
    temp[] = [1, 2]
  * Shift rest of the arr[]
    arr[] = [3, 4, 5, 6, 7, 6, 7]
  * Store back the K elements from temp
    arr[] = [3, 4, 5, 6, 7, 1, 2]


```python
#array_rotation
arr=[1,2,3,4,5,6,7]
s=len(arr)
k=2
new_arr=[]
arr_r=[]
count=0
for i in arr:
    if count<k:
        new_arr.append(i)
    elif count>=k:
        arr_r.append(i)
    count=1+count
arr_r.extend(new_arr)
print('The desired array after reversal is:',arr_r)

```

    The desired array after reversal is: [3, 4, 5, 6, 7, 1, 2]
    


```python
#reversing an array
arr=[1,2,3,4,5]
arr.reverse()
print(arr)
```

    [5, 4, 3, 2, 1]
    


```python

```
