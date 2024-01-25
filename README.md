## 首次发布（2024-01-25）
### 由于本人有使用多台R68S机器，已经使用1年多，在本地机器上通过大量的编译，现稳定运行，最后发现固件也要不定期的更新，有些软件不更新体验不是那么好。于是决定在github上使用actions自动编译。
### 配制信息
- 默认的管理地址是：192.168.1.180（原因是使用场景为旁路由，所以把原有的192.168.1.1改成了192.168.1.180）
- 子网掩码：255.255.255.0
- 默认网关：192.168.1.1
- DNS：223.5.5.5 192.168.1.1
- linux kernel版本是6.1.x（会根据https://github.com/coolsnowwolf/lede.git版本的升级自动升级）

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
