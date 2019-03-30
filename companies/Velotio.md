Questions
==

#### 1st Round - Logical Sudocode Type Questions
- Fibbonacci
    ```python
      def fibo(n):
        a, b = 0, 1
        while a <= n:
          print(a)
          a, b = b, a+b
    ```
- Find the second highest number
    ```python
      from sys import maxsize
      def secondHighest(li):
        first, second = -maxsize-1, -maxsize-1
        for i in li:
          if i > first:
            second = first
            first = i
          elif first > i > second:
            second = i

        if second == -maxsize-1:
          print("No second hightest number available")
        else:
          print(f"Second highest number is {second}")
    ```
- Anagram
    ```python
      def anagram(s, ss):
        if sorted(s) == sorted(ss):
          return True
        return False
    ```
- Given array of player's scores find how many times he broke his own record.
    ```python
      def recordsBroken(arr):
        record, count = arr[0], 0
        for r in set(arr):
          if r > record:
            record = r
            count += 1
        return count
    ```
- Check if two binary trees are equal
  ```python
    sameTree(tree1, tree2)
      1. If both trees are empty then return 1.
      2. Else If both trees are non -empty
           (a) Check data of the root nodes (tree1->data ==  tree2->data)
           (b) Check left subtrees recursively  i.e., call sameTree( 
                tree1->left_subtree, tree2->left_subtree)
           (c) Check right subtrees recursively  i.e., call sameTree( 
                tree1->right_subtree, tree2->right_subtree)
           (d) If a,b and c are true then return 1.
      3. Else return 0 (one is empty and other is not)
  ```
  Please find code at [this link](https://www.geeksforgeeks.org/write-c-code-to-determine-if-two-trees-are-identical/)
- Find longest prefix from array / Find the longest prefix from the list of strings - trie based solution
    - [solution 1](https://www.geeksforgeeks.org/longest-common-prefix-using-word-by-word-matching/)
    - [solution 2](https://www.geeksforgeeks.org/longest-common-prefix-using-binary-search/)
- Find nearest palindrome of a given number
- Given two arrays with different sums find numbers that can be swapped from arrays so as to make the sum equal
- Implement two stacks in a single array
- Get all unique elements from an array
- Check if expression consists of correct parenthesis
- Find if a small array is sub-array of the larger one
- Find the length of array without using len() function


#### 2nd & 3rd Round - Mostly review of previous questions. Can ask similar questions to slove on spot.
- How would you implement the tar program in python? 
- Design facebook database
- Multiply an integer which has max of -255 to 255 range. After multiplication, the result must be in the range itself.
- Write a pagination class for a search engine.
- What are mutable and immutable data types in Python
- Design an algorithm to implement the solution for the Sudoku problem.
- Implement your ordered dictionary without using dict() in python

