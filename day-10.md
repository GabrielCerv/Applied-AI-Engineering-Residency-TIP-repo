# Day 5


Problem 9: Word Pattern

Leetcode Link: https://leetcode.com/problems/word-pattern/description/

Input: STRING

Output: BOOLEAN 

Algorithm: Hash map


Python Solution:

```py
words = s.split()
        
        if len(pattern) != len(words):
            return False
        
        char_to_word = {}
        word_to_char = {}
        
        for char, word in zip(pattern, words):
            if char in char_to_word and char_to_word[char] != word:
                return False
            if word in word_to_char and word_to_char[word] != char:
                return False
            
            char_to_word[char] = word
            word_to_char[word] = char
        
        return True
```