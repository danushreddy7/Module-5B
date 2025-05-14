# NumPy Program: Column-wise Sorting of a 2D Array

## 🎯 Aim
To write a **NumPy** program that sorts the elements in each column of a given 2D array in ascending order.

## 🧠 Algorithm

1. **Import NumPy**: Start by importing the NumPy library.
2. **Get Input**: Accept a 2D NumPy array from the user.
3. **Sort Column-wise**: Use the `np.sort()` function with `axis=0` to sort each column in ascending order.
4. **Store Result**: Store the sorted result in a new array.
5. **Display Output**: Print the original array and the column-wise sorted array.

## 🧾 Program
```
import numpy as np

arr = np.array([[12, 5, 7],
                [4, 8, 9],
                [10, 1, 6]])
sorted_arr = np.sort(arr, axis=0)
print("Original array:\n", arr)
print("\nColumn-wise sorted array:\n", sorted_arr)
```
## Output:
```
    Input                              Result

Original array:              Column-wise sorted array:
 [[12  5  7]                 [[4 1 6]
 [ 4  8  9]                  [10 5 7]
 [10  1  6]]                 [12 8 9]]               
```
## Result:
The program was successful.
