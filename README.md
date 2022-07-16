# OC-DELL-OptiPlex7040MICRO
Opencore EFI for Dell OptiPlex 7040 Micro

简体中文 | [English](/.github/README-en.md)
## 硬件规格
| 型号    | Dell OptiPlex 7040 Micro |
|----------|-------------------------|
| CPU      | i5-6500T                |
| 核显     | HD530                   |
| 内存     | DDR4 2133 8+8           |
| 硬盘     | 三星960EVO 250GB (PCIE) |
| 板载声卡 | Realtek ALC255          |
| 无线网卡 | Intel AC8260            |
| 网口     | Intel I219-LM           |

## 测试成功的系统

macOS Monterey Version 12.4

如果使用Bigsur的话请自行修改文件(主要就更改一些WiFi与蓝牙相关的设置即可)

## Opencore与引导

- 使用Opencore 0.7.8
- BlueToolFixup最新版在我的机器上无法使用, 回退到2.6.2

## 使用前须知

- 请解锁 CGF lock 并调整 DVMT, 教程可以参照[此链接](https://github.com/optiplex-osx/Dell-OptiPlex-7040-Clover-EFI%0A)
- 我个人并没有使用 OSX + Win 的搭配, 如果造成Win的问题请自行解决
- 我并未使用HDMI接口, 如需要使用请自行定制
- 使用前请更新序列号
- 如转载或定制请注明来源

## 工作情况

- CPU：
    - 正常工作
    - 正常变频
    - 温度正常
- 板载声卡：
    - 正常工作
    - 支持耳机、内置扬声器输出
- 核芯显卡：
    - 正常工作
    - 支持DP输出
- 蓝牙：
    - 正常工作
- 无线网卡：
    - 正常工作
    - 隔空投送、随航因为Intel网卡限制无法使用, 但有线连接可以随航
- 睡眠：
    - 情况不知, 个人习惯是设置电脑不睡眠
- USB:
    - 全部定制完成, USB3和USB2设备均可使用

## 感谢

- Apple
- [@Acidanthera](https://github.com/acidanthera)
- [@daliansky](https://github.com/daliansky)
- 以及其他未列出的开发者