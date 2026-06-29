# Day 5


Problem 11: Running Sum of 1d Array

Leetcode Link: https://leetcode.com/problems/running-sum-of-1d-array/

Input: ARRAY [INT]

Output: NEW ARRAY [INT] 

Algorithm: Two-sum Method


Javascript Solution:

```js
 INPUT: ARRAY[INT]
 OUTPUT: ARRAY[INT]
 GOAL: While iterating through nums INPUT array continuously add up each new number to the previous count until you have reached the end of the array. 
 ALGORITHM: Sliding-door
 
var runningSum = function(nums) {
    let runCount = [];
    for(let i = 1; i < nums.length; i++){
        nums[i] += nums[i-1] 
        runCount++
    }
    return nums
}; 
```
Python Solution:

```py
 def runningSum(self, nums: List[int]) -> List[int]:
        runCount = []
        for i in range(1, len(nums)):
            nums[i] += nums[i-1]
        return nums
```