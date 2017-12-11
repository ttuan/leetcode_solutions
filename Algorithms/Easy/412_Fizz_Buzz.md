# Question

https://leetcode.com/problems/fizz-buzz/description/

Write a program that outputs the string representation of numbers from 1 to n.

But for multiples of three it should output “Fizz” instead of the number and for the multiples of five output “Buzz”. For numbers which are multiples of both three and five output “FizzBuzz”.

Example:

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


# Solution

```
# @param {Integer} n
# @return {String[]}
def fizz_buzz(n)
  (1..n).map do |i|
    case
    when i % 15 == 0
      "FizzBuzz"
    when i % 3 == 0
      "Fizz"
    when i % 5 == 0
      "Buzz"
    else
      i.to_s
    end
  end
end

```
