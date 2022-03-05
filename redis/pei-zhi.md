# 配置

* [课程介绍](broken-reference)
* **1.** Redis
*
* [本書使用 GitBook 釋出](https://www.gitbook.com)

### 学习目标 <a href="#xue-xi-mu-biao" id="xue-xi-mu-biao"></a>

* 能够根据参考资料修改常用Redis配置

### 配置 <a href="#pei-zhi" id="pei-zhi"></a>

* Redis的配置信息在`/etc/redis/redis.conf`下。
*   查看

    > sudo vi /etc/redis/redis.conf

### 核心配置选项 <a href="#he-xin-pei-zhi-xuan-xiang" id="he-xin-pei-zhi-xuan-xiang"></a>

*   绑定ip：如果需要远程访问，可将此⾏注释，或绑定⼀个真实ip

    > bind 127.0.0.1
*   端⼝，默认为6379

    > port 6379
*   是否以守护进程运⾏

    * 如果以守护进程运⾏，则不会在命令⾏阻塞，类似于服务
    * 如果以⾮守护进程运⾏，则当前终端被阻塞
    * 设置为yes表示守护进程，设置为no表示⾮守护进程
    * 推荐设置为yes

    > daemonize yes
*   数据⽂件

    > dbfilename dump.rdb
*   数据⽂件存储路径

    > dir /var/lib/redis
*   ⽇志⽂件

    > logfile "/var/log/redis/redis-server.log"
*   数据库，默认有16个

    > database 16
*   主从复制，类似于双机备份。

    > slaveof

### 参考资料 <a href="#can-kao-zi-liao" id="can-kao-zi-liao"></a>

redis配置信息[http://blog.csdn.net/ljphilp/article/details/52934933](http://blog.csdn.net/ljphilp/article/details/52934933)
