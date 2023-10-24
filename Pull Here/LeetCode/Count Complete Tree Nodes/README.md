# Count Complete Tree Nodes
## Problem Link: https://leetcode.com/problems/count-complete-tree-nodes/

## Problem:
Given the root of a complete binary tree, return the number of the nodes in the tree.

According to Wikipedia, every level, except possibly the last, is completely filled in a complete binary tree, and all nodes in the last level are as far left as possible. It can have between 1 and 2h nodes inclusive at the last level h.

Design an algorithm that runs in less than O(n) time complexity.

## Constraints
The number of nodes in the tree is in the range [0, 5 * 104].
0 <= Node.val <= 5 * 104
The tree is guaranteed to be complete.

## Example 1:
```
Input: root = [1,2,3,4,5,6]
Output: 6

```
## Example 2:
 ```
Input: root = []
Output: 0
```

## Example 3:
```
Input: root = [1]
Output: 1
```

# Template Function : 

- ## C++:
```
class Solution {
public:
    int countNodes(TreeNode* root) {
        
    }
};
```

// Optimized implementation of Bubble sort
#include <bits/stdc++.h>
using namespace std;
 
// An optimized version of Bubble Sort
void bubbleSort(int arr[], int n)
{
    int i, j;
    bool swapped;
    for (i = 0; i < n - 1; i++) {
        swapped = false;
        for (j = 0; j < n - i - 1; j++) {
            if (arr[j] > arr[j + 1]) {
                swap(arr[j], arr[j + 1]);
                swapped = true;
            }
        }
 
        // If no two elements were swapped
        // by inner loop, then break
        if (swapped == false)
            break;
    }
}
 
// Function to print an array
void printArray(int arr[], int size)
{
    int i;
    for (i = 0; i < size; i++)
        cout << " " << arr[i];
}
 
// Driver program to test above functions
int main()
{
    int arr[] = { 64, 34, 25, 12, 22, 11, 90 };
    int N = sizeof(arr) / sizeof(arr[0]);
    bubbleSort(arr, N);
    cout << "Sorted array: \n";
    printArray(arr, N);
    return 0;
}
