``
## 字母大小写问题
- string.upper() #转化string中所有字母大写
- string.lower() #转化string中所有字母小写
- string[0].lower() ##如果要只转化一个字母的大/小写利用slicing


## 排序:
- 方法一:
在list原来的基础上sort不额外增加空间即 space complexity为o(1)
sort() 有两个变量 一个是key,另外一个是reverse = False(默认)
list.sort(key = lambda x:x[0], reverse = True)

- 方法二:
用额外的空间 即space complexity 为o(n)
sorted() 有三个变量 要进行排序的iterable,key,reverse
sored(iterable, key,reverse)

- examples:
#对list1的index1元素进行降序排序
list1 = [("a",1),("b",2),("c",3)]

list1.sort(key = lambda x:x[1], reverse = True) ##[('c', 3), ('b', 2), ('a', 1)]

list2 = sorted(list1,key = lambda x:x[1], reverse=True) ##[('c', 3), ('b', 2), ('a', 1)]


``



