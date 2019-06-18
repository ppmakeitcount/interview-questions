Questions
==

### Preparation questions for SDE 1
- Convert sorted array to BST  
  Solution:
   0. Exit condition if arr empty return None
   1. Make mid of array root
   2. Make left of root, mid of left part of array
   3. Make right of root, mid of right part of array
   4. call this recursively at step 2 and 3
   5. return root from recursive function

  ``` python
      class Node:
        def __init__(self, d):
          self.data = d
          self.left = None
          self.right = None
      
      def sortedArrayToBST(arr):
        if not arr:
          return None

        mid = (len(arr)) // 2
        root = Node(arr[mid])
        root.left = sortedArrayToBST([:mid])
        root.right= sortedArrayToBST([mid+1:])
        return root

  ```