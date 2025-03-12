# Scentrealm

## 气味小播(蓝牙版)

[蓝牙协议文档](https://github.com/Scentrealm/Bluetooth)

[相关 Demo](https://github.com/Scentrealm/Bluetooth/tree/main/demo/BluetoothDemo)

## 气味小播(Wi-Fi版)

> Wi-Fi 版本的小播依赖外网，通过 HTTP 协议进行通讯。
> 开发集成时需要联系商务开通 API key，并将相应设备的权限进行开通后方可使用。

[API 文档](https://github.com/Scentrealm/API)

## 气味脖戴(蓝牙版)

> 蓝牙版本的设备，统一采用相同的协议格式。

[蓝牙协议文档](https://github.com/Scentrealm/Bluetooth)

[SDK](https://github.com/Scentrealm/neck-scent-player/tree/main/BluetoothSDK)

[Demo](https://github.com/Scentrealm/neck-scent-player/tree/main/demo)

[本地测试工具](https://github.com/Scentrealm/neck-scent-player/tree/main/tools)

*BluetoothWearDemo（脖戴版本）.zip 解压后可以运行*

## 气味脖戴(433版)

> 433 无线通讯模块是一种常见的低功耗、短距离无线通讯模块，通常用于 IoT（物联网）设备和无线遥控系统中。它的工作频段为 433 MHz，适用于需要低数据传输速率和较短通讯距离的应用场景

[驱动安装](https://github.com/Scentrealm/neck-scent-player/tree/main/driver)

[Python SDK](https://github.com/Scentrealm/neckwearsdks)

[DLL](https://github.com/Scentrealm/neck-scent-player/tree/main/Scentrealm_bcc)

[UDP服务](https://github.com/Scentrealm/neck-scent-player/tree/main/%E8%84%96%E6%88%B4%E8%AE%BE%E5%A4%87UDP%E6%9C%8D%E5%8A%A1)

[Unity3d 接入？](https://github.com/Scentrealm/neck-scent-player/tree/main/Scentrealm_bcc)

*查看目录下 README.docx文档*

[在 PPT 中集成气味设备？](https://github.com/Scentrealm/scent-ppt)

*脖戴设备可以集成在 PPT 中，展示某个 PPT 页面，进行气味播放*

## 脖戴式气味设备接入说明

1. 准备硬件设备：window系统的电脑（win7及以上版本），气味控制器，气味设备（脖戴式设备）
2. 气味设备开机（绿灯慢闪），气味控制器连接到电脑上，控制器开机（红绿灯闪）
3. 电脑安装 driver/CP210x_Windows_Drivers.zip 驱动
4. win7系统可能需要安装vc_redist.x86.exe/vc_redist.x64.exe 程序，您可以先运行DllTest.exe程序进行测试，如果运行未报错，则无需安装
5. 导入 scentrealm_bcc.dll
6. 调用连接方法，连接控制器( Scentrealm_AutoConnectCTL/Scentrealm_ManualConnectCTL)
7. 调用唤醒方法，唤醒气味设备
8. 调用播放气味方法，控制设备播放气味（安装了料盒会出现对应的气味）
