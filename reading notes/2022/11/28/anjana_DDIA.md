# 11.28

索引部分一直半懂，所以看到DDIA索引部分跑去看了《高性能MySQL》的索引部分。

## Chapter5 创建高性能的索引

索引定义：`存储引擎`用于快速找到记录的一种`数据结构`。

索引对多个值进行排序的依据是CREATE TABLE语句中定义索引时`列的顺序`。

B-Tree index:

* 全键值查找
* 键值范围查找
* 键前缀查找：仅适用于根据最左前缀的查找

如何判断一个系统的索引是合理的：

1. 按响应时间对查询分析：找出那些消耗最长时间/给服务器带来最大压力的查询
2. 检查这些查询的schema、SQL和索引结构
3. 判断是否
   * 扫描了太多行
   * 做了很多额外排序
   * 使用了临时表
   * 使用随机I/O访问数据
   * 有太多回表查询那些不在索引中的列的操作


