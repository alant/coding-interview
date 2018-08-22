# todo
## BFS
### [图上的BFS 判断一个图是否是一棵树](http://www.lintcode.com/problem/graph-valid-tree/)
### [矩阵上的BFS Lintcode Build Post Office II (Hard)](http://www.lintcode.com/problem/build-post-office-ii/)
### [Lintcode 892. Alien Dictionary (Hard)](https://www.lintcode.com/problem/alien-dictionary/description)
### [Binary Tree Level Order Traversal II](http://www.lintcode.com/en/problem/binary-tree-level-order-traversal-ii/)
### [Binary Tree Zigzag Order Traversal](http://www.lintcode.com/en/problem/binary-tree-zigzag-level-order-traversal/)
### [Convert Binary Tree to Linked Lists by Depth](http://www.lintcode.com/en/problem/convert-binary-tree-to-linked-lists-by-depth/)
### [Lintcode 7. Serialize and Deserialize Binary Tree (Medium)](https://www.lintcode.com/problem/serialize-and-deserialize-binary-tree/description)
```html
Design an algorithm and write code to serialize and deserialize a binary tree. Writing the tree to a file is called 'serialization' and reading back from the file to reconstruct the exact same binary tree is 'deserialization'.

There is no limit of how you deserialize or serialize a binary tree, LintCode will take your output of serialize as the input of deserialize, it won't check the result of serialize.

Example
An example of testdata: Binary tree {3,9,20,#,#,15,7}, denote the following structure:

  3
 / \
9  20
  /  \
 15   7
Our data serialization use bfs traversal. This is just for when you got wrong answer and want to debug the input.

You can use other method to do serializaiton and deserialization.
```
思路：BFS 来 serialize, 有坑， 先放 todo
```python
"""
Definition of TreeNode:
class TreeNode:
    def __init__(self, val):
        self.val = val
        self.left, self.right = None, None
"""


class Solution:
    """
    @param root: An object of TreeNode, denote the root of the binary tree.
    This method will be invoked first, you should design your own algorithm
    to serialize a binary tree which denote by a root node to a string which
    can be easily deserialized by your own "deserialize" method later.
    """
    def serialize(self, root):
        # write your code here
        if root == None:
            return "{}"

    """
    @param data: A string serialized by your serialize method.
    This method will be invoked second, the argument data is what exactly
    you serialized at method "serialize", that means the data is not given by
    system, it's given by your own serialize method. So the format of data is
    designed by yourself, and deserialize it here as you serialize it in
    "serialize" method.
    """
    def deserialize(self, data):
        # write your code here
```    
## Two pointers
### [Lintcode Sort Colors II (medium)](https://www.lintcode.com/problem/sort-colors-ii/description)
有难度，解法用的是桶排序，需要理解下， 有空的话还有： 烙饼排序 Pancake Sort， 睡眠排序 Sleep Sort， 面条排序 Spaghetti Sort， 猴子排序 Bogo Sort
### [Partition Array by Odd and Even](http://www.lintcode.com/problem/partition-array-by-odd-and-even/)
### [Interleaving Positive and Negative Numbers](http://www.lintcode.com/problem/interleaving-positive-and-negative-numbers/)
### [Sort Letters by Case](http://www.lintcode.com/problem/sort-letters-by-case/)
### [18. 4Sum (Medium)](https://leetcode.com/problems/4sum/description/)
### [658. Find K Closest Elements (Medium)](https://leetcode.com/problems/find-k-closest-elements/description/)
```html
Given a sorted array, two integers k and x, find the k closest elements to x in the array. The result should also be sorted in ascending order. If there is a tie, the smaller elements are always preferred.

Example 1:
Input: [1,2,3,4,5], k=4, x=3
Output: [1,2,3,4]
Example 2:
Input: [1,2,3,4,5], k=4, x=-1
Output: [1,2,3,4]
Note:
The value k is positive and will always be smaller than the length of the sorted array.
Length of the given array is positive and will not exceed 104
Absolute value of elements in the array and x will not exceed 104
UPDATE (2017/9/19):
The arr parameter had been changed to an array of integers (instead of a list of integers). Please reload the code definition to get the latest changes.
```

### [409. Longest Palindrome (Easy)](https://leetcode.com/problems/longest-palindrome/description/)
```html
Given a string which consists of lowercase or uppercase letters, find the length of the longest palindromes that can be built with those letters.

This is case sensitive, for example "Aa" is not considered a palindrome here.

Note:
Assume the length of given string will not exceed 1,010.

Example:

Input:
"abccccdd"

Output:
7

Explanation:
One longest palindrome that can be built is "dccaccd", whose length is 7.
```

基于中心点枚举法 Enumeration
基于动态规划 Dynamic Programming

