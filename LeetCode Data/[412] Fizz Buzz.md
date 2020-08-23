# [412] Fizz Buzz (Easy)



[Magic Portal](https://leetcode.com/problems/fizz-buzz/)

## My Submission

- Runtime: 44 ms
- Completed time: 2020-07-23 15:53:54

```python3
class Solution:
    def fizzBuzz(self, n: int) -> List[str]:
        ret = []
        for i in range(1, n+1):
            if i % 15 == 0:
                ret.append("FizzBuzz")
            elif i % 5 ==0:
                ret.append("Buzz")
            elif i % 3 ==0:
                ret.append("Fizz")
            else:
                ret.append(str(i))
        return ret
```

## Content
<p>Write a program that outputs the string representation of numbers from 1 to <i>n</i>.</p>

<p>But for multiples of three it should output “Fizz” instead of the number and for the multiples of five output “Buzz”. For numbers which are multiples of both three and five output “FizzBuzz”.</p>

<p><b>Example:</b>
<pre>
n = 15,

Return:
[
    "1",
    "2",
    "Fizz",
    "4",
    "Buzz",
    "Fizz",
    "7",
    "8",
    "Fizz",
    "Buzz",
    "11",
    "Fizz",
    "13",
    "14",
    "FizzBuzz"
]
</pre>
</p>

## Related Problems
[Fizz Buzz Multithreaded](https://leetcode.com/problems/fizz-buzz-multithreaded/) (Medium) <br>

## What a(n) Easy problem!
Among **565625** total submissions, **352600** are accepted, with an acceptance rate of 62.3%. <br>

- Likes: 938
- Dislikes: 1236
