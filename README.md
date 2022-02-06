# macOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

# BIOS设置：

- 关闭`SecureBoot`

- 关闭`FastBoot`

- 硬盘模式修改为`AHCI`

- DVMT修改为`64M`


## 一、配置：

|    配置       |        型号                 |
|--------------|-----------------------------|
|    处理器     |          i7-1065G7          |
|     核显      |    Intel lris Plus Graphics G7    |
|     独显      |      MX330（已屏蔽）    |
|     内存      |     8GB+4GB DDR4        |
|     硬盘      |       西数 512G SSD        |
|     声卡      |       Realtek ALC256        |
|   无线网卡     |        Intel Wireless-AC 9461      |

|             |                           |
|--------------|-----------------------------|
|   Mac模拟机型     |        MacBookPro 16,2      |
|   支持安装版本（已做测试）     |        Mac OS Catalina 10.15.7（19H2) ~ Mac OS  Monterey 12.2    |


`注意：我的机型没有带指纹识别，如果是带有指纹识别的同款机型则指纹不能用`


## 二、正常工作
1. Type-C、USB3.0，2.0接口和读卡器（HDMI未做测试）
2. 核显`Intel lris Plus Graphics G7`的硬件加速（独显`MX330`无法驱动已做屏蔽）
3. 声卡输出（alcid=5）
4. 耳机接口
5. 麦克风
6. WIFI/蓝牙
7. 电池
8. 触控板
9. 睡眠和唤醒

## 三、关于亮度键F4~F5的问题。

亮度键需直接按F4    F5 （需进系统偏好设置自行修改为F4  F5） 按 FN+F4    FN+F5  无效

注意：

除F4和F5外，其他功能键需和FN一起使用        

部分快捷键在Mac下无法使用，比如触摸板开关键F6

## 四、Bug
1.声音有概率`从 Windows 切换到 Mac OS`时 Mac OS 无声音 (` Windows`下的` Realtek`驱动若为` Windows`自带的HDA驱动则无此Bug）

2.~~电池显示容量和电池实际情况对不上~~ （已修复）

3.~~核显有一定概率开机跑完进度条后黑屏，需强制关机再开机即可正常使用~~（已修复）



## 五、注意事项
1.下载的EFI请替换其中的三码后再使用，防止出现冲突。  

2.默认开启跑码模式`-v`，可自行关闭 

3.如存在安装最新系统存在停留在还剩15分钟可先安装 `Mac OS Catalina 10.15.7（19H2)`然后再使用系统更新升级到最新系统

4.未进行USB定制，如有需要，请自行定制

5.使用 EFI for 19H2版本的升级到 12.1或12.2需去引导文件 `config.plist`里的Kernel开启`BlueToolFixup.kext`然后关闭`BrcmBluetoothInjector.kext`以确保12的蓝牙能正常使用

## 六、本机NVRAM在Mac下能正常使用，需通过开机按`Ctrl+Enter`选择默认启动盘。
