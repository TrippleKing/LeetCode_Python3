从上到下打印二叉树 III

# 题目描述

请实现一个函数按照之字形顺序打印二叉树，即第一行按照从左到右的顺序打印，第二层按照从右到左的顺序打印，第三行再按照从左到右的顺序打印，其他行以此类推。

## 示例

给定二叉树：`[3,9,20,null,null,15,7]`

```
    3
   / \
  9  20
    /  \
   15   7
```

返回其层次遍历结果：

```
[
  [3],
  [20,9],
  [15,7]
]
```

## 提示

- `节点总数 <= 1000`

# 解题思路

> 本题是[从上到下打印二叉树](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题32-I.从上到下打印二叉树.md)和[从上到下打印二叉树 II](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题32-II.从上到下打印二叉树II.md)的一个衍生，依然是按层打印，差异是每一层打印顺序发生变化。

对比之前两题，本题的关键在于何时进行反向打印。如何判断节点在同一层在[从上到下打印二叉树 II](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题32-II.从上到下打印二叉树II.md)中已经有明确的描述，我们只要设置一个反向标志符，来提示打印需要反向即可。（每一次打印完一层节点，下一次必然发生反向）

## 复杂度分析

- 时间复杂度：$O(N)$
- 空间复杂度：$O(N)$

## 代码

```python
# Definition for a binary tree node.
# class TreeNode:
#     def __init__(self, x):
#         self.val = x
#         self.left = None
#         self.right = None

class Solution:
    def levelOrder(self, root: TreeNode) -> List[List[int]]:

        if not root: return []
        queue = collections.deque()
        res = []
        queue.append(root)
        flag = -1
        while queue:
            tmp = []
            for _ in range(len(queue)):
                node = queue.popleft()
                tmp.append(node.val)
                if node.left: queue.append(node.left)
                if node.right: queue.append(node.right)
            flag = -flag
            if flag == 1:
                res.append(tmp)
            else:
                res.append(tmp[::-1])
        return res
    
# 补充：也可以使用双端队列来构建tmp，判断换层也可以根据res当前行数是否为奇数/偶数进行判断
# 代码如下：供参考
class Solution:
    def levelOrder(self, root: TreeNode) -> List[List[int]]:

        if not root: return []
        queue = collections.deque()
        res = []
        queue.append(root)
        while queue:
            tmp = collections.deque()
            for _ in range(len(queue)):
                node = queue.popleft()
                if len(res) & 1:
                    tmp.appendleft(node.val)
                else:
                    tmp.append(node.val)        
                if node.left: queue.append(node.left)
                if node.right: queue.append(node.right)
            res.append(list(tmp))
        return res
```

