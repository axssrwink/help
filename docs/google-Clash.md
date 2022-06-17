# 仅代理浏览器-Clash

- - -

Chrome 浏览器搭配 Proxy SwitchyOmega 扩展使用是非常方便的，此方案需要配合 Clash 客户端使用，并需要禁用 Clash 客户端的“启用系统代理”。

 **须知：**

>1.在开始下面的教程前的请确保 Clash 客户端已经配置好，如果没有请参考：

- [在 Windows 中配置 Clash 客户端](https://axssr.cc/user/tutorial?os=Windows&client=Clash)

- [在 macOS 中配置 Clash 客户端](https://axssr.cc/user/tutorial?os=MacOS&client=Clash)


---

**1. 安装 SwitchyOmega**

通过 [Chrome 应用商店](https://chrome.google.com/webstore/detail/proxy-switchyomega/padekgcemlokbadohgkifijomclgjgif/related) 在线安装 ，  如果无法访问，也可以从 Github 直接下载安装包(自行查找)

在 Chrome 地址栏输入 chrome://extensions 打开扩展程序，拖动 .crx 后缀的 SwitchyOmega 安装文件到扩展程序中按提示进行安装。


**2. 配置 情景模式**

安装完成后会在 Chrome 浏览器右上角显示扩展程序的图标，如果你不想浏览器走代理可以选择“直接连接”。

下面开始为 SwitchyOmega 配置 Clash 代理。首先打开 SwitchyOmega 选项设置界面，如果有教程提示请选择跳过。

首先我们需要新建一个情景模式，命名为“SS”，并选择类型为 “代理服务器”，这个模式主要设置为全部都走 Clash 代理。

需要配置代理协议：SOCKS5，代理服务器：127.0.0.1，代理端口：7890

代理端口需要和上面 Clash 客户端配置的端口一样，默认情况下代理服务器地址都是 127.0.0.1

如果你有使用内网的需求可以在 “不代理的地址列表” 排除内网。可以查看上图中排除 192.168.0.* 整个网段。

配置完成后请记得 “应用选项” 保存配置。

完成后你可以在 SwitchyOmega 扩展程序菜单中选择刚刚配置好的SS情景模式即可仅浏览器通过代理。


**3. 测试代理**

使用 IP125.com 查看访问国内外时的 IP 地址。
- - -
注意事项：  
1. Clash不需要开启系统代理只需选择节点
2. 如果想正常使用，请记得在 SwitchyOmega 扩展程序菜单中选择系统代理或者直接连接 

