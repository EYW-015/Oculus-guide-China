# 华硕路由器+梅林固件

## 简介

华硕路由器**WIFI信号较好**，使用简单，但成本较高，550起步，功能性及算力不如软路由

{% hint style="info" %}
由于硬路由CPU性能局限，外网速度慢是正常情况，对速度有需求请使用软路由
{% endhint %}

梅林固件支持的华硕路由器型号很多，查看支持型号及固件下载，请访问[**Koolshare 论坛**](https://koolshare.cn/forum.php)\*\*\*\*

## **梅林上网插件**

* [fancyss仓库](https://github.com/hq450/fancyss)

先到上方链接下载对应机型的上网插件，并将下载好的文件名改为`shadowsocks.tar.gz`

### 插件安装

路由器设置完成后进入路由器页面，左侧菜单找到**系统管理**，上方菜单进入**系统设置**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/merlin/merlin2.png)

找到**启用 SSH**选项，设置为**LAN only**，应用本页面设置

电脑运行**CMD命令提示符**，输入`ssh <路由器登录名>@<路由器IP地址>`回车，如出现密钥认证提示，输入`yes`并回车，然后输入你的**路由器登录密码**\(输入不显示，输入正确回车即可\)

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/merlin/merlin3.png)

当出现最后两行样式，说明你已经成功进入路由器SSH后台

复制以下代码，粘贴至**CMD**并敲下回车

```text
sed -i 's/\tdetect_package/\t# detect_package/g' /koolshare/scripts/ks_tar_install.sh
```

在左侧菜单最底部找到**软件中心**，并点击**更新**按钮

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/merlin/merlin1.png)

进入离线安装菜单，选择之前下载好的上网插件，上传并安装即可

### 插件使用

安装成功后回到软件中心主页，打开上网插件，会提示你添加节点，可以选择手动添加或订阅

{% hint style="info" %}
上网插件仅支持 SS / SSR / V2Ray 协议，且不支持SS订阅
{% endhint %}

在机场找到你的 SSR / V2 订阅地址，复制，进入上网插件中的**更新管理**页面

在第一大项中找到**规则更新**，点击**立即更新**

将订阅地址粘贴至**订阅地址管理**，订阅模式更改为**大陆白名单 / 游戏模式**，点击**保存并订阅**

回到账号设置，选择你需要使用的线路，将上方的**上网开关**打开，点击底部的**保存&应用**

如插件运行状态显示正常，即可正常使用

