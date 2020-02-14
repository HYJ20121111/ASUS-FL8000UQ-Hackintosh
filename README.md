# ASUS-FL8000UQ-Hackintosh For MacOS Catalina

## 配置：

|    配置       |        型号                 |
| ------------ | --------------------------- |
|    处理器     |          i7 8550U           |
|     核显      |          UHD620             |  
|     独显      |        940MX（已禁用）        |
|     内存      |  4G/4G 海力士DDR4 2400MHz    | 
|     硬盘      |       120G SSD/1T HDD       | 
|     声卡      |           ALC294            | 
|   无线网卡     |        BCM94360CD四天线      | 

## 正常工作
1. CPU变频
2. 核显硬件加速，独显无法驱动已做屏蔽
3. 声卡输出（自编译AppleALC驱动）
4. HDMI输出
5. USB
6. WIFI/蓝牙(已更换BCM94360CD,原装AR9565可驱动,有需要可去远景论坛查找）
7. 电量显示正常
8. 触控板
9. 睡眠和唤醒

## 注意事项
1.经多人测试，本机型最新版BIOS-309无法安装黑苹果，需要将BIOS降级到老版本: [BIOS降级教程](http://bbs.pcbeta.com/viewthread-1841246-1-1.html)  
2.安装完成后请重新定制USB以解决睡眠问题：[USB定制教程](https://blog.daliansky.net/Intel-FB-Patcher-USB-Custom-Video.html)  
3。不要使用Fn+F1进行睡眠，否则将无法唤醒，只能重启。

## 感谢[黑果小兵的部落阁](https://blog.daliansky.net/)镜像及文章的帮助
## 感谢[acidanthera](https://github.com/acidanthera/AppleALC)的AppleALC源码
