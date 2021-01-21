# 路由器激活\(推荐\)

{% hint style="warning" %}
请查看你所使用的线路是否支持UDP转发，如不支持请切换其他线路
{% endhint %}

## 老毛子路由器

{% page-ref page="../router/padavan.md" %}

进入科学上网插件

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/pdv/pdv2.png)

将**`游戏UDP中继服务器`**设置为**`与主服务相同`**  
**`运行模式`**设置为**`绕过大陆IP模式`**  
**`需要代理的端口`**设置为**`所有端口`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/pdv/pdv3.png)

{% hint style="danger" %}
请注意停止你的BT下载，否则可能会触发机场的封禁规则
{% endhint %}

将Quest链接至WIFI，正常激活

激活完成后推荐将设置调整为以下选项  
**`游戏UDP中继服务器`**设置为**`停用`**  
**`需要代理的端口`**设置为**`仅常用端口`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/pdv/pdv4.png)

## 梅林

{% page-ref page="../router/asuswrt.md" %}

连接至你的路由器WIFI，确保你路由器插件开启了**`游戏模式`**，即可正常激活

## 软路由

{% hint style="success" %}
既然你已经会折腾软路由了，那这点设置难不倒你
{% endhint %}

注意激活时将**`UDP转发`**打开，**`运行模式`**设为**`绕过大陆IP`**，**`代理端口`**设为**`所有端口`**

激活完成后关闭**`UDP转发`**，**`代理端口`**设为**`常用端口`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/openwrt/op1.png)

