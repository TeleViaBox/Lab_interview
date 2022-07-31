- 168. Excel Sheet Column Title
py
// status: not yet completed
```
class Solution:
    def convertToTitle(self, columnNumber: int) -> str:
        tens = columnNumber/26
        units = columnNumber%26
        print(chr(tens+96))
        # return ''.join([tens, units])

```
