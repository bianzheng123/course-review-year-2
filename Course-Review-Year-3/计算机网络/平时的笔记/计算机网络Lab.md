# 计算机网络Lab

### Week1

网络号和主机号唯一的标记主机

子网掩码

- 显示的是网络号和主机号的区别

- 是一个32位的2进制数， 其对应网络地址的所有位都置为1，对应于主机地址的所有位都置为0

IP地址

`ping 127.0.0.1` 看看TCP，IP协议是否正常

默认网关

- 当主机访问其他网络时第一个需要过的网关

DNS服务器

- 解析域名和ip地址的服务器

`ping 127.0.0.1`

- 代表端到端的测试

- 即将一个测试报文发送到指定的服务器

`tracert www.baidu.com`

- 将测试报文发送到指定的ip地址，测试其追踪的路径

- 测定路由跳数

- ipconfig查看网络的连接状态

`nslookup`

- 通过ip地址查找域名，

- 也可以反向查找，可能不会成功

TTL

- 报文的生存时间，每经过一个路由器生命值就减1
- 对于测试类的报文，路由器将自己的ip地址打包，发送回来，并且将该测试报文发送到下一个路由器上

不同的网络上会连接不同的IP地址

TCP如果发生丢包就重传，UDP就不会

netstat通过IP地址查看TCP，UDP端口状态