
heap:
1.在python中, heap默认为minheap

2.如果想让heap为maxheap -> 只需要把所有的值*-1即可

3.minheap,maxheap 的本质为complete binary tree 
minheap: tree的node的值小于等于他的children的值
maxheap: tree的node的值大于等于他的children 的值

4.
hp = []
heapq.heappush(hp, (value1,value)) #默认根据value1来对比的





time: o(n*logk) -> 如果只需要topk的话
space:o(n)
