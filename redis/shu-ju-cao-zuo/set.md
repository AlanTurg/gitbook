# set

* [课程介绍](broken-reference)
* **1.** Redis
*
* [本書使用 GitBook 釋出](https://www.gitbook.com)

### set类型 <a href="#xue-xi-mu-biao" id="xue-xi-mu-biao"></a>

* ⽆序集合
* 元素为string类型
* 元素具有唯⼀性，不重复
* 说明：对于集合没有修改操作

### 增加 <a href="#zeng-jia" id="zeng-jia"></a>

*   添加元素

    > sadd key member1 member2 ...
*   例1：向键`a3`的集合中添加元素`zhangsan`、`lisi`、`wangwu`

    > sadd a3 zhangsan sili wangwu

### 获取 <a href="#huo-qu" id="huo-qu"></a>

*   返回所有的元素

    > smembers key
*   例2：获取键`a3`的集合中所有元素

    > smembers a3

### 删除 <a href="#shan-chu" id="shan-chu"></a>

*   删除指定元素

    > srem key
*   例3：删除键`a3`的集合中元素`wangwu`

    > srem a3 wangwu
