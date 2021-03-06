## List mutability

```python
>>> def change(L):
	L[0] = 'python'

	
>>> mylist = [12, 3, 45, 2]
>>> change(mylist)
>>> mylist
['python', 3, 45, 2]
```

## Selection sort

```python
def selectsort(L):
    for i in range(len(L)):
        # Unsorted sub list
        U = L[i:]
        # The smallest in the sublist
        m = min(U)
        # index of the smallest 
        j = L.index(m, i)
        # swap
        L[i], L[j] = L[j], L[i]
    return L


L = [12, 4, 7, 56, 2]
selectsort(L)
print(L)
```

## Sorting

Sorting is the arrangement of set in order
- sorting a set of numbers
- sorting a set of words

### Sorting a set of numbers 
Consider the list of prices of mobile phones of different brands (in thousands).
```
price = [ 54, 23, 45, 12,  14,  11, 10, 12]
```
Now, we want to find the first three mobile phones with least prices. 
(Example: sort by price option in Amazon) 

```
Before sorting,
  price = [ 54, 23, 45, 12,  14,  11, 10, 12]
After sorting,
  price = [ 10, 11, 12, 12, 14, 23,  45, 54]
```

### Question
Write the python code to display the price of first three items with the least price.

### Sorting a set of words
Consider the set of new students joined in a program,
```
  students = [ ‘akil’, ‘kapil’, ‘aakash’, ‘aswin’]
```
We want the computer to allot `rollno` for each student. For this, we need to sort the list first.

After sorting, 
```
students = [‘aakash’, ‘akil’, ‘aswin’, ‘kapil’]
```

### Question
Write the python code to allot `rollno` for each student.
```python 
students = {‘aakash’: '17CSE01', ‘akil’: '17CSE02', 
            ‘aswin’: '17CSE03' , ‘kapil’: '17CSE04'}
```

## Importance
- Sorting is the essential part of computing. Sorting takes ~ 30% of all the computing time spent.
- It is easier to `search` an item in the sorted set. Thus, sorting is the pre-requistie for the search algorithms.

# Merge sort
Now, how do we sort the given array? There are several algorithms to sort an array. Let's see how merge sort works.








