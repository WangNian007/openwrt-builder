# openwrt-builder
使用 OpenWrt ImageBuilder 快速构建可定制化的 OpenWrt 固件。

### 这是什么？

使用openwrt提供的 Image Builder 构建属于自己的固件。

### 本项目特点

* 使用 ImageBuilder 构建固件，省时省力，构建一次最多只需要不到半个小时。
* 内置了自己日常会用到的 Luci 软件包开箱即用。
* 内置了最新版本的 Clash 内核，无需自己下载。
* 内置开箱即用的 Docker 组件，无需复杂的配置。
* 只需简单修改 build.sh 即可二次构建属于你自己的固件，方便定制。

### 固件详情

固件上游：openwrt 24.10 分支

登录密码：root / password



### 使用方法

可以直接在 Release 页面下载编译完成的固件刷入使用。

如果你想添加或删除其他内置组件，只需 Fork 本仓库，修改 build.sh 然后进入 Actions 编译即可。如果想添加自定义的 ipk 包，则需要把 ipk 包的下载链接添加到 external-package-urls.txt 中，同时也需要在 build.sh 中添加对应的包名。

### 鸣谢

[OpenWrt](https://github.com/openwrt/openwrt/)

[GitHub Actions](https://github.com/features/actions)

[MyWrtBuilder](https://github.com/Revincx/MyWrtBuilder) 提供参考
