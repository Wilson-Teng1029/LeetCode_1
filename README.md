# LeetCode - Two Sum


Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

***
#### 題目：陣列中哪兩個數字加起來等於target
##### 使用兩個迴圈，將陣列中數字兩兩加起來，如陣列若是[1,2,3,4]
##### 那就是1+2、1+3、1+4，然而這時候1+2已經確認過了，於是到2開始時只需要2+3、2+4
##### 所以第二個迴圈只需要 int someNumber = i+1 作為檢查變數即可
 
***

### Example 1:

**Input:** nums = [2,7,11,15], target = 9

**Output:** [0,1]

**Explanation:** Because nums[0] + nums[1] == 9, we return [0, 1].

### Example 2:

**Input:** nums = [3,2,4], target = 6

**Output:** [1,2]

### Example 3:

**Input:** nums = [3,3], target = 6

**Output:** [0,1]
 
***

## Constraints:

#### 2 <= nums.length <= 104

#### -109 <= nums[i] <= 109

#### -109 <= target <= 109

#### **Only one valid answer exists.**
 
 ***

### ※ Follow-up: Can you come up with an algorithm that is less than O(n2) time complexity?
