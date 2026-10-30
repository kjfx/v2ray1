# S-UI面板搭建教程，功能强大！支持Anytls，Hysteria2，Vless+Reality，TUIC协议等，s-ui怎么使用一键脚本搭建anytls

### 一、VPS购买：https://www.vultr.com/?ref=9827682
VPS服务器选择说明：[点击查看>>](https://raw.githubusercontent.com/kjfx/v2ray1/refs/heads/main/vps%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%80%89%E6%8B%A9%E8%AF%B4%E6%98%8E.png)

### 二、搭建工具下载
下载地址：https://kjfx.lanzoui.com/iqm6Uosbzha , 备用下载地址（含MAC版）：<a href="http://www.hostbuf.com/t/988.html" target="_blank">点击下载>></a>


### 三、搭建代码：
    bash <(curl -Ls https://raw.githubusercontent.com/alireza0/s-ui/master/install.sh)

### 四、准备工作（可选）
- 更新系统<br>
apt update && apt upgrade -y

- 安装 curl<br>
apt install curl -y

- 关闭防火墙：<br>
sudo ufw disable

- 查看防火墙状态：<br>
sudo ufw status

- 放行端口：<br>
sudo ufw allow 80<br>
sudo ufw allow 443<br>
提示：80/443/S-UI面板对应的端口/节点端口需要放行，如果关闭防火墙了这一步可以忽略。

### 五、域名注册解析教程：[点击查看>>](https://youtu.be/3rRZY0-CH0E)


### 六、使用客户端下载
Windows（v2rayN）：[点击下载>>](https://github.com/2dust/v2rayN/releases/latest/download/v2rayN-windows-64.zip)<br>
Android（v2rayNG）：[点击下载>>](https://github.com/2dust/v2rayNG/releases/download/2.3.11/v2rayNG_2.3.11_arm64-v8a.apk)<br>
IOS（shadowrocket）：[https://github.com/kjfx/AppleID](https://github.com/kjfx/AppleID)

### 其它内容
REALITY 目标网站 SNI

    www.intel.com
    www.amd.com
    www.nvidia.com
    www.samsung.com
    www.microsoft.com
    www.amazon.com
