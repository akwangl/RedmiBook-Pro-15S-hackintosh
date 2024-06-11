# macOS on RedmiBook Pro 15S
## 配置

Type | Spec
:---------|:---------
Model Name | RedmiBook Pro 15S 2021
CPU | AMD Ryzen™ 7 5600H
RAM | 16 GB 3200 MHz DDR4
Wi-Fi | Intel® Wi-Fi 6 AX200
Audio | Realtek ALC256

## 安装时需要关闭的驱动

驱动 | 
:---------|
AirportItlwm |
IntelBluetoothFirmware |
IntelBluetoothInjector | 
IntelBTPatcher | 
BlueToolFixup | 
NootedRed | 

> 当系统完全安装完毕时（系统激活完毕）将以上关闭驱动再次打开，如果你是5800H只需要修改AMD内核补丁即可。当前`OpenCore 1.0.0`


## 虚拟化问题
目前仅只有Monterey（mac os 12.x）以下版本支持VirtualBox。我只是用来安装Debian然后在里面安装docker完成项目的编译打包工作（内存只需要分配300MB），当然如果你有更复杂的操作可以考虑买一块RK3399开发版来满足你的需求，这两者目前我都有使用。

> 如果你不考虑虚拟化可以使用最新版本系统，目前`12.x`是解决虚拟化问题的最后一个版本

## 睡眠问题
该款机器BIOS不支持S3睡眠，所以无法完成深度睡眠，使用上只是会更耗电。

