# Get-Your-Wheel
C++轮子速查手册，无需重复发明轮子

# 0、原则
* 从知名C++库收集轮子
* 与STD标准库相似的不收录
* 应用面太小的不收录

# 1、容器
## 1.1、hash类容器
### 1.1.1、支持并发 
* 并发hash array，固定大小：[AtomicHashArray.h](https://github.com/facebook/folly/blob/main/folly/AtomicHashArray.h)
* 并发hash map：[AtomicHashMap.h](https://github.com/facebook/folly/blob/main/folly/AtomicHashMap.h)
* 并发unorder map，固定大小：[AtomicUnorderedMap.h](https://github.com/facebook/folly/blob/main/folly/AtomicUnorderedMap.h)
* 
## 1.2、链表类容器
### 1.2.1、支持并发 
* 简单的并发链表，只支持头部插入、遍历：[AtomicLinkedList.h](https://github.com/facebook/folly/blob/main/folly/AtomicLinkedList.h)
* 并发跳表：[ConcurrentSkipList.h](https://github.com/facebook/folly/blob/main/folly/ConcurrentSkipList.h)

## 1.3、bit类容器
### 1.3.1、支持并发 
* 并发bit map，固定大小：[ConcurrentBitSet.h](https://github.com/facebook/folly/blob/main/folly/ConcurrentBitSet.h)
* 

# 2、模板元编程
## 2.1、数学类
* 计算max、min、log2、pow等：[ConstexprMath.h](https://github.com/facebook/folly/blob/main/folly/ConstexprMath.h)
