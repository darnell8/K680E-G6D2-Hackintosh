# K680E-G6D2-Hackintosh

|    硬件    |     型号      |   状态   |
| :--------: | :-----------: | :------: |
|    CPU     |    i3-8100    |  已睿频  |
|   图形卡   |     HD630     |  已驱动  |
|  图形卡2   |  GTX 1050Ti   |  已屏蔽  |
|    声卡    |    ALC269     |  已驱动  |
| Wi-Fi&蓝牙 | Dell 1820A |  已驱动  |
|    USB     |               |  ?  |
|    睡眠    |               | ~~正常~~ |
|   FN映射   |               | ~~正常~~ |
|   显示器   |               | ~~正常~~ |
|   触摸板   |               |   正常   |

### 前言
使用黑苹果最大的目的是避免安装一些国产的软件，另外也希望转到macOS平台带来更好的电池续航和开发效率。
目前工作续航两个小时

### TODO:
- 睡眠模式会睡死（指睡眠变重启）
- 亮度调节无法使用FN快捷键
- USB是否定制？
- 续航问题
    - 目前来看CPU频率无法降到1GHz以下，观测到Windows平台也是如此。正在寻找解决方案

### 已修复
- 主板时间问题
    - 系统板维护的时间称为RTC（实时时钟）。这是由主板上的小电池维护的时钟。Windows预计此时间表示当地时间，而OS X预计此时间表示UTC。
    - 出于所有实际目的，GMT和UTC是相同的，当地时间是相对于GMT/UTC的时间。RealTimeIsUniversal只是让Windows将BIOS/RTC时间视为UTC，就像OS X一样。
    - 尽管许多技术人员认为，默认情况下Windows期望BIOS时间为本地时间是愚蠢的，但为了向后兼容和99.9%的人不双启动，它被保留，并会对BIOS显示UTC与Windows显示本地时间感到困惑。
    - https://www.tonymacx86.com/threads/fix-incorrect-time-in-windows-osx-dual-boot.133719/

### 截图
- eul监控

![eul监控](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.11.04.png?raw=true)

- 桌面

![桌面](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.17.22.png?raw=true)

- 关于

![关于](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.18.04.png?raw=true)

![显示器](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.18.26.png?raw=true)

- 设置

![设置](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.19.07.png?raw=true)

- 电池

![电池](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.19.25.png?raw=true)

- 触控板

![触控板](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.20.27.png?raw=true)

- 随航

![随航](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.20.43.png?raw=true)

- 显示器

![随航](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.21.08.png?raw=true)

- 音量

![音量](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-17%20%E4%B8%8B%E5%8D%8811.21.32.png?raw=true)

- 额外的截图

![TRIM支持](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.15.09.png?raw=true)

![图形卡设备](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.21.04.png?raw=true)

![摄像头设备](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.22.07.png?raw=true)

![电池设备](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.35.26.png?raw=true)

![蓝牙设备](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.37.15.png?raw=true)

![WiFi设备](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.38.45.png?raw=true)

![CPU睿频](./ScreenShot/%E6%88%AA%E5%B1%8F2023-06-19%2022.46.38.png?raw=true)