* 找到起始点已知的直接相连的节点赋值, 将不能直接相连的节点赋值为无穷大.
* 从已知value的节点中找一个已经遍历过的节点中的最小值作为中继点,将自身值加上直连value后与该节点的value进行配比,如果比原有值小,则更新它.
* 递归执行到最后,便得到起始点到任意点之间的最短路径.
* 在处理value为负数时,可能会失效.


|1|2|3|4|
|:----:|:-----:|:----:|:----:|
|4|2|3|4|
|3|1|4|5|
|2|5|6|7|

* 以上表格中任意栅格代表一个节点
* 每个节点上的值代表该节点所拥有的代价
* 给出两个节点的索引(x1,y1)和(x2,y2)
* 计算两点间的最小代价

