# Ch0 introduction

## part1 sql执行流程

1. sql-> AST
2. AST -> AST optimized
3. AST optimized -> Actions
4. actions -> QueryPlan
5. queryPlan -> QueryPipeline
6. QueryPipeline执行


## part2 MergeTree

1. MergeTree的基础
2. Merge的过程
3. Mutation的过程
4. derivation of MergeTree
