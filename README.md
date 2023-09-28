# Actions-OpenWrt

## 本项目包含3个构建Action

### lean-openwrt
[lean源码](https://github.com/coolsnowwolf/lede) 构建的 x86_64 固件. 

workflows: [https://github.com/day4742/Actions-OpenWrt/blob/master/.github/workflows/build-openwrt-Lean.yml)

config：[https://github.com/day4742/diy/blob/master/config-x86-Lean)

DIY 脚本：[https://github.com/day4742/diy/blob/master/diy-x86-Lean.sh)


##### 默认登陆:192.168.5.1, 密码:password ,默认4个网口，第1个到第3个网口为lan口,第4个网口为wan口





如需修改默认配置比如定制插件等，请编辑 `workflow` 文件，修改`SSH_ACTIONS`环境变量的值`false`修改为`true`。在触发工作流程后，在 Actions 页面等待执行到SSH connection to Actions步骤，复制 SSH 连接命令粘贴到终端内，连接到 GitHub Ac­tions 虚拟服务器环境。执行：`cd openwrt && make menuconfig` 编译配置。

