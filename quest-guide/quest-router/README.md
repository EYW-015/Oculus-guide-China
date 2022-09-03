# 路由器激活

{% hint style="danger" %}
激活头显需要你的**梯子线路**<mark style="color:red;">**支持UDP转发**</mark>，否则头显无法更新固件
{% endhint %}

## 老毛子路由器

低成本的路由器解决方案，性能一般，适合小白用户使用

{% content-ref url="padavan.md" %}
[padavan.md](padavan.md)
{% endcontent-ref %}

进入科学上网插件

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/pdv/pdv1.png)

将**`运行模式`**设置为**`全局模式`**\
**`游戏UDP中继服务器`**设置为**`与主服务相同`**\
**`需要代理的端口`**设置为**`所有端口`**

{% hint style="danger" %}
请注意停止你的BT下载，否则可能会触发机场的封禁规则
{% endhint %}

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/pdv/pdv3.png)

将Quest链接至WIFI，正常激活并更新

激活完成后将**`运行模式`**设置为**`绕过大陆IP模式`**\
将**`需要代理的端口`**设置为**`仅常用端口`**\
****将**`游戏UDP中继服务器`**设置为**`停用`**

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/pdv/pdv4.png)

## 梅林

折中的方案，WIFI性能强大，成本较高，适合对WIFI有需求的用户，需求无线串流的用户可考虑购买华硕

{% content-ref url="asuswrt.md" %}
[asuswrt.md](asuswrt.md)
{% endcontent-ref %}

连接至你的路由器WIFI，确保你路由器插件开启了<mark style="color:red;">**游戏模式**</mark>，即可正常激活更新

## 软路由

最折腾、最强大的路由器方案，功能最多，成本也较高，电脑小白直接跳过

{% hint style="success" %}
既然你已经会折腾软路由了，那这点设置难不倒你
{% endhint %}

{% content-ref url="ruan-lu-you.md" %}
[ruan-lu-you.md](ruan-lu-you.md)
{% endcontent-ref %}

注意激活时将**`运行模式`**设为**`全局模式`**\
**`游戏UDP中继服务器`**设置为**`与主服务相同`**\
**`代理端口`**设为**`所有端口`**

激活完成后将**`运行模式`**设置为**`绕过大陆IP模式`**\
将**`代理端口`**设为**`常用端口`**\
****将**`游戏模式UDP中继服务器`**设置为**`停用`**

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/openwrt/op1.png)
