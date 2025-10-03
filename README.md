# Aim: To study Sorting Algorithms in C plus plus

## Theory:

Sorting is the process of arranging data elements in a specific order, usually in ascending or descending sequence. It is one of the most fundamental operations in computer science, as it makes searching, organizing, and processing data more efficient.

There are several types of sorting algorithms, each with its own method and efficiency:

- **Selection Sort** – Repeatedly finds the smallest (or largest) element and places it in its correct position. Easy to implement but has higher time complexity.

- **Bubble Sort** – Compares adjacent elements and swaps them if they are in the wrong order. This process repeats until the list is sorted. Simple but inefficient for large data sets.

- **Quick Sort** – Another divide-and-conquer method that selects a pivot, partitions the array, and recursively sorts the subarrays. Generally faster in practice than merge sort.

## 1. Algorithm: For Selection sorting

**Step 1**: Start

**Step 2**: Take an unsorted array of size n.

**Step 3**: Repeat the following for i = 0 to n-2: Assume the element at index i is the minimum (min_idx = i). Compare this element with all elements to its right (j = i+1 to n-1).

**Step 4**: If any element arr[j] is smaller than arr[min_idx], update min_idx = j. After the inner loop ends, swap arr[i] and arr[min_idx].

**Step 5**: Continue until the whole array is sorted.

**Step 6**: Print the sorted array.

**Step 7**: End

## 2.Algorithm: for Bubble sort

**Step 1**: Start

**Step 2**: Input an array of integers.

**Step 3**: Sort the array using Bubble Sort:

- Repeat for i = 0 to n-2:

- For each j = 0 to n-i-2:

- If arr[j] > arr[j+1], swap them.

**Step 4**: Display the sorted array.

**Step 5**: Input the target element to search.

**Step 6**: Apply Binary Search:

- Initialize low = 0, high = n-1.

- Repeat while low <= high:

- Find mid = (low + high)/2.

- If arr[mid] == target, return index.

- Else if arr[mid] < target, set low = mid+1.

- Else set high = mid-1.

**Step 7**: If element found, print index; otherwise print "not found".

**Step 8**: End

## 3. Algorithm: For Quick sorting

**Step 1**: Start

**Step 2**: Partition function (partition(arr, low, high)): Choose the last element as pivot (arr[high]). Initialize index i = low - 1. For each j = low to high - 1:

- If arr[j] < pivot:

- Increment i. Swap arr[i] and arr[j]. After loop, swap arr[i+1] and arr[high]. Return i+1 (partition index).

**Step 3**: Quick Sort function (quickSort(arr, low, high)): If low < high:

- Call partition(arr, low, high) to get pivot index pi. Recursively call quickSort(arr, low, pi - 1). Recursively call quickSort(arr, pi + 1, high).

**Step 4**: Main function:

- Initialize an array arr = {10,7,8,9,1,5}. Call quickSort(arr, 0, n-1). Print the sorted array.

**Step 5**: End

## Conclusion

Through this experiment, we learned how sorting algorithms arrange data in a specific order, making it easier to search and process. 
By implementing sorting in C++, we understood the working of basic algorithms like Bubble Sort, Selection Sort, and Quick Sort.
