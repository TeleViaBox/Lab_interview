##### related knowledge:
- 常用算法：贪心法、字符串处理、递归、BFS、DFS、分治、排序
- 常用数据结构：数组/列表、队列、栈、链表、二叉树、哈希表

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
