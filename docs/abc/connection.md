# 软件互联协议机制

软件使用网络协议取向：

* 客户端间歇性的发起无状态的查询且允许发生延迟，使用http/https，如：浏览器
* 客户端和服务器都可独立发包的情况下： 
    * 可容忍延迟但对数据来说一个字节都不能改变，使用tcp，如：在线斗地主
    * 有实时性要求，准许部分字节错误，但不能容忍延迟，使用udp，如：即时动作类游戏

TCP/IP协议拓扑图

<!-- ![](https://ipfs.io/ipfs/QmWu85jmMDSfWNRDtX2JrtRtkqpWDvAWj9XQhXmY85p6Bv?0.png) -->

![](https://raw.githubusercontent.com/hoodiearon/fq-book/master/docs/images/171651525642888.png)

所以VPN能连接TCP与UDP协议，是因为虚拟网卡以及其生成的IP比TCP与UDP更为底层；sock处于OSI模型中的会话层，负责在数据传输中设置和维护电脑网络中两台电脑之间的通信连接，并不关心是何种应用协议，以至于sock代理不能互联用于其他协议的软件。典型的例子：v2ray需要switchyomega在表示层做中继代理打开被封锁的站点。

由于游戏外挂使用Socks代理的也较多，为了防止外挂，封禁也是最立竿见影的办法，Proxifer这类转换网络协议的软件也卻遭到鱼池之殃；当然，最好的办法还是刷梅林路由器，路由器本身就是小型linux系统，因此可以从物理层的路由器内嵌SS转发UDP，因为外挂识别主要针对PC操作系统而不是路由器，所以并不会被游戏厂商认为是外挂。

