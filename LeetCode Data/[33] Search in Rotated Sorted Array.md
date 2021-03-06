# [33] Search in Rotated Sorted Array (Medium)

[![Array_badge](https://img.shields.io/badge/topic-Array-green.svg)](https://leetcode.com/problems/search-in-rotated-sorted-array/)  [![Binary%20Search_badge](https://img.shields.io/badge/topic-Binary%20Search-green.svg)](https://leetcode.com/problems/search-in-rotated-sorted-array/) 

:+1: 5517 &nbsp; &nbsp; :thumbsdown: 479

---

## My Submission

- Language: python3
- Runtime: 32 ms
- Completed time: 2020-08-17 18:41:38

```python3
class Solution:
    def search(self, nums: List[int], target: int) -> int:
        i = 0
        j = len(nums) - 1
        
        while i <= j:
            if nums[i] == target:
                return i
            if nums[j] == target:
                return j
            i += 1
            j -= 1
        return -1
```

## Content
<p>Given an integer array <code>nums</code> sorted in ascending order, and an integer <code>target</code>.</p>

<p>Suppose that <code>nums</code> is rotated at some pivot unknown to you beforehand (i.e., <code>[0,1,2,4,5,6,7]</code> might become <code>[4,5,6,7,0,1,2]</code>).</p>

<p>You should search for&nbsp;<code>target</code> in <code>nums</code> and if you found return its index, otherwise return <code>-1</code>.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>
<pre><strong>Input:</strong> nums = [4,5,6,7,0,1,2], target = 0
<strong>Output:</strong> 4
</pre><p><strong>Example 2:</strong></p>
<pre><strong>Input:</strong> nums = [4,5,6,7,0,1,2], target = 3
<strong>Output:</strong> -1
</pre><p><strong>Example 3:</strong></p>
<pre><strong>Input:</strong> nums = [1], target = 0
<strong>Output:</strong> -1
</pre>
<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= nums.length &lt;= 5000</code></li>
	<li><code>-10^4 &lt;= nums[i] &lt;= 10^4</code></li>
	<li>All values of <code>nums</code> are <strong>unique</strong>.</li>
	<li><code>nums</code> is guranteed to be rotated at some pivot.</li>
	<li><code>-10^4 &lt;= target &lt;= 10^4</code></li>
</ul>


## Related Problems
[Search in Rotated Sorted Array II](https://leetcode.com/problems/search-in-rotated-sorted-array-ii/) (Medium) <br>
[Find Minimum in Rotated Sorted Array](https://leetcode.com/problems/find-minimum-in-rotated-sorted-array/) (Medium) <br>

## What a(n) Medium problem!
Among **2231166** total submissions, **772384** are accepted, with an acceptance rate of **34.6%**. <br>

- Likes: 5517
- Dislikes: 479

