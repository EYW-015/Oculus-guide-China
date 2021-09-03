# Oculus PC客户端

## 更改安装路径

Oculus客户端默认安装路径是**C盘**，如果想安装到其他盘符，可按以下步骤操作

{% hint style="info" %}
确认目标硬盘有足够可用空间，且硬盘为NTFS格式分区，**不建议安装至机械硬盘内**
{% endhint %}

以**`管理员权限`**运行**`CMD`**，输入以下代码，回车

```text
<你的OC安装包路径>\OculusSetup.exe /drive=<目标安装盘符>
```

#### 范例

```text
C:\Users\USERNAME\Downloads\OculusSetup.exe /drive=D
```

## OC无法联网 / 登录

{% hint style="info" %}
由于OC客户端不能使用系统代理，无法使用标准系统代理方式联网，需要使用第三方软件进行应用代理，或开启虚拟网卡TAP模式进行OC客户端联网
{% endhint %}

如果你只开了梯子客户端的**系统代理**，就算开了**全局模式**，那也只是系统代理的全局模式，俗称**假全局**，所以OC客户端仍然无法连接至网络，便会出现诸如OC客户端无法安装，卡OC在登录界面无限转圈，或是FB认证失败等情况

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/ochome/och1.png)

