## 代码调优法则

### 空间换时间

修改数据结构

* 在数据结构中增加额外的信息
* 修改数据结构中的信息使之更易访问

存储预先计算好的结果

高速缓存

懒惰求值

### 时间换空间

堆积

解释程序

### 循环法则

将代码移出循环

合并测试条件

* 高效的内循环应该包含尽量少的测试条件，最好只有一个。
* 应用：哨兵

循环展开

* 避免管道延迟
* 减少分支
* 增加指令级的并行性

注：但真心觉得循环展开代码可读性不好。

删除赋值

消除无条件分支

循环合并

### 逻辑法则

利用等价的代数表达式

短路单调函数

对测试条件重新排序

预先计算逻辑函数

消除布尔变量

### 过程法则

打破函数层次

协同程序：

* 将多趟算法转换为单趟算法
* 管道

递归函数转换

* 递归——>迭代
* 消除尾递归

并行性

### 表达式法则

编译时初始化

* 在程序执行前，对尽可能多的变量初始化

利用等价的代数表达式

* 2的幂运算——>左移/右移
* 乘法——>加法

消除公共子表达式

成对计算

利用计算机字的并行性

