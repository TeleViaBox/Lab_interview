##### related knowledge:
- 常用算法：贪心法、字符串处理、递归、BFS、DFS、分治、排序
- 常用数据结构：数组/列表、队列、栈、链表、二叉树、哈希表

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
