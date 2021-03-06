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

## 1.4、数组类容器
### 1.4.1、支持并发 
### 1.4.2、不支持并发 
* 替换std::vector，针对就地重新分配（in-place reallocation）和jemalloc有优化：[FBVector.h](https://github.com/facebook/folly/blob/main/folly/FBVector.h)

# 2、模板元编程
## 2.1、数学类
* 计算max、min、log2、pow等：[ConstexprMath.h](https://github.com/facebook/folly/blob/main/folly/ConstexprMath.h)
## 2.1、数据结构
* 模板实现的常量字符串：[FixedString.h](https://github.com/facebook/folly/blob/main/folly/FixedString.h)


# 3、硬件相关
## 3.1、CPU
* 获取cpu信息：[CpuId.h](https://github.com/facebook/folly/blob/main/folly/CpuId.h)
* 


# 4、数据结构
## 4.1、指针相关
### 4.1.1、类型管理
* 可以存放多种类型的指针：[DiscriminatedPtr.h](https://github.com/facebook/folly/blob/main/folly/DiscriminatedPtr.h)

## 4.2、动态类型
* 运行时动态类型，可存放int、string、vector等：[dynamic.h](https://github.com/facebook/folly/blob/main/folly/dynamic.h)

## 4.3、期望值
* 表示期望的值或错误，支持then：[Expected.h](https://github.com/facebook/folly/blob/main/folly/Expected.h)


# 5、字符串相关
## 5.1、字符串
* 分成了小（无alloc）中(alloc)大(ref cnt)三种尺寸：[FBString.h](https://github.com/facebook/folly/blob/main/folly/FBString.h)
* 模板实现的常量字符串：[FixedString.h](https://github.com/facebook/folly/blob/main/folly/FixedString.h)
## 5.2、格式化
* 使用{}进行格式化：[Format.h](https://github.com/facebook/folly/blob/main/folly/Format.h)

# 6、文件
* 对于文件读写的封装：[FileUtil.h](https://github.com/facebook/folly/blob/main/folly/FileUtil.h)


# 7、算法
## 7.1、加密相关
* 根据原始信息生成指纹：[Fingerprint.h](https://github.com/facebook/folly/blob/main/folly/Fingerprint.h)

