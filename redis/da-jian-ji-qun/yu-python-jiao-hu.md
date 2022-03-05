# 与Python交互

### 安装包 <a href="#an-zhuang-bao" id="an-zhuang-bao"></a>

安装Redis的有3种方式[https://github.com/andymccurdy/redis-py](https://github.com/andymccurdy/redis-py)

*   第一种：进⼊虚拟环境，联⽹安装包redis

    > pip install redis
*   第二种：进⼊虚拟环境，联⽹安装包redis

    > easy\_install redis
*   第三种：到中⽂官⽹-客户端下载redis包的源码，使⽤源码安装

    > 一步步执行 wget [https://github.com/andymccurdy/redis-py/archive/master.zip](https://github.com/andymccurdy/redis-py/archive/master.zip)\
    > unzip master.zip\
    > cd redis-py-master\
    > sudo python setup.py install

### 调⽤模块 <a href="#tiao-mo-kuai" id="tiao-mo-kuai"></a>

*   引⼊模块

    > from redis import StrictRedis
* 这个模块中提供了`StrictRedis对象`，⽤于连接redis服务器，并按照不同类型提供 了不同⽅法，进⾏交互操作
