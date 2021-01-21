# NAT 测试工具

## NAT / UDP 测试工具

* [最新版本发布页](https://github.com/HMBSbige/NatTypeTester/releases/)

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/nat.png)

其中的Public end可以反映出你的UDP传输有没有经过加速器 / 梯子转发：  
Public end显示的是你当前连接到测试服务器使用的网络IP地址与端口，  
冒号前面（不包含冒号）的是IP地址，将IP地址复制到查询工具中查询，  
IP在线查询：[IPIP.NET](https://www.ipip.net/ip.html) / [ChinaZ站长之家](http://ip.tool.chinaz.com/) / [淘宝IP库](http://ip.taobao.com/)  
如果查询到的位置是你的本地宽带，那么说明UDP是直连，没有生效，  
如果查询到的位置是加速器 / 梯子服务器的所在地，那么说明经过了转发，加速生效

### 注意

只能测试电脑连接的wifi是否可科学转发udp，如果wifi热点本身是由这台电脑共享的，推荐使用另一台电脑连接该热点测试  
如果你在别处下载过NatTypeTester，也请重新下载，我们提供的是确保实现正确的版本，有个广为流传的旧版实现不正确，测试结果不准  
如果测试工具的服务器出问题，也会影响测试结果，如果你担心这点，可以在STUN Server选项中切换到不同服务器后重新运行测试  


