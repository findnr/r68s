## 官网L大已经修复之前的问题了，现已可以正常编译，新一版本中加入了acme（此固件是自动续签https证书）（2024-03-30）
- 插件名称：luci-app-acme
## （2024-03-03和2024-03-10）这两次没有编译通过是因为新的passwall2中的插件编译时golang的版本要求1.22,但系统中是1.21,所以没有编译成功（2024-03-11）
- 具体的解决方案在github中有说，能不能成功就不知道了：https://github.com/coolsnowwolf/lede/issues/11921
- 我没有试，等主库更新。。。
## 2024-02-19更新
- 增加wan口均衡负载，多线多拨，单线多拨  luci-app-mwan3 luci-app-mwan3helper luci-app-syncdial
## 2024-02-04更新
- 固件存储14G太大了，编译出错。修改为5G
## 首次发布（2024-01-25）
### 本地机器上通过大量的编译，现稳定运行，最后发现固件也要不定期的更新，有些软件不更新体验不是那么好。于是决定在github上使用actions自动编译（初步每周周日更新）。
- 固件中已经编译docker,为了可以简便利用r68s 16G存储，我已在编译镜像时把硬盘的大小调了了14G
![image](https://github.com/findnr/r68s/assets/3909023/6e9c0d6d-8ad8-49ed-b1d2-59c807519a24)
![image](https://github.com/findnr/r68s/assets/3909023/cf2883bb-d047-40f1-91c5-d6f8e2446d6b)
### 本固件中还添加了ffmpeg ffprobe的支持、固件中有passwall2 helloworld istore,方便日常使用
![image](https://github.com/findnr/r68s/assets/3909023/0af5ecf4-8c21-401d-99de-c6453fa4454d)
![image](https://github.com/findnr/r68s/assets/3909023/949806b5-5a3e-46ff-9b1a-8ce69b7ff40d)
### 配制信息
- 默认的管理地址是：192.168.1.180（原因是使用场景为旁路由，所以把原有的192.168.1.1改成了192.168.1.180）
- 子网掩码：255.255.255.0
- 默认网关：192.168.1.1
- DNS：223.5.5.5 192.168.1.1
- linux kernel版本是6.1.x（会根据https://github.com/coolsnowwolf/lede.git版本的升级自动升级）
- 用户名：root
- 密码：password

##### 首先感谢大佬的开源项目，是在他们基础上构建出来的：
- https://github.com/coolsnowwolf/lede.git
- https://github.com/linkease/istore
- https://github.com/xiaorouji/openwrt-passwall-packages.git
- https://github.com/xiaorouji/openwrt-passwall2.git
- https://github.com/fw876/helloworld.git
![image](https://github.com/findnr/r68s/assets/3909023/b1363c8b-79d9-4123-a00f-90f8eb23d97f)
![image](https://github.com/findnr/r68s/assets/3909023/2cc58e49-3869-4274-8276-4067dd27b0aa)
![image](https://github.com/findnr/r68s/assets/3909023/17b54e4c-94a3-43d4-9c6b-ca198a50a44e)
![image](https://github.com/findnr/r68s/assets/3909023/a29ea381-a2f0-41b8-8195-e6891284bb7d)
![image](https://github.com/findnr/r68s/assets/3909023/cf465aa0-14ab-4d8b-8117-c175c9c87ca8)
![image](https://github.com/findnr/r68s/assets/3909023/c8fe8508-d682-4fca-8c0f-3b2877044924)
说明：如有侵权请及时联系删除
