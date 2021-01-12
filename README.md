# SnowFlake
* 核心功能生成16位的单机版UUID字符串，java默认的36位太长了 使用SnaowFlake.UUID() *

Twitter的雪花算法SnowFlake，使用Java语言实现。

SnowFlake算法用来生成64位的ID，刚好可以用long整型存储，能够用于分布式系统中生产唯一的ID， 并且生成的ID有大致的顺序。
在这次实现中，生成的64位ID可以分成5个部分：

  `0 - 40位时间戳 - 10位机器标识 - 13位序列号`
