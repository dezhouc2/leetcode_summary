```python

--*:基础知识：
常见的BFS用来解决什么问题？
(0) 是否有路径问题

(1) 简单图（有向无向皆可）的最短路径长度，注意是长度而不是具体的路径

(2）拓扑排序(判断图中是否有环,一般用dfs来表示)

(3） 遍历一个图（或者树）

--*:BFS基本模板（需要记录层数或者不需要记录层数）
(1) 需要记录层数 (多用于树的载体)
queue = [start]
viz = set()  ## 用于记录路径避免重复
viz.add(start)
step = 0 ##步数为0

while queue:
  size = len(queue)  #记录此时queue中层的个数
  
  for i in range(size):  ##遍历这一层所有的点
    s = queue.pop(0)
    if s == target:
      return step
     
    for x in [(上),(下),(左),(右)]:  #邻居节点
      if x 满足限制 和 x不在viz:
        x加入queue
        x加入viz
    step = step +1



(2) 不需要记录层树 (多用于图的载体)


--*: 复杂度
(1)时间
如果是图的话大多数为 o(e+v) 边的个数加点的个数; 如果是树的话 为o(v) 点的个数

(2)空间
图/树大多数为 o(v) 点的个数





```
