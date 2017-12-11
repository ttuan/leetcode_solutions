# Question

Given a List of words, return the words that can be typed using letters of alphabet on only one row's of American keyboard like the image below.

American keyboard

Example 1:

Input: ["Hello", "Alaska", "Dad", "Peace"]
Output: ["Alaska", "Dad"]

Note:

    You may use one character in the keyboard more than once.
    You may assume the input string will only contain letters of alphabet.

# Solution

```
# @param {String[]} words
# @return {String[]}
def find_words(words)
  rows = ["qwertyuiop", "asdfghjkl", "zxcvbnm"]
  f = ->word, list{word.downcase.chars.all?{|c| list.include?(c)}}
  words.select {|word| f[word, rows[0]] || f[word, rows[1]] || f[word, rows[2]]}
end
```
