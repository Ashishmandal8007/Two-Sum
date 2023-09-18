# Two-Sum
##Explanation

class Solution - This line defines a new class called Solution.

public int[] twoSum(int[] nums, int target) - This line defines a public method called twoSum that takes an array of integers and a target value as input and returns an array of integers containing the indices of the two elements in the array that add up to the target value, or null if no such elements exist.

for(int i = 0; i<nums.length; i++){ - This line begins a for loop that iterates over the input array, starting at index 0 and ending at index nums.length - 1.

for(int j = i+1; j<nums.length ; j++){ - This line begins a nested for loop that iterates over the input array, starting at index i + 1 and ending at index nums.length - 1. This ensures that we do not compare the same element to itself twice.

if( nums[i]+nums[j] == target){ - This line checks if the sum of the current element (at index i) and the next element (at index j) is equal to the target value.

int a[] ={i,j}; - If the sum of the two elements is equal to the target value, this line creates a new array containing the indices of the two elements.

return a; - This line returns the array containing the indices of the two elements.

} - This line closes the nested for loop.

} - This line closes the outer for loop.

return null; - If no two elements in the array add up to the target value, the code returns null.

This is a simple and straightforward implementation of the Two Sum algorithm. However, it has a time complexity of O(n^2), which means that it can be slow for large arrays.
