Leetcode刷题笔记整理——Python3

By Xyao

本人从2020/04/25开始正式在LeetCode上刷题，于2020/07/04完整刷完一遍剑指offer系列，边刷题边整理笔记。（此处特别感谢LeetCode解题区及评论区的大佬们提供的一些优质题解！在笔记整理过程中也参考了大佬们的解题思路，如认为有所侵权，请与我联系：Xyao@zju.edu.cn）

如果有发现超链接错误或网页打不开的情况及其他问题，欢迎留言~

# 剑指Offer系列

> 最近LeetCode把剑指offer的题从原来的`面试题 03`改为了`剑指Offer 03`，只是改了名字而已，其他没什么变化。
>
> 这里将笔记按照顺序简单整理一下，方便大家快速查找。

- [剑指Offer 03 - 数组中重复的数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题03.数组中重复的数字.md)
- [剑指Offer 04 - 二维数组中的查找](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题04.二维数组中的查找.md)
- [剑指Offer 05 - 替换空格](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题05.替换空格.md)
- [剑指Offer 06 - 从尾到头打印链表](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题06.从尾到头打印链表.md)
- [剑指Offer 07 - 重建二叉树](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题07.重建二叉树.md)
- [剑指Offer 09 - 用两个栈实现队列](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题09.用两个栈实现队列.md)
- [剑指Offer 10-I - 斐波那契数列](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题10-I.斐波那契数列.md)
- [剑指Offer 10-II - 青蛙跳台阶的问题](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题10-II.青蛙跳台阶问题.md)
- [剑指Offer 11 - 旋转数组的最小数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题11.旋转数组的最小数字.md)
- [剑指Offer 12 - 矩阵中的路径](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题12.矩阵中的路径.md)
- [剑指Offer 13 - 机器人的运动范围](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题13.机器人的运动范围.md)
- [剑指Offer 14-I - 剪绳子](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题14-I.剪绳子.md)
- [剑指Offer 14-II - 剪绳子 II](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题14-II.剪绳子II.md)
- [剑指Offer 15 - 二进制中1的个数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题15.二进制中1的个数.md)
- [剑指Offer 16 - 数值的整数次方](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题16.数值的整数次方.md)
- [剑指Offer 17 - 打印从1到最大的n位数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题17.打印从1到最大的n位数.md)
- [剑指Offer 18 - 删除链表的节点](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题18.删除链表的节点.md)
- [剑指Offer 19 - 正则表达式匹配](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题19.正则表达式匹配.md)
- [剑指Offer 20 - 表示数值的字符串](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题20.表示数值的字符串.md)
- [剑指Offer 21 - 调整数组顺序使奇数位于偶数前面](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题21.调整数组顺序使奇数位于偶数前面.md)
- [剑指Offer 22 - 链表中倒数第k个节点](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题22.链表中倒数第k个节点.md)
- [剑指Offer 24 - 反转链表](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题24.反转链表.md)
- [剑指Offer 25 - 合并两个排序的链表](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题25.合并两个排序的链表.md)
- [剑指Offer 26 - 树的子结构](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题26.树的子结构.md)
- [剑指Offer 27 - 二叉树的镜像](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题27.二叉树的镜像.md)
- [剑指Offer 28 - 对称的二叉树](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题28.对称二叉树.md)
- [剑指Offer 29 - 顺时针打印矩阵](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题29.顺时针打印矩阵.md)
- [剑指Offer 30 - 包含min函数的栈](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题30.包含min函数的栈.md)
- [剑指Offer 31 - 栈的压入、弹出序列](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题31.栈的压入、弹出序列.md)
- [剑指Offer 32-I - 从上到下打印二叉树](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题32-I.从上到下打印二叉树.md)
- [剑指Offer 32-II - 从上到下打印二叉树 II](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题32-II.从上到下打印二叉树II.md)
- [剑指Offer 32-III - 从上到下打印二叉树 III](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题32-III.从上到下打印二叉树III.md)
- [剑指Offer 33 - 二叉搜索树的后序遍历序列](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题33.二叉搜索树的后序遍历序列.md)
- [剑指Offer 34 - 二叉树中和为某一值的路径](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题34.二叉树中和为某一值的路径.md)
- [剑指Offer 35 - 复杂链表的复制](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题35.复杂链表的复制.md)
- [剑指Offer 36 - 二叉搜索树与双向链表](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题36.二叉搜索树与双向链表.md)
- [剑指Offer 37 - 序列化二叉树](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题37.序列化二叉树.md)
- [剑指Offer 38 - 字符串的排列](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题38.字符串的排列.md)
- [剑指Offer 39 - 数组中出现次数超过一半的数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题39.数组中出现次数超过一半的数字.md)
- [剑指Offer 40 - 最小的k个数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题40.最小的k个数.md)
- [剑指Offer 41 - 数据流中的中位数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题41.数据流中的中位数.md)
- [剑指Offer 42 - 连续子数组的最大和](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题42.连续子数组的最大和.md)
- [剑指Offer 43 - 1~n整数中1出现的次数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题43.1~n整数中1出现的次数.md)
- [剑指Offer 44 - 数字序列中某一位的数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题44.数字序列中某一位的数字.md)
- [剑指Offer 45 - 把数组排成最小的数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题45.把数组排成最小的数.md)
- [剑指Offer 46 - 把数字翻译成字符串](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题46.把数字翻译成字符串.md)
- [剑指Offer 47 - 礼物的最大价值](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题47.礼物的最大价值.md)
- [剑指Offer 48 - 最长不含重复字符的子字符串](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题48.最长不含重复字符的子字符串.md)
- [剑指Offer 49 - 丑数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题49.丑数.md)
- [剑指Offer 50 - 第一个只出现一次的字符](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题50.第一个只出现一次的字符.md)
- [剑指Offer 51 - 数组中的逆序对](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题51.数组中的逆序对.md)
- [剑指Offer 52 - 两个链表的第一个公共节点](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题52.两个链表的第一个公共节点.md)
- [剑指Offer 53-I - 在排序数组中查找数字 I](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题53-I.在排序数组中查找数字I.md)
- [剑指Offer 53-II - 0~n-1中缺失的数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题53-II.0~n-1中缺失的数字.md)
- [剑指Offer 54 - 二叉搜索树的第k大节点](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题54.二叉搜索树的第k大节点.md)
- [剑指Offer 55-I - 二叉树的深度](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题55-I.二叉树的深度.md)
- [剑指Offer 55-II - 平衡二叉树](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题55-II.平衡二叉树.md)
- [剑指Offer 56-I - 数组中数字出现的次数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题56-I.数组中数字出现的次数.md)
- [剑指Offer 56-II - 数组中数字出现的次数 II](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题56-II.数组中数字出现的次数II.md)
- [剑指Offer 57 - 和为s的两个数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题57.和为s的两个数字.md)
- [剑指Offer 57-II - 和为s的连续正数序列](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题57-II.和为s的连续正数序列.md)
- [剑指Offer 58-I - 翻转单词顺序](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题58-I.翻转单词顺序.md)
- [剑指Offer 58-II - 左旋转字符串](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题58-II.左旋转字符串.md)
- [剑指Offer 59-I - 滑动窗口的最大值](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题59-I.滑动窗口的最大值.md)
- [剑指Offer 59-II - 队列的最大值](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题59-II.队列的最大值.md)
- [剑指Offer 60 - n个骰子的点数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题60.n个骰子的点数.md)
- [剑指Offer 61 - 扑克牌中的顺子](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题61.扑克牌中的顺子.md)
- [剑指Offer 62 - 圆圈中最后剩下的数字](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题62.圆圈中最后剩下的数字.md)
- [剑指Offer 63 - 股票的最大利润](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题63.股票的最大利润.md)
- [剑指Offer 64 - 求1+2+...+n](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题64.求1%2B2%2B...%2Bn.md)
- [剑指Offer 65 - 不用加减乘除做加法](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题65.不用加减乘除做加法.md)
- [剑指Offer 66 - 构建乘积数组](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题66.构建乘积数组.md)
- [剑指Offer 67 - 把字符串转换成整数](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题67.把字符串转换成整数.md)
- [剑指Offer 68-I - 二叉搜索树的最近公共祖先](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题68-I.二叉搜索树的最近公共祖先.md)
- [剑指Offer 68-II - 二叉树的最近公共祖先](https://github.com/TrippleKing/LeetCode_Python3/blob/master/剑指offer系列/面试题68-II.二叉树的最近公共祖先.md)

# 每日一题系列

> 该系列先不作目录整理。