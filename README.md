# HP-15-dc1061tx-hackintosh
暗影精灵5 ｜ macOS Sequoia 15.0.1  ｜ OpenCore 1.0.2 ｜ hackintosh

## 前言
暗影精灵5的OC文件在作者更新到macOS Monterey/Ventura后便停止维护了。本仓库在原分支基础上更新OC至1.0.2版本，并对蓝牙和wifi做了一定调整以便在Sequoia上能稳定运行。

感谢[BobMaster's Blog](https://blog.hibobmaster.com/2020/10/26/hp-15-dc1010nr-hackintosh/comment-page-6/)的分享。

电脑配置以及OC相关的配置信息，这里不赘述。可以移步[传送门](https://blog.hibobmaster.com/2020/10/26/hp-15-dc1010nr-hackintosh/comment-page-6/)查看。

## 正常的

1. 核显加速成功
2. 睡眠
3. 电池
4. 扬声器、麦克风、摄像头
5. 有线、蓝牙
6. 无线（由于AirportItlwm驱动在Sequoia上尚未支持，目前的解决办法是[itlwm](https://github.com/OpenIntelWireless/itlwm) 和  [HeliPort](https://github.com/OpenIntelWireless/HeliPort/releases/download/v1.5.0/HeliPort.dmg)联合的方式来使用WIFI功能）
7. 触控板手势以及物理按键(手势等支持的不是特别好，强烈建议外接鼠标和键盘使用或等VoodooPS2后续更新)
8. NVME 和 Sata Trim 支持

## 异常的
1.dp/hdmi貌似直连独显。使用核显需要在外接显示器时用type-c接口。如果外接显示器支持Type-C直连就更好了，省去转接。
2.无法直接操作键盘背光灯，但有个办法，在windwos系统下把背光灯激活成想要的模式，再之后切换到macOS中时，键盘背光是保留的。  

## 截图
![系统信息](https://github.com/user-attachments/assets/de2775ed-20b5-4087-b176-e631934d551c)

![蓝牙](https://github.com/user-attachments/assets/8613bf9d-2867-4ee4-9da2-bbe81590ef13)

![WIFI](https://github.com/user-attachments/assets/afd74f6b-a009-4782-a1bc-e4cd64e5c98e)

![OpenCore Version](https://github.com/user-attachments/assets/7c91c7be-9e70-4b25-89bc-6d35885096f6)
