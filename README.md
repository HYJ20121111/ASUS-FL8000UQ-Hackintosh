# ASUS-FL8000UQ-Hackintosh For MacOS Mojave/Catalina

## 配置：

|    配置       |        型号                 |
|--------------|-----------------------------|
|    处理器     |          i7-8550U           |
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
## 如果clover开机出现ACPI Error，请删除ACPI/patch下的DSDT.aml  
## 一键开启HIDPI项目地址：[one-key-hidpi](https://github.com/xzhih/one-key-hidpi)
## 注意事项
1.经多人测试，本机型最新版BIOS-309无法安装黑苹果，需要将BIOS降级到老版本: [BIOS降级教程](http://bbs.pcbeta.com/viewthread-1841246-1-1.html)  
2.安装完成后请重新定制USB以解决无法睡眠问题：[USB定制教程](https://blog.daliansky.net/Intel-FB-Patcher-USB-Custom-Video.html)  
3.进入睡眠需要一分钟左右的时间，再此期间屏幕黑屏无法唤醒，等彻底进入睡眠后即可唤醒。
## HDMI注意事项
此电脑在BIOS中打开CSM兼容选项就可以在外接显示器中显示BIOS和Clover界面以及开机过程，但如果用外接显示器开机，那么黑苹果内屏将无法使用，但是10.14 Mojave中在clover里加上“igfxcflbklt=1”启动参数，开机后将笔记本盖子合上再打开即可同时使用内外屏，但注意，加上此启动参数后亮度调节将失效。此方法在10.15 Catalina中无效，所以建议10.15 Catalina不要打开CSM兼容模式，用内屏来开机，等黑苹果完全启动即可使用外屏。
## 关于睡眠过程中电脑自动唤醒解决方案
当电脑出现自动唤醒后，打开终端输入 log show --last 1d | grep "Wake reason" 找到唤醒电脑的设备，然后在DSDT中搜索对应的设备，将设备下面的_PRW方法注释掉即可。clover中的DSDT已注释GLAN和XDCI。

## 有问题可加QQ交流：211560569。

## 感谢[黑果小兵的部落阁](https://blog.daliansky.net/)镜像及文章的帮助
## 感谢[acidanthera](https://github.com/acidanthera/AppleALC)的AppleALC源码
## 感谢[xzhih](https://github.com/xzhih/one-key-hidpi)的一键开启HIDPI

## 截图
![1.png](https://github.com/KKKIIINNN/ASUS-FL8000UQ-Hackintosh/blob/master/screenshot/1.png)  
![2.png](https://github.com/KKKIIINNN/ASUS-FL8000UQ-Hackintosh/blob/master/screenshot/2.png)  
![3.png](https://github.com/KKKIIINNN/ASUS-FL8000UQ-Hackintosh/blob/master/screenshot/3.png)  
![4.png](https://github.com/KKKIIINNN/ASUS-FL8000UQ-Hackintosh/blob/master/screenshot/4.png)
