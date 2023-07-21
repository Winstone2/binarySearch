# binarySearch
Thought Process:

    We start with defining two pointers, left and right, which represent the current search space within the sorted array.
    We then enter a loop, which continues as long as the left pointer is less than or equal to the right pointer. If left becomes greater than right, we've exhausted the search space, and the element is not present in the array.
    Inside the loop, we calculate the mid index, which is the middle index of the current search space.
    We check if the element at the mid index is equal to the target. If it is, we have found the element, and we return its index.
    If the element at the mid index is less than the target, we know the target must be in the right half of the search space. So, we update the left pointer to mid + 1 to search in the right half.
    If the element at the mid index is greater than the target, we know the target must be in the left half of the search space. So, we update the right pointer to mid - 1 to search in the left half.
    We continue the loop, dividing the search space in half at each step, until we find the element or exhaust the search space.
    Edge Cases to Consider:

    If the array is empty, the search should return -1 since the element cannot be found.
    If the array has only one element, we can directly check if it matches the target or not.
    Ensure that the array is sorted because binary search only works on sorted arrays. If the array is not sorted, the results will be incorrect.
    If the target is outside the range of the array (less than the first element or greater than the last element), return -1 as the element cannot exist in the array.

Keep in mind that binary search is most efficient for large sorted arrays. For smaller arrays or unsorted arrays, linear search might be more suitable.
