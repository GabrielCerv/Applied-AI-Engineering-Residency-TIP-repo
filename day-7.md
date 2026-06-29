# Day 5


Problem 7: Plus One

Leetcode Link:https://leetcode.com/problems/plus-one/ 
``` js 
 function plusOne(digits) {
   for (let i = digits.length - 1; i >= 0; i--) {
     if (digits[i] < 9) {
       digits[i] += 1;
       return digits;
     }
     digits[i] = 0;
   }
   digits.unshift(1);
   return digits;
 }
```
Input:

Output:

Algorithm:


Python Solution:

```py
# solution here
    def plusOne(self, digits: List[int]) -> List[int]:
        for i in range(len(digits) -1, -1, -1):
            if digits[i] < 9:
                digits[i] += 1
                return digits
            digits[i] = 0
        digits.insert(0,1)
        return digits 
```