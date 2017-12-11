# Question

https://leetcode.com/problems/power-of-three/description/

Given an integer, write a function to determine if it is a power of three.

Follow up:
Could you do it without using any loop / recursion?

# Solution

Max integer power of three is 1162261467

```
# @param {Integer} n
# @return {Boolean}
def is_power_of_three(n)
  return n > 0 && 1162261467 % n == 0
end

```

