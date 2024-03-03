# CFW TAP模式

首先参照前面的教程设置好你的CFW客户端\
然后在**`General`**菜单中找到**`TAP Device`**选项，点击**`Manage` > `Install`**

安装完成后在网络适配器中应新增一个名为**`cfw-tap`**的设备

然后在**`General`**页面找到**`Mixin`**，点击右边的齿轮

将下面的代码粘贴进去

```yaml
mixin: #object
  dns:
    enable: true
    listen: 0.0.0.0:53
    enhanced-mode: redir-host
    nameserver:
    - 119.29.29.29
    - 223.5.5.5
    - 223.6.6.6
```

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash\_mixin.png)

点击右下角保存，将**`Mixin`**开关打开

打开**`控制面板` > `网络和 Internet` > `网络和共享中心` > 左侧`更改适配器设置`**，找到名称为**`cfw-tap`**的适配器，如果显示已启用，说明tap模式成功开启
