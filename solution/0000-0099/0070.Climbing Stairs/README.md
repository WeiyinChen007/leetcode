## 爬楼梯
### 题目描述

假设你正在爬楼梯。需要 n 阶你才能到达楼顶。

每次你可以爬 1 或 2 个台阶。你有多少种不同的方法可以爬到楼顶呢？

注意：给定 n 是一个正整数。

示例 1：
```
输入： 2
输出： 2
解释： 有两种方法可以爬到楼顶。
1.  1 阶 + 1 阶
2.  2 阶
```

示例 2：
```
输入： 3
输出： 3
解释： 有三种方法可以爬到楼顶。
1.  1 阶 + 1 阶 + 1 阶
2.  1 阶 + 2 阶
3.  2 阶 + 1 阶
```

### 解法
爬上 1 阶有 1 种方法，爬上 2 阶有 2 种方法，爬上 n 阶 f(n) 有 f(n - 1) + f(n - 2) 种方法。可以利用数组记录中间结果，防止重复计算。

```java
class Solution {
    public int climbStairs(int n) {
        if (n < 3) {
            return n;
        }
        int[] res = new int[n + 1];
        res[1] = 1;
        res[2] = 2;
        for (int i = 3; i < n + 1; ++i) {
            res[i] = res[i - 1] + res[i - 2];
        }
        return res[n];
    }
}
```

# [题目](这里是题目链接，如：https://leetcode-cn.com/problems/shu-zu-zhong-zhong-fu-de-shu-zi-lcof/)

## 题目描述
<!-- 这里写题目描述 -->


## 解法
<!-- 这里可写通用的实现逻辑 -->


### Python3
<!-- 这里可写当前语言的特殊实现逻辑 -->

```python

```

### Java
<!-- 这里可写当前语言的特殊实现逻辑 -->

```java

```

### ...
```

```