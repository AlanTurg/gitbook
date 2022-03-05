# 服务端和客户端命令

* [课程介绍](broken-reference)
* **1.** Redis
*
* [本書使用 GitBook 釋出](https://www.gitbook.com)

### 学习目标 <a href="#xue-xi-mu-biao" id="xue-xi-mu-biao"></a>

*   了解Redis服务器端和客户端的命令

    ### 服务器端 <a href="#fu-wu-qi-duan" id="fu-wu-qi-duan"></a>
* 服务器端的命令为redis-server
*   可以使⽤help查看帮助⽂档

    > redis-server --help
*   个人习惯

    > ps aux | grep redis 查看redis服务器进程\
    > sudo kill -9 pid 杀死redis服务器\
    > sudo redis-server /etc/redis/redis.conf 指定加载的配置文件

### 客户端 <a href="#ke-hu-duan" id="ke-hu-duan"></a>

* 客户端的命令为redis-cli
*   可以使⽤help查看帮助⽂档

    > redis-cli --help
*   连接redis

    > redis-cli
*   运⾏测试命令

    > ping
* 切换数据库
*   数据库没有名称，默认有16个，通过0-15来标识，连接redis默认选择第一个数据库

    > select 10