### [Implement strStr](http://www.lintcode.com/problem/strstr/)
```html
Description
For a given source string and a target string, you should output the first index(from 0) of target string in source string.

If target does not exist in source, just return -1.

Have you met this question in a real interview?  
Clarification
Do I need to implement KMP Algorithm in a real interview?

Not necessary. When you meet this problem in a real interview, the interviewer may just want to test your basic implementation ability. But make sure you confirm with the interviewer first.
Example
If source = "source" and target = "target", return -1.

If source = "abcdabcdefg" and target = "bcd", return 1.

Challenge
O(n2) is acceptable. Can you implement an O(n) algorithm? (hint: KMP)
```
[240. Search a 2D Matrix II (Medium)](https://leetcode.com/problems/search-a-2d-matrix-ii/description/)
[Lintcode Search a 2D Matrix II](http://www.lintcode.com/en/problem/search-a-2d-matrix-ii/)

### [600. Smallest Rectangle Enclosing Black Pixels (Hard)](https://www.lintcode.com/problem/smallest-rectangle-enclosing-black-pixels/description)
```html
An image is represented by a binary matrix with 0 as a white pixel and 1 as a black pixel. The black pixels are connected, i.e., there is only one black region. Pixels are connected horizontally and vertically. Given the location (x, y) of one of the black pixels, return the area of the smallest (axis-aligned) rectangle that encloses all black pixels.

Example
For example, given the following image:

[
  "0010",
  "0110",
  "0100"
]
and x = 0, y = 2,
Return 6.
```
思路：   

### [680. Valid Palindrome II (Easy)](https://leetcode.com/problems/valid-palindrome-ii/description/)
```html
Given a non-empty string s, you may delete at most one character. Judge whether you can make it a palindrome.

Example 1:
Input: "aba"
Output: True
Example 2:
Input: "abca"
Output: True
Explanation: You could delete the character 'c'.
Note:
The string will only contain lowercase characters a-z. The maximum length of the string is 50000.
```
思路：目前网上看到大部分答案都以贪心算法为主， 等看贪心了再刷这题

# Binary Search & LogN Algorithm
比O(n)更优的时间复杂度几乎只能是O(logn)的二分法
二分法模板: start + 1 < end; start + (end - start) / 2; A[mid] ==, <, >; A[start] A[end] ? target

### [704. Binary Search (Easy)](https://leetcode.com/problems/binary-search/description/)
[lintcode's version](https://www.lintcode.com/problem/classical-binary-search/description)
```html
Find any position of a target number in a sorted array. Return -1 if target does not exist.

Example
Given [1, 2, 2, 4, 5, 5].

For target = 2, return 1 or 2.

For target = 5, return 4 or 5.

For target = 6, return -1.

Challenge
O(logn) time
```
```python
class Solution:
    """
    @param: nums: An integer array sorted in ascending order
    @param: target: An integer
    @return: An integer
    """
    def findPosition(self, nums, target):
        # write your code here
        if (len(nums) == 0):
          return -1
        start, end = 0, len(nums) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2     
            if (nums[mid] == target):
                return mid
            elif (nums[mid] < target):
                start = mid
            else:
                end = mid    
        if (nums[start] == target):
            return start
        if (nums[end] == target):
            return end
        return -1

```
总结：背好模板，lintcode 的 test case 包含空输入数组，需要 python3 的 // 整除运算符才能过

### [Lintcode 14. First Position of Target (Easy)](https://www.lintcode.com/problem/first-position-of-target/description)
```html
Description
For a given sorted array (ascending order) and a target number, find the first index of this number in O(log n) time complexity.

If the target number does not exist in the array, return -1.

Have you met this question in a real interview?  
Example
If the array is [1, 2, 3, 3, 4, 5, 10], for given target 3, return 2.

Challenge
If the count of numbers is bigger than 2^32, can your code work properly?
```
思路：找到了不要 return，扔掉大的一半，继续找
```python
class Solution:
    """
    @param nums: The integer array.
    @param target: Target to find.
    @return: The first position of target. Position starts from 0.
    """
    def binarySearch(self, nums, target):
        # write your code here
        if (len(nums) == 0):
            return -1
        start, end = 0, len(nums) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (nums[mid] >= target):
                end = mid
            else:
                start = mid
        if (nums[start] == target):
            return start
        if (nums[end] == target):
            return end
        return -1
```
总结：背好模板，模板 v5

### [278. First Bad Version (Easy)](https://leetcode.com/problems/first-bad-version/description/)
```html
You are a product manager and currently leading a team to develop a new product. Unfortunately, the latest version of your product fails the quality check. Since each version is developed based on the previous version, all the versions after a bad version are also bad.

Suppose you have n versions [1, 2, ..., n] and you want to find out the first bad one, which causes all the following ones to be bad.

You are given an API bool isBadVersion(version) which will return whether version is bad. Implement a function to find the first bad version. You should minimize the number of calls to the API.

Example:

Given n = 5, and version = 4 is the first bad version.

call isBadVersion(3) -> false
call isBadVersion(5) -> true
call isBadVersion(4) -> true

Then 4 is the first bad version.
```
思路：前面 first position of target 的变体，可以不做

```python
# The isBadVersion API is already defined for you.
# @param version, an integer
# @return a bool
# def isBadVersion(version):

class Solution(object):
    def firstBadVersion(self, n):
        """
        :type n: int
        :rtype: int
        """
        start, end = 0, n
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (isBadVersion(mid)):
                end = mid
            else:
                start = mid
        if (isBadVersion(start)):
            return start
        if (isBadVersion(end)):
            return end
        return -1
```
总结：可不做

### [Lintcode 460. Find K Closest Elements (Medium)](https://www.lintcode.com/problem/find-k-closest-elements/description)
```html
Given a target number, a non-negative integer k and an integer array A sorted in ascending order, find the k closest numbers to target in A, sorted in ascending order by the difference between the number and target. Otherwise, sorted in ascending order by number if the difference is same.

Example
Given A = [1, 2, 3], target = 2 and k = 3, return [2, 1, 3].

Given A = [1, 4, 6, 8], target = 3 and k = 3, return [4, 1, 6].

Challenge
O(logn + k) time complexity.

Notice
The value k is a non-negative integer and will always be smaller than the length of the sorted array.
Length of the given array is positive and will not exceed 10^4
Absolute value of elements in the array and x will not exceed 10^4
```
思路：二分查找找到 start end 以后，用两个判断条件来限制取值范围。当 left 超过取值范围之后，只取 right 以后的数。
当 right 超过取值范围之后，只取 left 之前的数

```python
class Solution:
    """
    @param A: an integer array
    @param target: An integer
    @param k: An integer
    @return: an integer array
    """
    def kClosestNumbers(self, A, target, k):
        # write your code here
        start, end = 0, len(A) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (A[mid] < target):
                start = mid
            else:
                end = mid
        left, right = start, end
        result = []
        while (k > 0):
            if (left >= 0 and right <= len(A) - 1):
                if (target - A[left] <= A[right] - target):
                    result.append(A[left])
                    left -= 1
                else:
                    result.append(A[right])
                    right += 1
            elif (left < 0):
                result.append(A[right])
                right += 1
            else:
                result.append(A[left])
                left -= 1
            k -=  1
        return result

```
总结，一开始没有充分理解题目，题目说的是 k closest elements to x in the array， 找到离 x 最近的点以后要往两边看 k 次。解题方法多少有点需要背的因素。

### [153. Find Minimum in Rotated Sorted Array (Medium)](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/description/)
```html
Suppose an array sorted in ascending order is rotated at some pivot unknown to you beforehand.

(i.e.,  [0,1,2,4,5,6,7] might become  [4,5,6,7,0,1,2]).

Find the minimum element.

You may assume no duplicate exists in the array.

Example 1:
Input: [3,4,5,1,2]
Output: 1

Example 2:
Input: [4,5,6,7,0,1,2]
Output: 0
```
思路：找 pivot，pivot > 0 时返回 nums[pivot + 1]。找 pivot 时,如果 mid < start, 扔 end， 如果 mid > start 扔 start
```python
class Solution:
    def findMin(self, nums):
        """
        :type nums: List[int]
        :rtype: int
        """
        if (nums[0] < nums[len(nums) - 1]):
            return nums[0]
        start, end = 0, len(nums) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (nums[mid] < nums[start]):
                end = mid
            else:
                start = mid
        return nums[end]
```
总结：应改为 Easy 难度的题。
Follow up: 如果有重复的数? 无法保证在 Log(N) 的时间复杂度内解决 例子:[1,1,1,1,1....,1] 里藏着一个 0.最坏情况下需要把每个位置上的1都看一遍，才能找到最后一个有0 的位置. 考点:能想到这个最坏情况的例子

### [Lintcode 585. Maximum Number in Mountain Sequence (Medium)](https://www.lintcode.com/problem/maximum-number-in-mountain-sequence/description)
[852. Peak Index in a Mountain Array](https://leetcode.com/problems/peak-index-in-a-mountain-array/description/)
```html
Given a mountain sequence of n integers which increase firstly and then decrease, find the mountain top.
Example
Given nums = [1, 2, 4, 8, 6, 3] return 8
Given nums = [10, 9, 8, 7], return 10
```
思路：一开始以为跟上题一样，返回 start 就行了，也许是不值得做的题，可是没有考虑到后面不是递增而是递减。所以，需要改算法为切一刀，判断递增就扔左边，递减就扔右边， 不然就找到了中点
```python
class Solution:
    """
    @param nums: a mountain sequence which increase firstly and then decrease
    @return: then mountain top
    """
    def mountainSequence(self, nums):
        # write your code here
        start, end = 0, len(nums) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (nums[mid - 1] < nums[mid] < nums[mid + 1]):
                start = mid
            elif (nums[mid - 1] > nums[mid] > nums[mid + 1]):
                end = mid
            else:
                return nums[mid]
        return nums[end] if nums[start] < nums[end] else nums[start]
```

### [74. Search a 2D Matrix (Medium)](https://leetcode.com/problems/search-a-2d-matrix/description/)
```html
Write an efficient algorithm that searches for a value in an m x n matrix. This matrix has the following properties:

Integers in each row are sorted from left to right.
The first integer of each row is greater than the last integer of the previous row.
Example 1:

Input:
matrix = [
  [1,   3,  5,  7],
  [10, 11, 16, 20],
  [23, 30, 34, 50]
]
target = 3
Output: true
Example 2:

Input:
matrix = [
  [1,   3,  5,  7],
  [10, 11, 16, 20],
  [23, 30, 34, 50]
]
target = 13
Output: false
```
思路：二分查找，不过是放到二维数组里了
```python
class Solution:
    def searchMatrix(self, matrix, target):
        """
        :type matrix: List[List[int]]
        :type target: int
        :rtype: bool
        """
        if len(matrix) == 0:
            return False
        if len(matrix[0]) == 0:
            return False
        startR, endR = 0, len(matrix) - 1
        startC, endC = 0, len(matrix[0]) - 1
        while(startR + 1 < endR):
            midR = startR + (endR - startR) // 2
            if (matrix[midR][0] == target):
                return True
            elif (matrix[midR][0] < target):
                startR = midR
            else:
                endR = midR
        if (matrix[startR][0] == target or matrix[endR][0] == target):
            return True
        elif (matrix[endR][0] < target):
            targetR = endR
        else:
            targetR = startR
        while(startC + 1 < endC):
            midC = startC + (endC - startC) // 2
            if (matrix[targetR][midC] == target):
                return True
            elif (matrix[targetR][midC] < target):
                startC = midC
            else:
                endC = midC
        if (matrix[targetR][startC] == target or matrix[targetR][endC] == target):
            return True
        return False
```
总结：注意检查空输入

### [Lintcode 61. Search for a Range (Medium)](https://www.lintcode.com/problem/search-for-a-range/description)
```html
Given a sorted array of n integers, find the starting and ending position of a given target value.

If the target is not found in the array, return [-1, -1].

Example
Given [5, 7, 7, 8, 8, 10] and target value 8,
return [3, 4].

Challenge
O(log n) time.
```
思路：找一个数的第一次和最后一次出现的 index
```python
class Solution:
    """
    @param A: an integer sorted array
    @param target: an integer to be inserted
    @return: a list of length 2, [index1, index2]
    """
    def searchRange(self, A, target):
        # write your code here
        firstO, lastO = -1, -1
        if len(A) == 0:
            return [firstO, lastO]
        start, end = 0, len(A) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (A[mid] < target):
                start = mid
            else:
                end = mid
        if (A[end] == target):
            firstO = end        
        if (A[start] == target):
            firstO = start
        start, end = 0, len(A) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (A[mid] <= target):
                start = mid
            else:
                end = mid
        if (A[start] == target):
            lastO = start
        if (A[end] == target):
            lastO = end
        return [firstO, lastO]
```
总结：注意检查空输入！

### [162. Find Peak Element (Medium)](https://leetcode.com/problems/find-peak-element/description/)
```html
A peak element is an element that is greater than its neighbors.

Given an input array nums, where nums[i] ≠ nums[i+1], find a peak element and return its index.

The array may contain multiple peaks, in that case return the index to any one of the peaks is fine.

You may imagine that nums[-1] = nums[n] = -∞.

Example 1:

Input: nums = [1,2,3,1]
Output: 2
Explanation: 3 is a peak element and your function should return the index number 2.
Example 2:

Input: nums = [1,2,1,3,5,6,4]
Output: 1 or 5
Explanation: Your function can return either index number 1 where the peak element is 2,
             or index number 5 where the peak element is 6.
Note:

Your solution should be in logarithmic complexity.
```
思路：和前面 Lintcode 585. Maximum Number in Mountain Sequence 应该是一个路子
```python
class Solution:
    def findPeakElement(self, nums):
        """
        :type nums: List[int]
        :rtype: int
        """
        if (len(nums) == 0):
            return -1
        start, end = 0, len(nums) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if (nums[mid - 1] < nums[mid] < nums[mid + 1]):
                start = mid
            elif (nums[mid - 1] < nums[mid] > nums[mid + 1]):
                return mid
            else:
                end = mid
        if nums[start] > nums[end]:
            return start
        else:
            return end
```
总结：确实和前面一样， 不用做

### [33. Search in Rotated Sorted Array (Medium)](https://leetcode.com/problems/search-in-rotated-sorted-array/description/)
```html
Suppose an array sorted in ascending order is rotated at some pivot unknown to you beforehand.

(i.e., [0,1,2,4,5,6,7] might become [4,5,6,7,0,1,2]).

You are given a target value to search. If found in the array return its index, otherwise return -1.

You may assume no duplicate exists in the array.

Your algorithm's runtime complexity must be in the order of O(log n).

Example 1:

Input: nums = [4,5,6,7,0,1,2], target = 0
Output: 4
Example 2:

Input: nums = [4,5,6,7,0,1,2], target = 3
Output: -1
```
思路：第一感觉是得知道 pivot 在哪，有 pivot 一侧不能随便扔，但是更优的方法是查单调的侧是否可以扔
```python
class Solution:
    def search(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: int
        """
        if len(nums) == 0:
            return -1
        start, end = 0, len(nums) - 1
        while (start + 1 < end):
            mid = start + (end - start) // 2
            if nums[start] < nums[mid]:
                if nums[start] <= target <= nums[mid]:
                    end = mid
                else:
                    start = mid
            else:
                if nums[mid] <= target <= nums[end]:
                    start = mid
                else:
                    end = mid
        if nums[start] == target:
            return start
        if nums[end] == target:
            return end
        return -1    
```
总结： 注意 [1, 3, 5] target 为 1 这种边界条件， 判断 target 在单调这边需要加等号

### [Lintcode 140. Fast Power (Medium)](https://www.lintcode.com/problem/fast-power/description)
```html
Calculate the a**n % b where a, b and n are all 32bit integers.

Example
For 2**31 % 3 = 2

For 100**1000 % 1000 = 0

Challenge
O(logn)
```
思路：第一感觉是：需要用某种数学方法，取模只取决于这个数取模后剩下的数加多少次，可以将次方换成乘法，再取模，乘法可以换算成 n 次幂取模 b 再乘 a。
总结：递归版本： (a * b) % p = (a % p * b % p) % p 将 a^n % b 分解为 (a^(n/2) * a^(n/2) * (a)) %b = ((a^(n/2) * a^(n/2))%b * (a)%b) %b = ((a^(n/2)%b * a^(n/2)%b)%b * (a)%b) %b； 非递归版本，思路是转换为二进制

### [50. Pow(x, n) (Medium)](https://leetcode.com/problems/powx-n/description/)
```html
Implement pow(x, n), which calculates x raised to the power n (xn).

Example 1:

Input: 2.00000, 10
Output: 1024.00000
Example 2:

Input: 2.10000, 3
Output: 9.26100
Example 3:

Input: 2.00000, -2
Output: 0.25000
Explanation: 2-2 = 1/22 = 1/4 = 0.25
Note:

-100.0 < x < 100.0
n is a 32-bit signed integer, within the range [−231, 231 − 1]
```
思路：递归
```python
class Solution:
    def myPow(self, x, n):
        """
        :type x: float
        :type n: int
        :rtype: float
        """
        if n < 0:
            return 1 / self.power(x, -n)
        else:
            return self.power(x, n)
    def power(self, x, n):    
        if n == 0:
            return 1
        result = self.power(x, n // 2)
        if n % 2 == 0:
            return result * result
        else:
            return x * result * result
```
总结：有固定写法套路的题目， 不值得做。
# Two pointers
## 预热
### [26. Remove Duplicates from Sorted Array (Easy)](https://leetcode.com/problems/remove-duplicates-from-sorted-array/description/)
```html
Given a sorted array nums, remove the duplicates in-place such that each element appear only once and return the new length.

Do not allocate extra space for another array, you must do this by modifying the input array in-place with O(1) extra memory.

Example 1:

Given nums = [1,1,2],

Your function should return length = 2, with the first two elements of nums being 1 and 2 respectively.

It doesn't matter what you leave beyond the returned length.
Example 2:

Given nums = [0,0,1,1,1,2,2,3,3,4],

Your function should return length = 5, with the first five elements of nums being modified to 0, 1, 2, 3, and 4 respectively.

It doesn't matter what values are set beyond the returned length.
Clarification:

Confused why the returned value is an integer but your answer is an array?

Note that the input array is passed in by reference, which means modification to the input array will be known to the caller as well.

Internally you can think of this:

// nums is passed in by reference. (i.e., without making a copy)
int len = removeDuplicates(nums);

// any modification to nums in your function would be known by the caller.
// using the length returned by your function, it prints the first len elements.
for (int i = 0; i < len; i++) {
    print(nums[i]);
}
```
思路：简单题， 慢指针只有在快指针碰到不同的值才走。
```python
class Solution:
    def removeDuplicates(self, nums):
        """
        :type nums: List[int]
        :rtype: int
        """
        if len(nums) == 0:
            return 0
        slow, fast = 0, 1
        while fast < len(nums):
            if nums[fast] == nums[slow]:
                fast += 1
            else:
                slow += 1
                nums[slow] = nums[fast]
                fast += 1
        return slow + 1
```
总结：纯热身，秒解
### [160. Intersection of Two Linked Lists (Easy)](https://leetcode.com/problems/intersection-of-two-linked-lists/description/)
```html
Write a program to find the node at which the intersection of two singly linked lists begins.

For example, the following two linked lists:

A:          a1 → a2
                   ↘
                     c1 → c2 → c3
                   ↗            
B:     b1 → b2 → b3
begin to intersect at node c1.

Notes:
If the two linked lists have no intersection at all, return null.
The linked lists must retain their original structure after the function returns.
You may assume there are no cycles anywhere in the entire linked structure.
Your code should preferably run in O(n) time and use only O(1) memory.
```
思路：统计两条链走到头的长度，lenA 和 lenB, 然后让长的那条先走两者的差值，然后一起走，返回相遇的那点

```python
# Definition for singly-linked list.
# class ListNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.next = None

class Solution(object):
    def getIntersectionNode(self, headA, headB):
        """
        :type head1, head1: ListNode
        :rtype: ListNode
        """
        savedHeadA, savedHeadB = headA, headB
        if headA == None or headB == None:
            return None
        lenA, lenB = 1, 1
        while headA.next != None:
            headA = headA.next
            lenA += 1
        while headB.next != None:
            headB = headB.next
            lenB += 1
        if lenA > lenB:
            diff = lenA - lenB
            for x in xrange(diff):
                savedHeadA = savedHeadA.next
        else:
            diff = lenB - lenA
            for x in xrange(diff):
                savedHeadB = savedHeadB.next
        while savedHeadA != None:
            if savedHeadA == savedHeadB:
                return savedHeadA
            else:
                savedHeadA = savedHeadA.next
                savedHeadB = savedHeadB.next
        return None
```
总结：1.注意空输入（不能假设 headA 或 B 有 next）2.注意 headA headB 是一个节点 i.e. 合体的情况
### [141. Linked List Cycle (Easy)](https://leetcode.com/problems/linked-list-cycle/description/)
```html
Given a linked list, determine if it has a cycle in it.

Follow up:
Can you solve it without using extra space?
```
思路：记得应该是慢的 +1 快的 +2 如果有 loop 会重逢。。。可能不那么值得做，热身吧
```python
# Definition for singly-linked list.
# class ListNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.next = None

class Solution(object):
    def hasCycle(self, head):
        """
        :type head: ListNode
        :rtype: bool
        """
        if head == None or head.next == None:
            return False
        slow, fast = head, head.next.next
        while fast != None and fast.next != None and fast.next.next != None:
            if slow == fast:
                return True
            slow = slow.next
            fast = fast.next.next
        return False
```
总结：有点意思，适合热身，代码写好后要测的情况比较多， 1 -> 2 无 loop，1 -> 2 -> 3 -> 4 loop 回 2 这些情况都要测一下。防止 next 和 next.next 不存在的情况
### [142. Linked List Cycle II (Medium)](https://leetcode.com/problems/linked-list-cycle-ii/description/)
```html
Given a linked list, return the node where the cycle begins. If there is no cycle, return null.

Note: Do not modify the linked list.

Follow up:
Can you solve it without using extra space?
```
思路：记得好像是找到有 loop 以后走多久能找到 cycle 的起点。
```python
# Definition for singly-linked list.
# class ListNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.next = None

class Solution(object):
    def detectCycle(self, head):
        """
        :type head: ListNode
        :rtype: ListNode
        """
        if head == None or head.next == None:
            return None
        slow, fast = head, head
        while fast.next != None and fast.next.next != None:
            slow = slow.next
            fast = fast.next.next            
            if slow == fast:
                while head != slow:
                    head = head.next
                    slow = slow.next
                return head
        return None
```        
总结：slow fast 同时在 head，先走再判断。不然容易出错。有数学关系，面试当场不一定能推导出来。就算推导出来也要注意前面的 slow，fast写法。
    a            b
A ------ B --------+
         |         |
       c |         |
         +-------- C

* A: 起始点
* B: Cycle Begins
* C: 1st 快慢指针相遇点

* A->B: a
* B->C: b
* C->B: c
* 环的长度 (b+c) 为 R

第一次相遇时，慢指针所走步数为 a + b 快指针走的步数为 *a + b + nR*
我们知道快指针是慢指针速度的2倍，因此 2(a + b) = a + b + nR 那么 a + b = nR
同时 b + c = R 所以 a = (n - 1)R + c;
也就是说，从A点和C点同时出发，以相同的速度前进，相遇的位置将是B。
## 题目
### [283. Move Zeroes (Easy)](https://leetcode.com/problems/move-zeroes/description/)
```html
Given an array nums, write a function to move all 0's to the end of it while maintaining the relative order of the non-zero elements.

Example:

Input: [0,1,0,3,12]
Output: [1,3,12,0,0]
Note:

You must do this in-place without making a copy of the array.
Minimize the total number of operations.
```
思路：第一感觉是快指针直接跑到最后， 慢指针遇到 0 就接快指针面；仔细读题才发现是数组 in place 转换；那就快指针到第一个非 0 的数，直到快指针到最后
```python
class Solution(object):
    def moveZeroes(self, nums):
        """
        :type nums: List[int]
        :rtype: void Do not return anything, modify nums in-place instead.
        """
        if len(nums) == 0 or len(nums) == 1:
            return
        slow, fast = 0, 0
        while fast < len(nums) and nums[fast] == 0:
            fast += 1
        while slow < len(nums) - 1 and fast < len(nums):
            if nums[slow] == 0:
                nums[slow], nums[fast] = nums[fast], nums[slow]
                while fast < len(nums) and nums[fast] == 0:
                    fast += 1
            slow += 1
            if slow > fast:
                fast += 1
                while fast < len(nums) and nums[fast] == 0:
                    fast += 1
```
总结：思路简单，但是情况很多， 需要考虑，无 0， 0 在前， 后， 中四种情况 [1,2], [0, 1, 2], [1, 0, 0], [1, 0, 0, 1] 才能写对

### [125. Valid Palindrome (Easy)](https://leetcode.com/problems/valid-palindrome/description/)
```html
Given a string, determine if it is a palindrome, considering only alphanumeric characters and ignoring cases.

Note: For the purpose of this problem, we define empty string as valid palindrome.

Example 1:

Input: "A man, a plan, a canal: Panama"
Output: true
Example 2:

Input: "race a car"
Output: false
```
思路：头尾双指针， 碰头了返回 True，相同继续走，不同返回 False
```python
class Solution(object):
    def isPalindrome(self, s):
        """
        :type s: str
        :rtype: bool
        """
        if len(s) == 0 or len(s) == 1:
            return True
        head, tail = 0, len(s) - 1
        while head < tail:
            while not s[head].isalnum() and head < tail:
                head += 1
            while not s[tail].isalnum() and head < tail:
                tail -= 1
            if s[head].lower() != s[tail].lower():
                return False
            else:
                head += 1
                tail -= 1
        return True
```
总结：思路简单， 但是要想到的 case 很多。考虑带标点符号，连续两个位置都是标点符号，整个字符串都是标点符合这三个情况才能写对

### [1. Two Sum (Easy)](https://leetcode.com/problems/two-sum/description/)
```html

Given an array of integers, return indices of the two numbers such that they add up to a specific target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

Example:

Given nums = [2, 7, 11, 15], target = 9,

Because nums[0] + nums[1] = 2 + 7 = 9,
return [0, 1].
```
思路：固定一个找另一个
```python
class Solution:
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        for index1 in xrange(len(nums)):
            for index2 in xrange(index1 + 1, len(nums)):
                if nums[index1] + nums[index2] == target:
                    return [index1, index2]
```
总结： 第二层循环的起始数字注意条件 you may not use the same element twice

### [167. Two Sum II - Input array is sorted (Easy)](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/description/)
```html
Given an array of integers that is already sorted in ascending order, find two numbers such that they add up to a specific target number.

The function twoSum should return indices of the two numbers such that they add up to the target, where index1 must be less than index2.

Note:

Your returned answers (both index1 and index2) are not zero-based.
You may assume that each input would have exactly one solution and you may not use the same element twice.
Example:

Input: numbers = [2,7,11,15], target = 9
Output: [1,2]
Explanation: The sum of 2 and 7 is 9. Therefore index1 = 1, index2 = 2.
```
思路：增加了 sorted 这个条件， 第一感觉是可以折半查找了。固定 index1，index2 用折半查找获得
```python
class Solution:
    def twoSum(self, numbers, target):
        """
        :type numbers: List[int]
        :type target: int
        :rtype: List[int]
        """
        for index1 in range(len(numbers)):
            start, end = index1 + 1, len(numbers) - 1
            while start + 1 < end:
                mid = start + (end - start) // 2
                if numbers[index1] + numbers[mid] == target:
                    return [index1 + 1, mid + 1]
                elif numbers[index1] + numbers[mid] < target:
                    start = mid + 1
                else:
                    end = mid - 1
            if numbers[index1] + numbers[start] == target:
                return [index1 + 1, start + 1]
            elif numbers[index1] + numbers[end] == target:
                return [index1 + 1, end + 1]
```
总结：要细心。1.题中 answers are not zero-based 2.要测两个情况 [2, 7, 19], 9 和 [5, 25, 75] 可以测出代码的问题

### [Lintcode 607. Two Sum III - Data structure design (Easy)](https://www.lintcode.com/problem/two-sum-iii-data-structure-design/description)
```html
Design and implement a TwoSum class. It should support the following operations: add and find.

add - Add the number to an internal data structure.
find - Find if there exists any pair of numbers which sum is equal to the value.

Example
add(1); add(3); add(5);
find(4) // return true
find(7) // return false
```
思路：add 的时候把 sum 都存 dict 里面， 查的时候直接返回 dict 里面有没有 sum. 会超时。
```python
class TwoSum:
    keys = {}
    """
    @param: number: An integer
    @return: nothing
    """
    def add(self, number):
        # write your code here
        if number not in self.keys:
            self.keys[number] = 1
        else:
            self.keys[number] = 2
    """
    @param: value: An integer
    @return: Find if there exists any pair of numbers which sum is equal to the value.
    """
    def find(self, value):
        # write your code here
        for key in self.keys:
            if value - key in self.keys:
                if value - key == key:
                    if self.keys[key] == 2:
                        return True
                else:
                    return True
        return False
```
总结：虽然是一道容易题， 第一反应的思路会超时。 需要在 find 的时候判断能凑出答案的另一个 key 是不是已经在 keys 里了。而不是先存好 sum。 还要判断两个数相同的时候有没有存过两个数。

### [15. 3Sum (Medium)](https://leetcode.com/problems/3sum/description/)
```html
Given an array nums of n integers, are there elements a, b, c in nums such that a + b + c = 0? Find all unique triplets in the array which gives the sum of zero.

Note:

The solution set must not contain duplicate triplets.

Example:

Given array nums = [-1, 0, 1, 2, -1, -4],

A solution set is:
[
  [-1, 0, 1],
  [-1, -1, 2]
]
```
思路：可以吧 a + b + c = 0 变为 a + b = - c 的问题，问题则变为， 对于任意数 a，dict 里是否存在 -c - a 这么个数， a 和 c 是两层循环
```python
class Solution:
    def threeSum(self, nums):
        """
        :type nums: List[int]
        :rtype: List[List[int]]
        """
        results = []
        nums.sort()
        for index1 in range(len(nums) - 2):
            if index1 and nums[index1] == nums[index1 - 1]:
                continue
            head = index1 + 1
            tail = len(nums) - 1
            while head < tail:
                if nums[index1] + nums[head] > -nums[tail]:
                    tail -= 1
                elif nums[index1] + nums[head] < -nums[tail]:
                    head += 1
                else:
                    results.append([nums[index1], nums[head], nums[tail]])
                    head += 1
                    tail -= 1
                    while head < tail and nums[head] == nums[head - 1]:
                        head += 1
                    while head < tail and nums[tail] == nums[tail + 1]:
                        tail -= 1
        return results
```
总结：三层循环是暴力方法，去重会受阻，这个时候需要想到给输入数组先排个序，因为结果里，没有要求元素的顺序，这是个重要的提示。排序以后每次固定一个数 index1，然后找的过程是：while head < tail: head = index1 + 1, tail = len(nums) - 1, if nums[index1] + nums[head] > - nums[tail]: tail -= 1, elif nums[index1] + nums[head] < -nums[tail]: head += 1, else: results.append()
代码还需要考虑的几个情况：1.对于已经用过的元素需要跳过， 这里要用到 if index1 and nums[index1] == nums[index1 - 1]; 2.如果碰到了一个 result，要跳过所有重复的元素，需要用到 while head < tail and nums[head] == nums[head - 1]: 和相应的 ...nums[tail + 1]

### [Lintcode 382. Triangle Count (Medium)](https://www.lintcode.com/problem/triangle-count/description)
```html
Given an array of integers, how many three numbers can be found in the array, so that we can build an triangle whose three edges length is the three numbers that we find?

Example
Given array S = [3,4,6,7], return 3. They are:

[3,4,6]
[3,6,7]
[4,6,7]
Given array S = [4,4,4,4], return 4. They are:

[4(1),4(2),4(3)]
[4(1),4(2),4(4)]
[4(1),4(3),4(4)]
[4(2),4(3),4(4)]
```
思路： 判断能不能做三角形以后全排列
```python
class Solution:
    """
    @param S: A list of integers
    @return: An integer
    """
    def triangleCount(self, S):
        # write your code here
        S.sort(reverse=True)
        sum = 0
        for index1, longest in enumerate(S):
            head, tail = index1 + 1, index1 + 2
            while tail < len(S) and S[head] + S[tail] > longest:
                tail += 1
            tail -= 1
            while head < tail:
                sum += tail - head
                head += 1
                while head < tail and S[head] + S[tail] <= longest:
                    tail -= 1
        return sum
```
总结：看清题目，问的是有多少个这样的三角形， 返回数就行。 全排列效率比较低。 更优解是每次定下最长边， 寻找符合条件的另外两个边的数量。 双指针的解法是将 tail 推到最小不能组成三角形的位置， 退一步， 然后从 tail 到 head 的位置的都可以组， 因为他们相加只会比最长边更长。 然后将 head 进一步（缩短），tail 边加长到大于最长边的位置，新 tail 到 head 的位置又都可以组。

### [16. 3Sum Closest (Medium)](https://leetcode.com/problems/3sum-closest/description/)
```html
Given an array nums of n integers and an integer target, find three integers in nums such that the sum is closest to target. Return the sum of the three integers. You may assume that each input would have exactly one solution.

Example:

Given array nums = [-1, 2, 1, -4], and target = 1.

The sum that is closest to the target is 2. (-1 + 2 + 1 = 2).
```
思路：3sum 的思路是先排序，固定一个点以后，开始用双指针搜索符合条件的数。closest 感觉已经是 4sum，需要记 delta，然后往 delata 小的方向走。
```python
class Solution:
    def threeSumClosest(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: int
        """
        ans = None
        nums.sort()
        for index1, val in enumerate(nums):
            head = index1 + 1
            tail = len(nums) - 1
            while head < tail:
                sum = nums[index1] + nums[head] + nums[tail]
                if ans == None or abs(target - sum) < abs(target - ans):
                    ans = sum
                if sum < target:
                    head += 1
                elif sum > target:
                    tail -= 1
                else:
                    return target
        return ans
```
总结：比 3sum 省事的是不需要优化跳过重复的元素也可以过。pyhton 可以用 None 就不用想 Java 那样吧 ans 初始化为 MAX_VALUE 了
### [86. Partition List (Medium)](https://leetcode.com/problems/partition-list/description/)
```html
Given a linked list and a value x, partition it such that all nodes less than x come before nodes greater than or equal to x.

You should preserve the original relative order of the nodes in each of the two partitions.

Example:

Input: head = 1->4->3->2->5->2, x = 3
Output: 1->2->2->4->3->5
```
思路：慢快指针，慢指针在最后一个 < x 的位置， 快指针在最后一个 >= x 的位置，快指针碰到一个 < x 的就和慢指针换
```python
# Definition for singly-linked list.
# class ListNode:
#     def __init__(self, x):
#         self.val = x
#         self.next = None

class Solution:
    def partition(self, head, x):
        """
        :type head: ListNode
        :type x: int
        :rtype: ListNode
        """
        if head == None or head.next == None:
            return head
        fakie = ListNode(-1)
        fakie.next = head
        slow, fast = fakie, None
        while slow != None:
            while slow != None and slow.next != None and slow.next.val < x:
                slow = slow.next
            if fast == None:
                fast = slow
            while fast != None and fast.next != None and fast.next.val >= x:
                fast = fast.next
            if fast.next == None or slow.next == None:
                break
            savedFastNext = fast.next
            fast.next = fast.next.next
            savedSlowNext = slow.next
            slow.next = savedFastNext
            savedFastNext.next = savedSlowNext
            slow = slow.next
        return fakie.next
```
总结：链表的问题需要先放一个假头，注意 1->1 x = 0, 1->1 x = 2, 2->1 x = 2 这三种情况和题中的例子情况 1->4->3->2->5->2 才能写对。

### [Lintcode 31. Partition Array (Medium)](https://www.lintcode.com/problem/partition-array/description)
```html
Description
Given an array nums of integers and an int k, partition the array (i.e move the elements in "nums") such that:

All elements < k are moved to the left
All elements >= k are moved to the right
Return the partitioning index, i.e the first index i nums[i] >= k.

You should do really partition in array nums instead of just counting the numbers of integers smaller than k.

If all elements in nums are smaller than k, then return nums.length
Example
If nums = [3,2,2,1] and k=2, a valid answer is 1.

Challenge
Can you partition the array in-place and in O(n)?
```
思路：和 partition list 很像， 数组的话就只能用双指针了. l 是最后一个 < k, r 是最后一个 >= k
```python
class Solution:
    """
    @param nums: The integer array you should partition
    @param k: An integer
    @return: The index after partition
    """
    def partitionArray(self, nums, k):
        # write your code here
        if len(nums) == 0:
            return 0
        l, r = 0, len(nums) - 1
        while l <= r:
            while l < len(nums) and nums[l] < k:
                l += 1
            while r >= 0 and nums[r] >= k:
                r -= 1
            if l > r:
                break
            nums[l], nums[r] = nums[r], nums[l]
        return l    
```
总结：因为数组比链表好操作的多， 比 partition list 解法简单， 需要注意：1。while 的条件是 l <= r 2。l 往右走，r 往左走不要越界，r 往左需要 r >= 0 3.l > r 的时候需要 break

### [215. Kth Largest Element in an Array (Medium)](https://leetcode.com/problems/kth-largest-element-in-an-array/description/)
```html
Find the kth largest element in an unsorted array. Note that it is the kth largest element in the sorted order, not the kth distinct element.

Example 1:
Input: [3,2,1,5,6,4] and k = 2
Output: 5

Example 2:
Input: [3,2,3,1,2,4,5,5,6] and k = 4
Output: 4
Note:
You may assume k is always valid, 1 ≤ k ≤ array's length.
```
思路：应该是不去排序的基础上找到第 K 大的数。现场想是基本没戏的。网上答案：quickselect 算法，基于 quicksort. 1.选第一个数为 pivot 2.比 pivot 大的放左边， 不然右边 3.如果 pivot 是第 k, 返回该值， 大于 k 扔掉右边， 否则扔掉左边
```python
class Solution:
    def findKthLargest(self, nums, k):
        """
        :type nums: List[int]
        :type k: int
        :rtype: int
        """
        k -= 1
        def quickSelect(s, e):
            l, r = s + 1, e
            while l <= r:
                if nums[l] > nums[s]:
                    l += 1
                else:
                    nums[l], nums[r] = nums[r], nums[l]
                    r -= 1
            nums[s], nums[r] = nums[r], nums[s]
            if r == k:
                return nums[r]
            elif r > k:
                return quickSelect(s, r - 1)
            else:
                return quickSelect(r + 1, e)
        return quickSelect(0, len(nums) - 1)
```
总结：要背 pivot 的部分，如果第一个数是 pivot，那么走一遍，碰到比他大的不动，小的塞右边，l <= r 走完把 pivot 和 r 值互换，r 左边就是大于 pivot 数的子数组. 注意：递归调用的时候记得函数名前要加 return 否则不会返回任何值。由于完全抛弃另一侧，时间复杂度平均由 quick sort 的 O(nlogn) 降为 O(n) 因为输入变小了， quicksort 的输入一直是 n, 最差情况 O(n^2)

### [75. Sort Colors (Medium)](https://leetcode.com/problems/sort-colors/description/)
```html
Given an array with n objects colored red, white or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white and blue.

Here, we will use the integers 0, 1, and 2 to represent the color red, white, and blue respectively.

Note: You are not suppose to use the library's sort function for this problem.

Example:

Input: [2,0,2,1,1,0]
Output: [0,0,1,1,2,2]
Follow up:

A rather straight forward solution is a two-pass algorithm using counting sort.
First, iterate the array counting number of 0's, 1's, and 2's, then overwrite array with total number of 0's, then 1's and followed by 2's.
Could you come up with a one-pass algorithm using only constant space?
```
思路：因为只有 3 种颜色，1 pass 就是设好 l, r 两个指针，分别代表颜色的边界，碰到不属于边界的就往正确的边界内交换
```python
class Solution:
    def sortColors(self, nums):
        """
        :type nums: List[int]
        :rtype: void Do not return anything, modify nums in-place instead.
        """
        if len(nums) == 0 or len(nums) == 1:
            return
        index, l, r = 0, 0, len(nums) - 1
        while l < r and index <= r:
            while nums[l] == 0 and l < r:
                l += 1
            while nums[r] == 2 and l < r:
                r -= 1
            if l > index:
                index = l
            if nums[index] == 0:
                nums[l], nums[index] = nums[index], nums[l]
            if nums[index] == 1:
                index += 1
                continue
            if nums[index] == 2:
                nums[index], nums[r] = nums[r], nums[index]
```
总结：counting sort：数一下每个元素有多少个，一次给写到结果里; 这种写法基本上秒出 :)，想当年傻逼呵呵的这种简单题都面试的时候挂掉，哎。。。如今得换种 1 pass 高级点的；一开始想的思路有个问题，就是如果只有两个指针，两个指针都指 1， 中间夹一大堆 2 就没办法了。 改成三指针， l, r 维持边界，index 从 l 走到 r; 要一次写对得注意：1.当 l 大于 index 的时候， index 要追上来 2.整个循环的终止条件需要 l < r and index <= r, 不然过不了 [2, 0, 1] (index <= r), [0, 0], [1, 1] (l < r) 这两个情况

# BFS
图的遍历 Traversal in Graph
* 层级遍历 Level Order Traversal
* 由点及面 Connected Component
* 拓扑排序 Topological Sorting
最短路径 Shortest Path in Simple Graph
* 仅限简单图求最短路径
* 即，图中每条边长度都是1，或者边长都相等
### [102. Binary Tree Level Order Traversal (Medium)](https://leetcode.com/problems/binary-tree-level-order-traversal/description/)
```html
Given a binary tree, return the level order traversal of its nodes' values. (ie, from left to right, level by level).

For example:
Given binary tree [3,9,20,null,null,15,7],
    3
   / \
  9  20
    /  \
   15   7
return its level order traversal as:
[
  [3],
  [9,20],
  [15,7]
]
```
思路：热身阶段，先看答案
```python
# Definition for a binary tree node.
# class TreeNode:
#     def __init__(self, x):
#         self.val = x
#         self.left = None
#         self.right = None

class Solution:
    def levelOrder(self, root):
        """
        :type root: TreeNode
        :rtype: List[List[int]]
        """
        ans = []
        if root == None:
            return ans
        q = [root]
        while q:
            new_q = []
            temp = []
            for node in q:
                temp.append(node.val)
                if node.left:
                    new_q.append(node.left)
                if node.right:
                    new_q.append(node.right)
            ans.append(temp)
            q = new_q
        return ans
```
总结：看来答案还是很简单的，注意只需要处理 root 为空，记得返回 ans

### [133. Clone Graph (Medium)](https://leetcode.com/problems/clone-graph/description/)
```html
Clone an undirected graph. Each node in the graph contains a label and a list of its neighbors.


OJ's undirected graph serialization:
Nodes are labeled uniquely.

We use # as a separator for each node, and , as a separator for node label and each neighbor of the node.
As an example, consider the serialized graph {0,1,2#1,2#2,2}.

The graph has a total of three nodes, and therefore contains three parts as separated by #.

First node is labeled as 0. Connect node 0 to both nodes 1 and 2.
Second node is labeled as 1. Connect node 1 to node 2.
Third node is labeled as 2. Connect node 2 to node 2 (itself), thus forming a self-cycle.
Visually, the graph looks like the following:

       1
      / \
     /   \
    0 --- 2
         / \
         \_/
```
思路：BFS, 用一个 dict 存当前节点的邻居，如果没见过就加 dict 存 queue，queue 出来建 node，放 neighbor；概念上比较好懂，写码可能有坑
```python
# Definition for a undirected graph node
# class UndirectedGraphNode:
#     def __init__(self, x):
#         self.label = x
#         self.neighbors = []

class Solution:
    # @param node, a undirected graph node
    # @return a undirected graph node
    def cloneGraph(self, node):
        if node == None:
            return None
        dict = {}
        _cloneNode = UndirectedGraphNode(node.label)
        dict[node] = _cloneNode
        q = [node]
        while q:
            new_q = []
            for _node in q:
                for neighbor in _node.neighbors:
                    if neighbor not in dict:
                        _cloneNode = UndirectedGraphNode(neighbor.label)
                        dict[neighbor] = _cloneNode
                        new_q.append(neighbor)
                    dict[_node].neighbors.append(dict[neighbor])    
            q = new_q
        return dict[node]
```
总结：思路用 dict 来存当前节点的邻居是错的，需要用 dict 存当前节点和克隆节点的映射关系。因为反正映射关系在，加邻居可以后加. 邻居是不能直接 copy 或者 = 的， 因为邻居的类型也是节点， 需要创造以后加进去。测一下，然后 debug 细一点， 要测出
```python
dict[_node].neighbors.append(dict[neighbor])
```
### [127. Word Ladder (Medium)](https://leetcode.com/problems/word-ladder/description/)
```html
Given two words (beginWord and endWord), and a dictionary's word list, find the length of shortest transformation sequence from beginWord to endWord, such that:

Only one letter can be changed at a time.
Each transformed word must exist in the word list. Note that beginWord is not a transformed word.
Note:

Return 0 if there is no such transformation sequence.
All words have the same length.
All words contain only lowercase alphabetic characters.
You may assume no duplicates in the word list.
You may assume beginWord and endWord are non-empty and are not the same.
Example 1:

Input:
beginWord = "hit",
endWord = "cog",
wordList = ["hot","dot","dog","lot","log","cog"]

Output: 5

Explanation: As one shortest transformation is "hit" -> "hot" -> "dot" -> "dog" -> "cog",
return its length 5.
Example 2:

Input:
beginWord = "hit"
endWord = "cog"
wordList = ["hot","dot","dog","lot","log"]

Output: 0

Explanation: The endWord "cog" is not in wordList, therefore no possible transformation.
```
思路：确实是寻找路径的问题，从 beginWord 到 endWord 是否存在最短路径让他俩相连，最短路径取决于词库里有哪些词（路径）。怎么实现很不清晰
```python
import string
class Solution(object):
    def ladderLength(self, beginWord, endWord, wordList):
        """
        :type beginWord: str
        :type endWord: str
        :type wordList: List[str]
        :rtype: int
        """
        if beginWord == endWord:
            return 0
        wordSet = set(wordList)
        q = collections.deque([[beginWord, 1]])
        while q:
            word, level = q.popleft()
            for index in range(len(word)):
                for char in 'abcdefghijklmnopqrstuvwxyz':
                    newWord = word[:index] + char + word[index + 1:]
                    if newWord in wordSet:
                        if newWord == endWord:
                            return level + 1
                        wordSet.remove(newWord)
                        q.append([newWord, level + 1])
        return 0

```
总结：看了下答案，网上答案解释的比较好理解的是，起始词是树的根节点，每一层是从第一个字母到最后一个字母，每次一个字母，从 a - z 替换过一遍，同时又在 wordList 里的词。从上往下 BFS，找到 endWord 即返回当前 level。啧啧啧，强大的应用题。逻辑对还得不 TLE 需要1.将 wordList 转成 set；2.使用 collections.deque；3.碰到 wordSet 中的词，先该词在 wordSet 中删除，再入 deque

### [200. Number of Islands (Medium)](https://leetcode.com/problems/number-of-islands/description/)
```html
Given a 2d grid map of '1's (land) and '0's (water), count the number of islands. An island is surrounded by water and is formed by connecting adjacent lands horizontally or vertically. You may assume all four edges of the grid are all surrounded by water.

Example 1:
Input:
11110
11010
11000
00000
Output: 1

Example 2:
Input:
11000
11000
00100
00011
Output: 3
```
思路：遍历矩阵，碰到 1 就上下左右 BFS，碰到 0 跳过。BFS 访问过的标 0
```python
class Solution(object):
    def numIslands(self, grid):
        """
        :type grid: List[List[str]]
        :rtype: int
        """
        if len(grid) == 0:
            return 0
        ans = 0
        for rowI in range(len(grid)):
            for colI in range(len(grid[0])):
                if grid[rowI][colI] == "1":
                    ans += 1
                    q = collections.deque([[rowI, colI]])
                    grid[rowI][colI] = "0"
                    while q:
                        row, col = q.popleft()
                        # up
                        if (row > 0) and grid[row - 1][col] == "1":
                                q.append([row - 1, col])
                                grid[row - 1][col] = '0'
                        # down
                        if (row < len(grid) - 1) and grid[row + 1][col] == "1":
                                q.append([row + 1, col])
                                grid[row + 1][col] = '0'
                        # left
                        if (col > 0) and grid[row][col - 1] == "1":
                                q.append([row, col - 1])
                                grid[row][col - 1] = '0'
                        # right
                        if (col < len(grid[0]) - 1) and grid[row][col + 1] == "1":
                                q.append([row, col + 1])
                                grid[row][col + 1] = '0'
        return ans
```
总结：对于 leetcode ac 比较重要的细节是，gird[][] = '0' 这句话要在 while 的每个 if 里面，否则逻辑 OK 但是会 TLE

### [Lintcode 611. Knight Shortest Path (Medium)](https://www.lintcode.com/problem/knight-shortest-path/description)
```html
Given a knight in a chessboard (a binary matrix with 0 as empty and 1 as barrier) with a source position, find the shortest path to a destination position, return the length of the route.
Return -1 if knight can not reached.

source and destination must be empty.
Knight can not enter the barrier.

Clarification
If the knight is at (x, y), he can get to the following positions in one step:

(x + 1, y + 2)
(x + 1, y - 2)
(x - 1, y + 2)
(x - 1, y - 2)
(x + 2, y + 1)
(x + 2, y - 1)
(x - 2, y + 1)
(x - 2, y - 1)
Example
[[0,0,0],
 [0,0,0],
 [0,0,0]]
source = [2, 0] destination = [2, 2] return 2

[[0,1,0],
 [0,0,0],
 [0,0,0]]
source = [2, 0] destination = [2, 2] return 6

[[0,1,0],
 [0,0,1],
 [0,0,0]]
source = [2, 0] destination = [2, 2] return -1
```
思路：没什么思路， 看了下答案，就是 BFS 硬来，需要检查走了某个方向以后是不是还是在棋盘内
```python
"""
Definition for a point.
class Point:
    def __init__(self, a=0, b=0):
        self.x = a
        self.y = b
"""

class Solution:
    """
    @param grid: a chessboard included 0 (false) and 1 (true)
    @param source: a point
    @param destination: a point
    @return: the shortest path
    """
    def shortestPath(self, grid, source, destination):
        # write your code here
        if len(grid) == 0 or (len(grid[0]) == 1 and grid[0][0] == 1):
            return -1
        ans = 0
        dx = [1, 1, -1, -1, 2, 2, -2, -2]
        dy = [2, -2, 2, -2, 1, -1, 1, -1]
        q = collections.deque([source])
        grid[source.x][source.y] = 1
        while q:
            qlen = len(q)
            next_q = collections.deque()
            for i in range(qlen):
                pt = q.popleft()
                if pt.x == destination.x and pt.y == destination.y:
                    return ans
                for move in range(len(dx)):
                    nextPt = Point(pt.x + dx[move], pt.y + dy[move])
                    if (self.isInbound(grid, nextPt) and grid[nextPt.x][nextPt.y] == 0):
                        next_q.append(nextPt)
                        grid[nextPt.x][nextPt.y] = 1
            ans += 1
            q = next_q
        return -1
    def isInbound(self, grid, pt):
        return pt.x >= 0 and pt.x < len(grid) and pt.y >= 0 and pt.y < len(grid[0])
```
总结：注意 isInbound 要查的是 >=0 和 < len()， 其他的问题可以通过跑一个测试数据发现

## Topological sorting 拓扑排序

### [Lintcode 127. Topological Sorting (Medium)](https://www.lintcode.com/problem/topological-sorting/description)
```html
Given an directed graph, a topological order of the graph nodes is defined as follow:

For each directed edge A -> B in graph, A must before B in the order list.
The first node in the order can be any node in the graph with no nodes direct to it.
Find any topological order for the given graph.

You can assume that there is at least one topological order in the graph.

Clarification
[Learn more about representation of graphs](http://www.lintcode.com/help/graph)

Example
For graph as follow:
```
![graph example](images/lintcode_127_topo_1.jpeg)
```html
The topological order can be:
[0, 1, 2, 3, 4, 5]
[0, 2, 3, 1, 5, 4]
```
思路：拓扑排序，算法貌似是：1.统计每个点的入度；2.将入度为 0 的点入 queue；3.从队列中 pop 点，去掉所有指向别的点的边: 相应点入度 -1；4.新入度为 0 的点入 queue
```python
"""
Definition for a Directed graph node
class DirectedGraphNode:
    def __init__(self, x):
        self.label = x
        self.neighbors = []
"""


class Solution:
    """
    @param: graph: A list of Directed graph node
    @return: Any topological order for the given graph.
    """
    def topSort(self, graph):
        # write your code here
        if len(graph) == 0:
            return []
        ans = []
        inBound = {}
        for node in graph:
            if node not in inBound:
                inBound[node] = 0
            for neighbor in node.neighbors:
                if neighbor not in inBound:
                    inBound[neighbor] = 0
                inBound[neighbor] += 1
        q = collections.deque()
        for node in inBound:
            if inBound[node] == 0:
                q.append(node)
        while q:
            zNode = q.popleft()
            ans.append(zNode)
            for node in zNode.neighbors:
                inBound[node] -= 1
                if inBound[node] == 0:
                    q.append(node)
        return ans
```            
总结：顺利。但是题目没有说清楚 return 的是一个拓扑排序好的 node 的 list

### [207. Course Schedule (Medium)](https://leetcode.com/problems/course-schedule/description/)
```html
There are a total of n courses you have to take, labeled from 0 to n-1.

Some courses may have prerequisites, for example to take course 0 you have to first take course 1, which is expressed as a pair: [0,1]

Given the total number of courses and a list of prerequisite pairs, is it possible for you to finish all courses?

Example 1:

Input: 2, [[1,0]]
Output: true
Explanation: There are a total of 2 courses to take.
             To take course 1 you should have finished course 0. So it is possible.
Example 2:

Input: 2, [[1,0],[0,1]]
Output: false
Explanation: There are a total of 2 courses to take.
             To take course 1 you should have finished course 0, and to take course 0 you should
             also have finished course 1. So it is impossible.
Note:

The input prerequisites is a graph represented by a list of edges, not adjacency matrices. Read more about how a graph is represented.
You may assume that there are no duplicate edges in the input prerequisites.
```
思路：其实是问拓扑顺序存不存在，具体实现得看答案
```python
class Solution(object):
    def canFinish(self, numCourses, prerequisites):
        """
        :type numCourses: int
        :type prerequisites: List[List[int]]
        :rtype: bool
        """
        if len(prerequisites) == 0 or len(prerequisites[0]) == 0 or len(prerequisites[0]) == 1:
            return True
        graph = {}
        inBound = {}
        for prereqs in prerequisites:
            for index, course in enumerate(prereqs):
                if course not in graph:
                    graph[course] = []
                if course not in inBound:
                    inBound[course] = 0
                if index < len(prereqs) - 1:
                    graph[course].append(prereqs[index + 1])
                if index > 0:
                    inBound[course] += 1
        q = collections.deque()
        for key in inBound:
            if inBound[key] == 0:
                q.append(key)
        while q:
            course = q.popleft()
            for neighbor in graph[course]:
                inBound[neighbor] -= 1
                if inBound[neighbor] == 0:
                    q.append(neighbor)
        for key in inBound:
            if inBound[key] > 0:
                return False
        return True      
```
总结：有向图有环则拓扑顺序不存在，题可以变为如何检测有向图有环的问题。算法的核心是计算所有节点的入度，然后做类似上题的 BFS，每遍历一次邻居，入度减一，如果遍历完以后还有点的入度 > 0，则图有环。具体实现两个 dict，一个存节点和邻居们， 一个存节点和入度， 再加个 queue; 注意下 prerequisites 是个 list of list 别的没什么

### [210. Course Schedule II (Medium)](https://leetcode.com/problems/course-schedule-ii/description/)
```html
There are a total of n courses you have to take, labeled from 0 to n-1.

Some courses may have prerequisites, for example to take course 0 you have to first take course 1, which is expressed as a pair: [0,1]

Given the total number of courses and a list of prerequisite pairs, return the ordering of courses you should take to finish all courses.

There may be multiple correct orders, you just need to return one of them. If it is impossible to finish all courses, return an empty array.

Example 1:
Input: 2, [[1,0]]
Output: [0,1]
Explanation: There are a total of 2 courses to take. To take course 1 you should have finished   
             course 0. So the correct course order is [0,1] .

Example 2:
Input: 4, [[1,0],[2,0],[3,1],[3,2]]
Output: [0,1,2,3] or [0,2,1,3]
Explanation: There are a total of 4 courses to take. To take course 3 you should have finished both     
             courses 1 and 2. Both courses 1 and 2 should be taken after you finished course 0.
             So one correct course order is [0,1,2,3]. Another correct ordering is [0,2,1,3] .
Note:

The input prerequisites is a graph represented by a list of edges, not adjacency matrices. Read more about how a graph is represented.
You may assume that there are no duplicate edges in the input prerequisites.
```
思路：是前两道题的延伸，既要计算所有节点的入度， BFS，又要做拓扑排序，记下拓扑的顺序。 如果结束时还有入度 > 0 的节点，则图有环，无解
```python
class Solution(object):
    def findOrder(self, numCourses, prerequisites):
        """
        :type numCourses: int
        :type prerequisites: List[List[int]]
        :rtype: List[int]
        """
        ans = []
        if len(prerequisites) == 0 or len(prerequisites[0]) == 0:
            for i in range(numCourses):
                ans.append(i)
            return ans[::-1]
        graph = {}
        inBound = {}
        for prereqs in prerequisites:
            for index, course in enumerate(prereqs):
                if course not in graph:
                    graph[course] = []
                if course not in inBound:
                    inBound[course] = 0
                if index < len(prereqs) - 1:
                    graph[course].append(prereqs[index + 1])
                if index > 0:
                    inBound[course] += 1
        q = collections.deque()
        for course in inBound:
            if inBound[course] == 0:
                ans.append(course)
                q.append(course)
        while q:
            course = q.popleft()
            for neighbor in graph[course]:
                inBound[neighbor] -= 1
                if inBound[neighbor] == 0:
                    ans.append(neighbor)
                    q.append(neighbor)
        for course in inBound:
            if inBound[course] > 0:
                return []
        for i in range(numCourses):
            if i not in inBound:
                ans.append(i)
        return ans[::-1]
```
总结：值得做的题的边缘，要满足些很琐碎的细节才能 AC，和 Course Schedule 题不同点在于这题需要用 numCourses。如果有些节点在 prerequisites 里不出现的话，需要在答案里加进去

### [Lintcode 605. Sequence Reconstruction (Medium)](https://www.lintcode.com/problem/sequence-reconstruction/description)
```html
Check whether the original sequence org can be uniquely reconstructed from the sequences in seqs. The org sequence is a permutation of the integers from 1 to n, with 1 ≤ n ≤ 10^4. Reconstruction means building a shortest common supersequence of the sequences in seqs (i.e., a shortest sequence so that all sequences in seqs are subsequences of it). Determine whether there is only one sequence that can be reconstructed from seqs and it is the org sequence.

Example
Given org = [1,2,3], seqs = [[1,2],[1,3]]
Return false
Explanation:
[1,2,3] is not the only one sequence that can be reconstructed, because [1,3,2] is also a valid sequence that can be reconstructed.

Given org = [1,2,3], seqs = [[1,2]]
Return false
Explanation:
The reconstructed sequence can only be [1,2].

Given org = [1,2,3], seqs = [[1,2],[1,3],[2,3]]
Return true
Explanation:
The sequences [1,2], [1,3], and [2,3] can uniquely reconstruct the original sequence [1,2,3].

Given org = [4,1,5,2,6,3], seqs = [[5,2,6,3],[4,1,5,2]]
Return true
```
思路：没什么思路，被考点吸引，如何构建图，如何拓扑排序.
```python
class Solution:
    """
    @param org: a permutation of the integers from 1 to n
    @param seqs: a list of sequences
    @return: true if it can be reconstructed only one or false
    """
    def sequenceReconstruction(self, org, seqs):
        # write your code here
        if len(seqs) == 0 and len(org) == 0:
            return True
        if len(seqs) == 0 and len(org) != 0:
            return False
        if len(seqs) != 0 and len(org) == 0:
            return False
        graph = {}
        indegree = {}
        for seq in seqs:
            if len(seq) > len(org):
                return False
            for val in seq:
                if val not in graph:
                    graph[val] = []
                if val not in
```
总结：看了网上答案，记录入度，记录邻居，拓扑排序拓扑排序出来要有唯一解（q 每次长度都是 1）和 org 的相应位置的值要相等结束才能返回 True。写了一半实在是不想写了。 回头在写吧。todo item

#  Binary Tree & Tree-based DFS 二叉树与树上的深度优先搜索
考察形态:二叉树上求值，求路径 代表例题:http://www.lintcode.com/problem/subtree-with-maximum-average/ 考点本质:深度优先搜索(Depth First Search)
考察形态:二叉树结构变化 代表例题:http://www.lintcode.com/problem/invert-binary-tree/ 考点本质:深度优先搜索(Depth First Search)
考察形态:二叉查找树(Binary Search Tree) 代表例题:http://www.lintcode.com/problem/validate-binary-search-tree/ 考点本质:深度优先搜索(Depth First Search)

### [257. Binary Tree Paths (Easy)](https://leetcode.com/problems/binary-tree-paths/description/)
```html
Given a binary tree, return all root-to-leaf paths.

Note: A leaf is a node with no children.

Example:

Input:

   1
 /   \
2     3
 \
  5

Output: ["1->2->5", "1->3"]

Explanation: All root-to-leaf paths are: 1->2->5, 1->3
```
思路：既然是 DFS 环节，看着就是 DFS 的解法。实现应该有坑
```python
# Definition for a binary tree node.
# class TreeNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.left = None
#         self.right = None

class Solution(object):
    def binaryTreePaths(self, root):
        """
        :type root: TreeNode
        :rtype: List[str]
        """
        ans = []
        if root == None:
            return ans
        self.helper(root, '', ans)
        return ans
    def helper(self, root, cur, ans):
        if root.left == None and root.right == None:
            ans.append(cur + str(root.val))
            return
        if root.left != None:
            self.helper(root.left, cur + str(root.val) + '->', ans)
        if root.right != None:
            self.helper(root.right, cur + str(root.val) + '->', ans)  
```
总结：递归的模板需要记，需要当前答案 cur， 总答案 ans，每次进入递归函数时：1.如果已经到底，将 cur append 上 root.val 并加入到 ans；2.如有左边递归左边，如有右边递归右边。注意 python + string 要先把 int 变成 str

### [236. Lowest Common Ancestor of a Binary Tree (Medium)](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/description/)
```html
Given a binary tree, find the lowest common ancestor (LCA) of two given nodes in the tree.

According to the definition of LCA on Wikipedia: “The lowest common ancestor is defined between two nodes p and q as the lowest node in T that has both p and q as descendants (where we allow a node to be a descendant of itself).”

Given the following binary tree:  root = [3,5,1,6,2,0,8,null,null,7,4]

        _______3______
       /              \
    ___5__          ___1__
   /      \        /      \
   6      _2       0       8
         /  \
         7   4
Example 1:
Input: root = [3,5,1,6,2,0,8,null,null,7,4], p = 5, q = 1
Output: 3
Explanation: The LCA of of nodes 5 and 1 is 3.

Example 2:
Input: root = [3,5,1,6,2,0,8,null,null,7,4], p = 5, q = 4
Output: 5
Explanation: The LCA of nodes 5 and 4 is 5, since a node can be a descendant of itself
             according to the LCA definition.

Note:
All of the nodes' values will be unique.
p and q are different and both values will exist in the binary tree.
```
思路：很久没刷过题了，这题第一感觉是 DFS 回溯，但是没有多的灵感。看答案。
```python
# Definition for a binary tree node.
# class TreeNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.left = None
#         self.right = None

class Solution(object):
    def lowestCommonAncestor(self, root, p, q):
        """
        :type root: TreeNode
        :type p: TreeNode
        :type q: TreeNode
        :rtype: TreeNode
        """
        if root == None or root == p or root == q:
            return root
        l = self.lowestCommonAncestor(root.left, p, q)
        r = self.lowestCommonAncestor(root.right, p, q)
        if (l == p and r == q) or (l == q and r == p):
            return root
        if l != None:
            return l
        if r != None:
            return r
```
总结：答案的算法是 DFS，从叶子节点向上，如果子树中有目标节点，返回目标节点。否则为 None。如果左右子树都有目标节点，则找到 LCA，如果在 p 为跟节点的子树中有 q，则 p 为 LCA 反之亦然。最后为子树返回目标节点非常 tricky，必须要用 l != None。 直觉上更好理解的 l == p or l == q 过不了， 不知道为什么。 已经在[讨论区问了](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-tree/discuss/162142/Can't-tell-the-difference-between-two-versions-of-my-code-one-ac-one-fail)

### [235. Lowest Common Ancestor of a Binary Search Tree (Easy)](https://leetcode.com/problems/lowest-common-ancestor-of-a-binary-search-tree/description/)
思路：跟上题一样，除了多一个 BST 树的条件， 将题变成了一个二分查找的题
```python
# Definition for a binary tree node.
# class TreeNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.left = None
#         self.right = None

class Solution(object):
    def lowestCommonAncestor(self, root, p, q):
        """
        :type root: TreeNode
        :type p: TreeNode
        :type q: TreeNode
        :rtype: TreeNode
        """
        if root == None or root == p or root == q:
            return root
        if root.val > p.val and root.val > q.val:
            return self.lowestCommonAncestor(root.left, p, q)
        elif root.val < p.val and root.val < q.val:
            return self.lowestCommonAncestor(root.right, p, q)
        else:
            return root
```
总结：稍微看一下就行。 不值得刷的题。

### [114. Flatten Binary Tree to Linked List (Medium)](https://leetcode.com/problems/flatten-binary-tree-to-linked-list/description/)
```html
Given a binary tree, flatten it to a linked list in-place.

For example, given the following tree:

    1
   / \
  2   5
 / \   \
3   4   6
The flattened tree should look like:

1
 \
  2
   \
    3
     \
      4
       \
        5
         \
          6
```
思路：看着像典型的 DFS，不知道有什么坑，直接写吧
```python
# Definition for a binary tree node.
# class TreeNode(object):
#     def __init__(self, x):
#         self.val = x
#         self.left = None
#         self.right = None

class Solution(object):
    def flatten(self, root):
        """
        :type root: TreeNode
        :rtype: void Do not return anything, modify root in-place instead.
        """
        if root == None:
            return
        self.flatten(root.left)
        self.flatten(root.right)
        if root.left == None:
            return
        p = root.left
        while p.right:
            p = p.right
        p.right = root.right
        root.right = root.left
        root.left = None                 
```
总结：基本靠套路。1.None 既 return，左右到底， 左边为空既 return 2. 到左边一个，往右到底， 套路：p.right = root.right; root.right = root.left; root.left = null i.e.：将 root 右边接到 p（尾巴上）, root 右节点变为 root 左节点， root 左节点置空
