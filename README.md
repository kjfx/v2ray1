# 2023最新一键搭建教程，支持V2ray、Xray节点等，操作简单，4K速度
V2ray节点搭建教程：▶ https://youtu.be/UWWlrj26G50

### 一、VPS购买：https://www.vultr.com/?ref=8753714

### 二、搭建工具下载
下载地址：https://kjfx.lanzoui.com/iqm6Uosbzha    备用下载地址（含MAC版）：<a href="http://www.hostbuf.com/t/988.html" target="_blank">点击下载>></a>


### 三、搭建代码：
    bash <(curl -Ls https://raw.githubusercontent.com/FranzKafkaYu/x-ui/956bf85bbac978d56c0e319c5fac2d6db7df9564/install.sh) 0.3.4.4
    
备用搭建代码（两个任意选择一个使用）

    bash <(curl -Ls https://raw.githubusercontent.com/FranzKafkaYu/x-ui/master/install.sh) 0.3.4.4
    
### 四、搭建完后，放行端口
    iptables -I INPUT -p tcp --dport 54321 -j ACCEPT
    iptables -I INPUT -p tcp --dport 443 -j ACCEPT
    iptables -I INPUT -p tcp --dport 80 -j ACCEPT

### 五、安装证书
    curl https://get.acme.sh | sh; apt install socat -y || yum install socat -y; ~/.acme.sh/acme.sh --set-default-ca --server letsencrypt

#### 申请证书方式1
    ~/.acme.sh/acme.sh  --issue -d 你的域名 --standalone -k ec-256 --force --insecure

#### 申请证书方式2
    ~/.acme.sh/acme.sh --register-account -m "${RANDOM}@chacuo.net" --server buypass --force --insecure && ~/.acme.sh/acme.sh  --issue -d 你的域名 --standalone -k ec-256 --force --insecure --server buypass

#### 申请证书方式3：
    ~/.acme.sh/acme.sh --register-account -m "${RANDOM}@chacuo.net" --server zerossl --force --insecure && ~/.acme.sh/acme.sh  --issue -d 你的域名 --standalone -k ec-256 --force --insecure --server zerossl

#### 安装证书：
    ~/.acme.sh/acme.sh --install-cert -d 你的域名 --ecc --key-file /etc/x-ui/server.key --fullchain-file /etc/x-ui/server.crt

### 翻墙软件下载
Windows（v2rayN）：https://github.com/2dust/v2rayN/releases/download/6.23/zz_v2rayN-With-Core-SelfContained.7z<br>
Android（v2rayNG）：https://github.com/2dust/v2rayNG/releases/download/1.8.5/v2rayNG_1.8.5.apk<br>
IOS（shadowrocket）：https://github.com/kjfx/AppleID<br>
