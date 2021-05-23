# CFW TUN 模式

## CFW TUN模式

{% hint style="info" %}
对于不遵循系统代理的软件，开启 TUN 模式将在电脑设置一个虚拟网卡，接管其流量并交由 CFW 处理，在 Windows 中，TUN 模式性能比 TAP 模式好
{% endhint %}

### 安装TUN驱动

首先参照前面的教程设置好你的CFW客户端

进入网站[Wintun](https://www.wintun.net/)，点击界面中**`Download Wintun xxx`**下载压缩包，然后打开CFW的**`Home Directory`**目录

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_folder.png)

根据系统版本将对应目录中**`wintun.dll`**解压至**`Home Directory`**目录中。基于**`x64`**的处理器的**`64`**位操作系统请使用**`amd64`**版本，**`32`**位操作系统请使用**`x86`**版本

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_tun_dll.png)

然后在**`General`**菜单中找到**`Service Mode`**选项，点击**`Manage` &gt; `Install`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_tun_install.png)

### 设置并开启CFW TUN

进入**`Settings页面` &gt; `Profile Mixin` &gt; `YAML` &gt; `Edit`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_mixin_yaml.png)

将下面的代码粘贴进去

```yaml
mixin: # object
  dns:
    enable: true
    enhanced-mode: redir-host
    nameserver:
    - 119.29.29.29
    - 223.5.5.5
    - 223.6.6.6
  tun:
    enable: true
    stack: gvisor
    dns-hijack:
    - 198.18.0.2:53
    macOS-auto-route: true
    macOS-auto-detect-interface: true
```

修改好的配置文件应类似下图格式

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_mixin.png)

点击右下角保存，回到**`General`**页面，将**`Mixin`**开关打开

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称为**`Clash`**且描述为**`Clash Tunnel`**的适配器，如果显示已启用，说明tap模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_tun_adp.png)

