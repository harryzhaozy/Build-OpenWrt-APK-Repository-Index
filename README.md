# Build-OpenWrt-APK-Repository-Index
由于master.dl.sourceforge.net的passwall更新慢，25以上的X86的可能使用以下方法更新
# 在 OpenWrt 路由器的 /etc/apk/repositories.d/customfeeds.list 中写上：
https://harryzhaozy.github.io/Build-OpenWrt-APK-Repository-Index/packages.adb
在openwrt上执行：
  # 1. 将你的公钥直接保存为 private-key.pem.pub
curl -sL "https://raw.githubusercontent.com/harryzhaozy/Build-OpenWrt-APK-Repository-Index/main/apk.pub" -o /etc/apk/keys/private-key.pem.pub

# 2. 赋予正确的读取权限
chmod 644 /etc/apk/keys/private-key.pem.pub
