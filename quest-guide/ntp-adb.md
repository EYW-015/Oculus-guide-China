# 🛠 告别UDP网络受限(激活后)

参考教程：[悟空的谷歌TV激活教程](https://didiboy0702.gitbook.io/wukongdaily/wan-ke-yun-ji-qiao/google-tv-xiu-gai-ntp-fu-wu-qi-di-zhi)

{% hint style="info" %}
只是以后WiFi不需要UDP支持，但外网还是要连的
{% endhint %}

首先你需要启用开发者模式，并安装SideQuest

{% content-ref url="../quest-use/dev-sq.md" %}
[dev-sq.md](../quest-use/dev-sq.md)
{% endcontent-ref %}

打开SideQuest并连接头显，在头显中选择**允许**电脑访问，点击SideQuest右上角的 **`Run ADB...`** > **`CUSTOM...`**

<div align="left">

<figure><img src="../.gitbook/assets/image (3).png" alt="" width="205"><figcaption></figcaption></figure>

</div>

在弹出的框中点击左侧的List Devices，如果列出了一串头显序列号，就是连接成功了，然后把下面的代码粘贴进去运行

<mark style="color:red;">**一行一行运行，别4行一起进去了**</mark>

```sh
//设置NTP服务器
adb shell settings put global ntp_server ntp3.aliyun.com
//打开WiFi可用性验证
adb shell settings put global captive_portal_mode 1
//关闭https模式
adb shell settings put global captive_portal_ues_https 0
//设置WiFi验证地址
adb shell settings put global captive_portal_http_url http://connect.rom.miui.com/generate_204
```

