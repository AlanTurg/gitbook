# 数据操作

### 学习目标 <a href="#xue-xi-mu-biao" id="xue-xi-mu-biao"></a>

* 能够写出Redis中string类型数据的增删改查操作命令
* 能够写出Redis中hash类型数据的增删改查相关命令

### 重要文档 <a href="#zhong-yao-wen-dang" id="zhong-yao-wen-dang"></a>

* [Redis 参考命令](http://doc.redisfans.com)
* [Redis 官方文档](https://redis-py.readthedocs.io/en/latest/#indices-and-tables)

### 数据结构 <a href="#shu-ju-jie-gou" id="shu-ju-jie-gou"></a>

* redis是key-value的数据结构，每条数据都是⼀个键值对
* 键的类型是字符串
* 注意：键不能重复
* 值的类型分为五种：
  * 字符串string
  * 哈希hash
  * 列表list
  * 集合set
  * 有序集合zset

### 数据操作行为 <a href="#shu-ju-cao-zuo-hang-wei" id="shu-ju-cao-zuo-hang-wei"></a>

* 保存
* 修改
* 获取
* 删除

点击中⽂官⽹查看命令⽂档[http://redis.cn/commands.html](http://redis.cn/commands.html)
