# Intuition
The FizzBuzz problem is a classic programming challenge for beginners that tests basic control flow and conditional logic. 
The intuition is to iterate through numbers and apply specific rules based on divisibility.

# Approach
1. Initialize an empty list to store the results.
2. Iterate through numbers from 1 to n.
3. For each number, check if it's divisible by both 3 and 5, then by 3, then by 5.
4. Append the appropriate string based on the divisibility checks.
5. If the number isn't divisible by 3 or 5, append the number itself as a string.
6. Return the resulting list.

# Complexity
- Time complexity:
We iterate through the numbers from 1 to n once, performing constant-time operations for each number.

- Space complexity:
We create a list that stores n elements, where n is the input number.

# Code
```python []
class Solution(object):
    def fizzBuzz(self, n):
        result = []
        for i in range(1, n+1):
            if i % 3 == 0 and i % 5 == 0:
                result.append('FizzBuzz')
            elif i % 3 == 0:
                result.append('Fizz')    
            elif i % 5 == 0:
                result.append('Buzz')  
            else:
                result.append(str(i))   
        return result  
        
     
```
