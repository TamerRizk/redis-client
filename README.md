redis-client
============

*Redis client for TeaJS*


var Redis = require('redis').Redis; 

var redis = new Redis({host:config.redis.host, port:config.redis.port, password:config.redis.pw, db:config.redis.db});

var keys = redis.query('keys *');
system.stdout.writeLine(redis.status);

system.stdout.writeLine(keys.join("\n"));

redis.disconnect();
