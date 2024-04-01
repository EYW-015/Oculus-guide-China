# ❓ ※常见问题※

## 目录

* [#wang-luo-wen-ti](questions.md#wang-luo-wen-ti "mention")
  * [#ming-ming-neng-kan-youtube](questions.md#ming-ming-neng-kan-youtube "mention")
    * Quest2 WiFi显示**网络受限**
    * 头显固件更新卡在0%
    * 头显内应用商店无法访问
    * 头显无法下载游戏
    * 在线游戏无法联网
  * [#ke-yi-yong-shou-ji-re-dian-ji-huo-ma](questions.md#ke-yi-yong-shou-ji-re-dian-ji-huo-ma "mention")
  * [#gai-hosts-ye-neng-lian-wang-wei-shen-me-hai-gao-na-me-ma-fan](questions.md#gai-hosts-ye-neng-lian-wang-wei-shen-me-hai-gao-na-me-ma-fan "mention")
  * [#ti-zi-qu-na-li-zhao-you-mei-you-tui-jian](questions.md#ti-zi-qu-na-li-zhao-you-mei-you-tui-jian "mention")
  * [#yi-ding-yao-mai-lu-you-qi-ma](questions.md#yi-ding-yao-mai-lu-you-qi-ma "mention")
* [#quest-an-zhuang-ruan-jian](questions.md#quest-an-zhuang-ruan-jian "mention")
  * [#kai-fa-zhe-mo-shi](questions.md#kai-fa-zhe-mo-shi "mention")
  * [#tou-xian-an-zhuang-ruan-jian](questions.md#tou-xian-an-zhuang-ruan-jian "mention")（安装梯子
* [#meta-feng-hao](questions.md#meta-feng-hao "mention")
  * [#deng-lu-shou-bu-dao-shou-ji-yan-zheng-ma](questions.md#deng-lu-shou-bu-dao-shou-ji-yan-zheng-ma "mention")
* [#oculus-pc-duan-wen-ti](questions.md#oculus-pc-duan-wen-ti "mention")
  * [#ke-hu-duan-wu-fa-deng-lu](questions.md#ke-hu-duan-wu-fa-deng-lu "mention")
  * [#zen-me-gai-an-zhuang-lu-jing](questions.md#zen-me-gai-an-zhuang-lu-jing "mention")
* [#chuan-liu-tou-ping](questions.md#chuan-liu-tou-ping "mention")
  * [#virtual-desktop-wu-fa-lian-jie](questions.md#virtual-desktop-wu-fa-lian-jie "mention")
  * [#zen-me-yu-dian-nao-chuan-liu](questions.md#zen-me-yu-dian-nao-chuan-liu "mention")
  * [#air-link-wu-fa-lian-jie](questions.md#air-link-wu-fa-lian-jie "mention")
  * [#zen-me-tou-ping-zhi-qi-ta-she-bei](questions.md#zen-me-tou-ping-zhi-qi-ta-she-bei "mention")
* [#gou-mai-ruan-jian](questions.md#gou-mai-ruan-jian "mention")
  * [#ru-he-gou-mai-oculus-zheng-ban-you-xi](questions.md#ru-he-gou-mai-oculus-zheng-ban-you-xi "mention")
  * [#ke-yi-yong-yin-lian-ka-ma](questions.md#ke-yi-yong-yin-lian-ka-ma "mention")

## 网络问题

### 明明能看YouTube

* Quest2 WiFi显示**网络受限**
* 头显固件更新卡在0%
* 头显内应用商店无法访问
* 头显无法下载游戏
* 在线游戏无法联网

由于链接至Oculus设备服务需要**UDP数据传输**，请查询<mark style="color:red;">**线路**</mark>**以及**<mark style="color:red;">**联网方式**</mark>是否支持[**UDP转发**](quest-guide/basic-net.md)

### 可以用手机热点激活吗

不可以，未root的手机热点代理无法转发[**UDP数据包**](quest-guide/basic-net.md)，需要**电脑WIFI网卡**或购买**梯子路由器**

现在手机root困难，解锁都要申请，且root之后容易出问题，最直接的就是手机银行APP无法在root过的手机上使用

### 改hosts也能联网，为什么还搞那么麻烦

不推荐改hosts，原因查看[本页面](quest-use/oc-client/#yuan-li-jiang-jie)了解原理

### 梯子去哪里找，有没有推荐

查看[本页面](ready/proxy-server.md)寻找梯子

PS：作者只用过两三家梯子，没用过的也不好推荐，当前使用的虽然<mark style="color:green;">非常稳定</mark>且<mark style="color:green;">全线支持UDP</mark>，但<mark style="color:red;">价格较高</mark>，且<mark style="color:red;">无月付套餐</mark>，仅推荐有长期需求的用户购买

### 一定要买路由器吗

**不是必须的**，用软件方式进行联网也一样可以正常使用，当然路由器使用**更加方便**，但是一条**稳定的梯子线路**比路由器**重要的多**

## Quest安装软件

### 开发者模式

开发者模式怎么打开

先去申请VISA银行卡，根据[以下页面](quest-use/dev-sq.md)步骤绑定银行卡，并创建开发者组织

### 头显安装软件

可以在头显中安装梯子或安卓软件吗

开启开发者模式之后，可以在头显中安装标准安卓APK，在头显中安装梯子并进行联网，便无需使用梯子路由器/热点

{% content-ref url="quest-use/quest-client-inside.md" %}
[quest-client-inside.md](quest-use/quest-client-inside.md)
{% endcontent-ref %}

## **Meta封号**

Meta一注册就封号怎么办

查看[以下页面](ready/facebook-account.md#shen-su-liu-cheng)，根据说明进行申述解封，平均1-2天

### 登录收不到手机验证码

<div align="left">

<figure><img src=".gitbook/assets/int_msg_service.png" alt="" width="375"><figcaption></figcaption></figure>

</div>

## Oculus PC端问题

### 客户端无法登陆

明明能连Facebook登录，但还是显示请在浏览器中完成操作

Oculus Home无法使用系统代理，需要打开[Clash TUN模式](quest-guide/clash/clash-tun.md)联网

### 怎么改安装路径

查看[下方页面](quest-use/oc-client/#geng-gai-an-zhuang-lu-jing)，输入命令行修改安装目录

## 串流&投屏

### Virtual Desktop无法连接

* **`1.24.6`**版本之后加入了正版验证，需要头显端能访问外网环境进行验证

### 怎么与电脑串流

* [查看本页面](quest-use/stream.md#chuan-liu)

### Air Link无法连接

将<mark style="color:yellow;">**Oculus Home**</mark>与<mark style="color:yellow;">**头显系统**</mark>更新到最新版

### 怎么投屏至其他设备

* [查看本页面](quest-use/stream.md#tou-ping)

## 购买软件

### 如何购买Oculus正版游戏

绑定VISA银行卡，或使用PayPal进行购买，详情查看[本页面](quest-use/pay.md)

### 可以用银联卡吗

不可以，Oculus不支持银联卡，详细信息查看[下方页面](quest-use/pay.md)
