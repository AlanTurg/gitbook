# 键命令

* [课程介绍](broken-reference)
* **1.** Redis
*
* [本書使用 GitBook 釋出](https://www.gitbook.com)

### 学习目标 <a href="#xue-xi-mu-biao" id="xue-xi-mu-biao"></a>

* 能够写出删除指定键的相关命令

### 键命令 <a href="#jian-ming-ling" id="jian-ming-ling"></a>

*   查找键，参数⽀持正则表达式

    > keys pattern
*   例1：查看所有键

    > keys \*

    ![](../../.gitbook/assets/p1\_20)
*   例2：查看名称中包含`a`的键

    > keys a\*

    ![](../../.gitbook/assets/p1\_21)
*   判断键是否存在，如果存在返回`1`，不存在返回`0`

    > exists key1
*   例3：判断键`a1`是否存在

    > exists a1

    ![](../../.gitbook/assets/p1\_22)
*   查看键对应的`value`的类型

    > type key
*   例4：查看键`a1`的值类型，为redis⽀持的五种类型中的⼀种

    > type a1

    ![](../../.gitbook/assets/p1\_23)
*   删除键及对应的值

    > del key1 key2 ...
*   例5：删除键`a2、a3`

    > del a2 a3

    ![](../../.gitbook/assets/p1\_24)
* 设置过期时间，以秒为单位
*   如果没有指定过期时间则⼀直存在，直到使⽤`DEL`移除

    > expire key seconds
*   例6：设置键`a1`的过期时间为3秒

    > expire a1 3

    ![](../../.gitbook/assets/p1\_25)
*   查看有效时间，以秒为单位

    > ttl key
*   例7：查看键`bb`的有效时间

    > ttl bb

    ![](../../.gitbook/assets/p1\_27)
