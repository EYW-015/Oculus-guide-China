# 虚拟机软路由\(穷人方案\)

给周扒皮们用的终极方案，**不花钱**就可以获得一台软路由，但是**特别花时间和脑子**

{% hint style="info" %}
你是台式机，既没有无线网卡，也没有科学路由器，还没有ROOT手机，更不想多花一分钱去买一个路由器，那不花钱就只能花时间了
{% endhint %}

## 查看局域网IP段

查看你电脑的IP，系统托盘点击**`网络` &gt; `属性`**  
如果你的电脑使用的是**有线连接**，那么进入以太网详细信息寻找IP

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/wifi/wifi1.png)

下拉至详细属性，寻找你的**`IPv4 地址`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/wifi/wifi2.png)

**把这个IP地址记住，之后会频繁用到它  
！主要是前三段IP地址！  
！主要是前三段IP地址！  
！主要是前三段IP地址！**

## **虚拟机安装**

下载 [**VirtualBox虚拟机**](https://www.virtualbox.org/wiki/Downloads) ****并安装  
下载这个用于虚拟机的 **软路由固件** 并解压准备好，解压不了的去装一个 [**Bandizip**](https://cn.bandisoft.com/bandizip/)\*\*\*\*

先安装好虚拟机，安装完成后点击**`新建`**，名称为**`Openwrt`**，类型选择**`Linux`**，版本选择**`Other Linux (64-bit)`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm1.png)

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm2.png)

内存默认设为**`512MB`**，选择**`使用已有的虚拟硬盘文件`**，点击右边的**`文件夹图标`**，左上角**`注册`**，找到并选择之前解压好格式为**`vmdk`**的**`软路由固件`**，选择添加的固件，**`创建`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm3.png)

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm4.png)

选择创建的虚拟机，点击**`设置` &gt; `网络`**，连接方式改为**`桥接网卡` &gt; `OK` &gt; `启动`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm5.png)

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm6.png)



![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/vm/vm11.png)

## 软路由设置

打开浏览器，输入你刚才**虚拟机里设置的IP**，例如**`192.168.50.222`**  
输入密码**`password`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op2.png)

顶部**`网络` &gt; `接口` &gt; `LAN` &gt; `修改`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op3.png)

将**`IPv4网关`**设置为你的**WIFI路由器**地址，例如**`192.168.50.1`**  
将**`自定义DNS服务器`**设置为**`119.29.29.29`**  
拉到最底下，保存应用

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op4.png)

顶部**`服务` &gt; `SSR Plus` &gt; `服务器节点`**，复制你机场的**`订阅地址`**，粘贴进**`订阅URL`**框内  
点击**`更新订阅URL列表`**  
点击**`更新所有订阅服务器节点`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op5.png)

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op6.png)

左上角点击**`客户端`**  
**`主服务器`**选择你要用的节点  
**`游戏模式UDP`**选择与**`主服务相同`**  
**`代理端口`**选择**`所有端口`**  
保存应用

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op1.png)

Quest激活完成后  
将**`代理端口`**设为**`常用端口`**  
将**`游戏模式UDP中继服务器`**设置为**`停用`**

## Quest联网

将头显连接WIFI，在**输入密码的时候**打开下方**`高级设置`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/quest/wifi1.jpg)

将**`IP设置`**选为**`静态`**  
**`IP地址`前三段**填写为与你的**电脑IP地址**前三段相同，例如**`192.168.50.xxx`**，这里的**`xxx`**自己换一个数，例如**`233`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/quest/wifi2.jpg)

**`网关`**和**`DNS1`**填写为你的**`虚拟机IP地址`**，例如**`192.168.50.222`** 其他选项不动，然后连接至WIFI即可激活

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/quest/wifi3.jpg)

