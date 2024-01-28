Bubble sort is a simple sorting algorithm that repeatedly steps through the list, compares adjacent elements, and swaps them if they are in the wrong order. The pass through the list is repeated until the list is sorted.

Here's a simple implementation of the bubble sort algorithm in Python:

```python
def bubble_sort(arr):
    n = len(arr)

    # Traverse through all array elements
    for i in range(n):
        # Last i elements are already in place, so we don't need to check them
        for j in range(0, n-i-1):
            # Swap if the element found is greater than the next element
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]

# Example usage:
my_list = [64, 34, 25, 12, 22, 11, 90]
bubble_sort(my_list)

print("Sorted array:", my_list)
```

In this implementation, the `bubble_sort` function takes an array as input and sorts it in ascending order using the bubble sort algorithm. The outer loop (`for i in range(n)`) represents each pass through the array, and the inner loop (`for j in range(0, n-i-1)`) compares adjacent elements and swaps them if they are in the wrong order.

Note: Bubble sort is not the most efficient sorting algorithm, especially for large datasets, but it is easy to understand and implement. There are more efficient sorting algorithms like merge sort or quicksort for larger datasets.
