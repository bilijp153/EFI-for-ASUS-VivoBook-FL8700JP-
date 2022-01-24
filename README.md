# macOS Catalina/Big Sur/Monterey for ASUS VivoBook FL8700JP

# BIOS设置：

- 关闭`SecureBoot`

- 关闭`FastBoot`

- 硬盘模式修改为`AHCI`


## 一、配置：

|    配置       |        型号                 |
|--------------|-----------------------------|
|    处理器     |          i7-1065G7          |
|     核显      |    Intel lris Plus Graphics G7    |
|     独显      |    GeForce MX330（已屏蔽）    |
|     内存      |     8GB+4GB DDR4        |
|     硬盘      |       西数 512G SSD        |
|     声卡      |       Realtek ALC256        |
|   无线网卡     |        Intel Wireless-AC 9461      |

注意：我的机型没有带指纹识别，如果是带有指纹识别的同款机型则指纹不能用


## 二、正常工作
1. Type-C和USB3.0 2.0接口 （读卡器未测试，估计可以使用）
2. 核显硬件加速，独显无法驱动已做屏蔽
3. 声卡输出（LayoutID=5）
4. USB
5. WIFI/蓝牙
6. 电池（电池容量显示不正常但使用正常）
7. 触控板
8. 睡眠和唤醒

## 三、关于亮度键F4~F5的问题。

亮度键需直接按F4 F5 按 FN+F4 FN+F5无效

注意：除F4和F5外，其他功能键需和FN一起使用

## 四、Bug
1.声音存在有时开机使用无声音问题

2.电池显示容量和电池实际情况对不上

## 五、注意事项
1.下载的EFI请替换其中的三码后再使用，防止出现冲突。  

2.默认开启跑码模式（-v），可自行关闭 

3.如存在安装最新系统卡还剩15分钟可先安装黑果小兵的10.15.7（19H2）然后使用系统更新升级到最新系统

4.如OpenCore中的Windows无法启动，可打开oc编辑器 Misc>Entries 下修改Windows启动项文件所在盘符路径或删除此项 前往 Misc>Security 将Scan Policy值设为0

## 六、本机NVRAM在Mac下不能正常使用，但能通过开机按Ctrl+Enter选择默认启动盘。
