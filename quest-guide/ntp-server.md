# ⏰ NTP解析激活(无需UDP)

## 原理

将Facebook时间服务器地址<mark style="color:blue;">**`time.facebook.com`**</mark>解析至国内时间服务器，以获取正确的时间回应，从而解决网络受限的问题

{% hint style="danger" %}
**注意**：此方法不可用于游戏联网(如VRChat)，如需游戏联网，请参照[虚拟网卡+热点篇](udp-hotspot/)
{% endhint %}

#### 阿里云时间服务器地址

```
203.107.6.88 ntp.aliyun.com
120.25.115.20 ntp1.aliyun.com
```

#### Oculus请求的DNS地址

```
connectivitycheck.gstatic.com
time.facebook.com
www.google.com
oculus.com
graph.oculus.com
mqtt-mini.facebook.com
in.appcenter.ms
graph.facebook-hardware.com
graph.facebook.com
```

## 修改路由器hosts

### 一般市售路由器

{% hint style="info" %}
各品牌路由器设置不一样，需要自行查找修改方法
{% endhint %}

<mark style="color:red;">首先打开路由器的ssh功能</mark>

然后按下电脑上的**`Win+R`**键，输入**`cmd`**打开命令提示符

输入以下命令，回车并输入密码，连接至路由器

```
ssh 路由器用户名@路由器IP
```

然后输入以下命令，添加Facebook的时间服务器解析

```
sed -i '$a 120.25.115.20 time.facebook.com' /etc/hosts
```

查看是否修改成功

```
cat /etc/hosts
```

### 软路由

网络设置>DHCP/DNS设置底部>自定义劫持域名>填写<mark style="color:blue;">Facebook NTP域名</mark>与<mark style="color:blue;">阿里云NTP的IP</mark>

### 代理设置

将Facebook的NTP服务器地址修改解析完成后，把梯子软件的允许局域网连接打开，然后在Quest2连接WiFi输入密码的界面，打开高级选项

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/quest/wifi1.jpg)

将**代理**改为**手动**，把电脑代理软件的IP和端口输入进去，再进行连接即可

<figure><img src="https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/quest/wifi_proxy.jpg" alt=""><figcaption></figcaption></figure>

## 各个方案

### 路由器一体化

购买支持梯子的路由器，在路由器端挂梯子联网

### 路由器解析+电脑代理

修改路由器的hosts解析地址，并使用电脑梯子软件的局域网代理

### 路由器解析+手机代理

同理，使用手机梯子软件的局域网代理

### 手机解析+手机代理

根据原理，修改手机的hosts解析，并使用手机热点，连接手机端梯子软件的局域网代理

因各品牌权限设置不一样，如何修改手机hosts解析请自行搜索

### 电脑修改host解析+电脑热点

<mark style="color:red;">此方案不可用，windows网络逻辑不允许设备通过热点使用本机代理连网，目前没有解决办法</mark>

如果需要使用电脑热点连网，请参照[虚拟网卡+热点篇](udp-hotspot/)，或使用<mark style="background-color:blue;">电脑热点+手机代理</mark>
