title: 用R将两列的表格转化为行列的矩阵
date: 2016-02-20 15:44:00
tags: [date, R, coding]
---

> 用R将两列索引的表格转化为,二维的行列的矩阵

## example
### 表格长这样
| gene    | trait     | value    |
|---------|-----------|----------|
| YAR010C | D108_C    | 0.566691 |
| YBL016W | CCV12-1_C | 0.567051 |
| YBL016W | CCV128_C  | 0.587467 |
| YBR037C | D109_C    | 0.566084 |
| YBR040W | C101_A1B  | 0.578845 |
| YBR040W | C101_C    | 0.598443 |
| YBR040W | C102_C    | 0.587275 |
| YBR040W | C103_A1B  | 0.593403 |
| YBR040W | C103_C    | 0.597879 |
| YBR040W | C11-1_A   | 0.571026 |
| ...     | ...       | ...      |


### 代码在这里
```R
a <-read.table("gene_trait_table",head=T)
b<-data.frame()
fun<-function(x){b[x["gene"],x["trait"]] <<- x["value"]}
apply(a,1, fun)
```
