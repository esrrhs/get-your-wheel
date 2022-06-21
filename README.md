# Get-Your-Wheel
C++轮子速查手册，无需重复发明轮子

# 1、容器
## 1.1、hash类容器
### 1.1.1、支持并发 
* 并发hash array，固定大小，[AtomicHashArray.h](https://github.com/facebook/folly/blob/main/folly/AtomicHashArray.h)
* 并发hash map，[AtomicHashMap.h](https://github.com/facebook/folly/blob/main/folly/AtomicHashMap.h)
