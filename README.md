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

macOS Monterey Version 12.4 **12.5**

如果使用Bigsur的话请自行修改文件(主要就更改一些WiFi与蓝牙相关的设置即可)

## Opencore与引导

- 使用Opencore 0.7.8 **0.8.2**
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
- USB：
    - 全部定制完成, USB3和USB2设备均可使用
- 硬盘：
    - 因为个人使用的硬盘对trim支持不好，所以将其功能关闭，具体事项可以参照我的博客--[链接](https://www.yuko233.top/2022/07/21/%25e9%2583%25a8%25e5%2588%2586%25e4%25b8%2589%25e6%2598%259fnvme%25e5%259b%25ba%25e6%2580%2581%25e5%259c%25a8opencore%25e4%25b8%258b%25e7%259a%2584trim%25e9%2597%25ae%25e9%25a2%2598%25e8%25a7%25a3%25e5%2586%25b3/)，如果你使用其他品牌的支持trim的固态请将其开启。

## 注意事项
- 开机时有可能出现f1，f2，f3等字样并卡住，请进入 bios 人工设置boot 路径为 EFI 文件夹内`OC/OpenCore.efi`文件。

## 感谢

- Apple
- [@Acidanthera](https://github.com/acidanthera)
- [@daliansky](https://github.com/daliansky)
- 以及其他未列出的开发者