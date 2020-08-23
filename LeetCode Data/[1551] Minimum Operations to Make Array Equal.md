# [1551] Minimum Operations to Make Array Equal (Medium)

[![Math_badge](https://img.shields.io/badge/topic-Math-green.svg)](https://leetcode.com/problems/minimum-operations-to-make-array-equal/) 

[Magic Portal](https://leetcode.com/problems/minimum-operations-to-make-array-equal/)

## My Submission

- Runtime: 44 ms
- Completed time: 2020-08-15 19:49:58

```python3
class Solution:
    def minOperations(self, n: int) -> int:
        L = n//2
        if n % 2 == 1:

            return (2 + 2 * L) * L // 2
        L -= 1
        return (3 + 2 * L + 1) * L // 2 + 1
```

## Content
<p>You have an array <code>arr</code> of length <code>n</code> where <code>arr[i] = (2 * i) + 1</code> for all valid values of <code>i</code> (i.e. <code>0 &lt;= i &lt; n</code>).</p>

<p>In one operation, you can select two indices <code>x</code>&nbsp;and <code>y</code> where <code>0 &lt;= x, y &lt; n</code> and subtract <code>1</code> from <code>arr[x]</code> and add <code>1</code> to <code>arr[y]</code>&nbsp;(i.e. perform <code>arr[x] -=1&nbsp;</code>and <code>arr[y] += 1</code>).&nbsp;The goal is to make all the elements of the array <strong>equal</strong>. It is <strong>guaranteed</strong> that all the elements of the array can be made equal using some operations.</p>

<p>Given an integer <code>n</code>, the length of the array. Return <em>the minimum number of operations</em> needed to make&nbsp;all the elements of arr equal.</p>

<p>&nbsp;</p>
<p><strong>Example 1:</strong></p>

<pre>
<strong>Input:</strong> n = 3
<strong>Output:</strong> 2
<strong>Explanation:</strong> arr = [1, 3, 5]
First operation choose x = 2 and y = 0, this leads arr to be [2, 3, 4]
In the second operation choose x = 2 and y = 0 again, thus arr = [3, 3, 3].
</pre>

<p><strong>Example 2:</strong></p>

<pre>
<strong>Input:</strong> n = 6
<strong>Output:</strong> 9
</pre>

<p>&nbsp;</p>
<p><strong>Constraints:</strong></p>

<ul>
	<li><code>1 &lt;= n &lt;= 10^4</code></li>
</ul>

## Related Problems


## What a(n) Medium problem!
Among **15549** total submissions, **12165** are accepted, with an acceptance rate of 78.2%. <br>

- Likes: 95
- Dislikes: 20
