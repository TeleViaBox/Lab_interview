##### related knowledge:
- 常用算法：贪心法、字符串处理、递归、BFS、DFS、分治、排序
- 常用数据结构：数组/列表、队列、栈、链表、二叉树、哈希表
##### todo(last renew: 16:52)
36. Valid Sudoku
13. Roman to Integer
283. Move Zeroes
168. Excel Sheet Column Title
021. Merge Two Sorted Lists
344. Reverse String

##### 14. Longest Common Prefix
6
-py
7
-ref: https://zhuanlan.zhihu.com/p/106560131
```
"""
# 横向扫描
    def longestCommonPrefixHorizontalScan(self, strs):
        """
            Runtime: 28ms
            Memory Usage: 12.8MB

        """


        # If null return ""
        if len(strs) == 0:
            return ""

        prefix = strs[0]

        for i in range(1, len(strs)):
            while(strs[i].find(prefix) != 0):
                prefix = prefix[:-1]
                if len(prefix) == 0:
                    return ""

        return prefix
# 纵向扫描
   def longestCommonPrefixVerticalScan(self, strs):
        """
        Time 28 ms	Memory 12.8 MB

        """

        # If null return ""
        if len(strs) == 0:
            return ""

        for i in range(len(strs[0])):
            for j in range(1, len(strs)):
                if i == len(strs[j]) or strs[0][i] != strs[j][i]: # i==len must be put at the front
                    return strs[0][:i]
        return strs[0]
"""
```

##### 13. Roman to Integer
- c++
- STATUS: FAIL
```
class Solution {
public:
    int romanToInt(string s) {
// Input: s = "MCMXCIV"
// Output: 1994
// Explanation: M = 1000, CM = 900, XC = 90 and IV = 4.     
        
// I can be placed before V (5) and X (10) to make 4 and 9. 
// X can be placed before L (50) and C (100) to make 40 and 90. 
// C can be placed before D (500) and M (1000) to make 400 and 900.
        if "IV", "IX", XL, XC, CD, CM
        

    }
};


// //https://leetcode.com/problems/roman-to-integer/
// //20190520
// class Solution {
// public:
//     int romanToInt(string s) {
//         unordered_map<char, int> c = {{'I', 1},{'V', 5},{'X', 10},{'L', 50},{'C', 100},{'D',500},{'M',1000}};
//         int result = 0;
//         for(int i=0;i<s.size();i++){
//             if(i==0||c[s[i]] <= c[s[i - 1]]) 
//                 result += c[s[i]];
//             else
//                 result += c[s[i]]-2*c[s[i-1]];
//         }
//         return result;
//     }
// };
```
##### 283. Move Zeroes:
- related to: "27. Remove Element"
- c++
- STATUS: FAIL
```
class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        // [0,1,0,3,12]
        int idx = 0;
        int i;
        int record[nums.size()]; // = {0};
        for(i = 1; i<nums.size(); i++){
            if(i != 0){
                record[idx] = i;
                idx++;
            }           
        }
        for(i = idx; i<nums.size(); i++){
            record[idx] = 0;
        }
        return record; //??

    }
};


// class Solution {
// public:
//     void moveZeroes(vector<int>& nums) {
//         int i = 0, j = 0;
//         int tmp;
        
//         while (j < nums.size())
//         {
//             if (nums[j] == 0)
//                 j++;
//             else
//             {
//                 tmp = nums[j];
//                 nums[j] = nums[i];
//                 nums[i] = tmp;
//                 i++;
//                 j++;                
//             }                 
//         }
//     }
// };
```
##### 168. Excel Sheet Column Title
- py
- status: not yet completed
```
class Solution:
    def convertToTitle(self, columnNumber: int) -> str:
        tens = columnNumber/26
        units = columnNumber%26
        print(chr(tens+96))
        # return ''.join([tens, units])

```
##### 021. Merge Two Sorted Lists
- js
- status: not yet completed
```
```

##### 344. Reverse String
- 
- status: not yet completed
```
``` 


模板----------------------------------------------
##### 
- 
- status: not yet completed
```
```
