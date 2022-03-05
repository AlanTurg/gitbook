# StrictRedis

* [课程介绍](broken-reference)
* **1.** Redis
*
* [本書使用 GitBook 釋出](https://www.gitbook.com)

### StrictRedis对象⽅法 <a href="#strictredis-dui-xiang-fa" id="strictredis-dui-xiang-fa"></a>

* 通过init创建对象，指定参数host、port与指定的服务器和端⼝连接，host默认为localhost，port默认为6379，db默认为0

```
sr = StrictRedis(host='localhost', port=6379, db=0)

简写
sr=StrictRedis()
```

* 根据不同的类型，拥有不同的实例⽅法可以调⽤，与前⾯学的redis命令对应，⽅法需要的参数与命令的参数⼀致

### string <a href="#string" id="string"></a>

* set
* setex
* mset
* append
* get
* mget
* key

### keys <a href="#keys" id="keys"></a>

* exists
* type
* delete
* expire
* getrange
* ttl

### hash <a href="#hash" id="hash"></a>

* hset
* hmset
* hkeys
* hget
* hmget
* hvals
* hdel

### list <a href="#list" id="list"></a>

* lpush
* rpush
* linsert
* lrange
* lset
* lrem

### set <a href="#set" id="set"></a>

* sadd
* smembers
* srem

### zset <a href="#zset" id="zset"></a>

* zadd
* zrange
* zrangebyscore
* zscore
* zrem
* zremrangebyscore
