# Question

https://leetcode.com/problems/power-of-two/description/

Given an integer, write a function to determine if it is a power of two.

# Solution

```
def is_power_of_two(n)
  return n > 0 && Math.log2(n) % 1 == 0
end
```
