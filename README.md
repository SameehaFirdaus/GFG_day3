# GFG_day3
Given an array of integers arr []. Task is to reverse the given array.
---
Difficulty: Easy
Source: 160 Days of Problem Solving
Tags:
  - Arrays
---

# 🚀 _Day 3. Reverse an Array_ 🧠

The problem can be found at the following link: [Problem Link](https://www.geeksforgeeks.org/batch/gfg-160-problems/track/arrays-gfg-160/problem/reverse-an-array)
## 🔍 **Example Walkthrough:**

**Input:**  
`arr = [1, 4, 3, 2, 6, 5]`  
**Output:**  
`[5, 6, 2, 3, 4, 1]`

**Explanation:**  
The elements of the array are `1 4 3 2 6 5`. After reversing the array, the first element goes to the last position, the second element goes to the second-last position, and so on. Hence, the answer is `[5, 6, 2, 3, 4, 1]`.

**Input:**  
`arr = [4, 5, 2]`  
**Output:**  
`[2, 5, 4]`

**Explanation:**  
The elements of the array are `4 5 2`. The reversed array will be `[2, 5, 4]`.

**Input:**  
`arr = [1]`  
**Output:**  
`[1]`

**Explanation:**  
The array has only a single element, hence the reversed array is the same as the original.

### Constraints:
- $`1 <= arr.size() <= 10^5`$
- $`0 <= arr[i] <= 10^5`$

## 🎯 **My Approach:**

1. **Reversal Process:**
   - The main idea is to reverse the array in-place by swapping elements from both ends.
   - We initialize two pointers: `left` at the beginning of the array and `right` at the end.
   - We swap `arr[left]` and `arr[right]`, then move `left` forward and `right` backward until they cross each other.
   - This process effectively reverses the array.

2. **Alternative Approaches:**
   - **XOR Swap Method:** You can swap elements using XOR to avoid a temporary variable.
   - **Using List Reverse:** In some languages, you can simply call the reverse function on the array.

## 🕒 **Time and Auxiliary Space Complexity**📝

- **Expected Time Complexity:** O(n), where `n` is the number of elements in the array. We perform one pass through the array, swapping elements in place.
- **Expected Auxiliary Space Complexity:** O(1), as we only use a constant amount of additional space to track the left and right pointers.

## 📝 **Solution Code**
## Code (Python)

```python
class Solution:
    def reverseArray(self, arr):
        arr.reverse()
```
