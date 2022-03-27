# introduction

## Summary

数据库内核开发相对来说是一个比较冷门的专业（持疑问态度?）
本书抛砖引玉，可以作为对数据库内核开发有一定兴趣的新手的入门材料。另一方面，也是记录本人学习的过程。希望有更多的人加入数据库内核开发，特别是ClickHouse。
一般来说数据库可以粗略的分为计算层与存储层。本书同样也按照这个分了两个大模块，第一个模块详细介绍计算层，也就是数据库是如何把一个用户给的SQL执行，直到输出结果的过程。第二个模块将会详细介绍MergeTree,这是ClickHouse底层的存储。

在学习数据库内核的过程中，个人感受就是对于有些东西没有概念，甚至不知道它是个啥，学起来就会十分的迷茫。比如我刚开始接触的时候甚至连AST(Abstract Syntax Tree)都不知道是什么，于是学习起来就十分的迷茫和折磨。

## part1 sql执行流程

1. SQL -> AST
2. AST -> AST optimized
3. AST optimized -> Actions
4. actions -> QueryPlan
5. queryPlan -> QueryPipeline
6. QueryPipeline执行


## part2 MergeTree

7. MergeTree的基础
8. Merge的过程
9. Mutation的过程
10. derivation of MergeTree
