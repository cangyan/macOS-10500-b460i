# macOS-10500-b460i
- opencore 0.8.8
- ventura 13.1

---
## 硬件
| 类别 | 型号                            |
| ---- | ------------------------------- |
| CPU  | i5-10500                        |
| 主板 | rog strix b460i gaming          |
| 内存 | 海盗船 lpx ddr4 3000hz 16GB x 2 |
| 硬盘 | WD sn750 500G                   |
| 显卡 | Intel UHD Graphics 630          |
| 机箱 | inwin b1                        |


## 正常功能
- CPU睿频
- usb端口映射（背板USB3.0x6， 前置USB3.0x1）
- 集成显卡驱动正常（dp输出正常，hdmi输出正常）
- 板载无线网卡AX200(itlwm.kext临时方案)
- 板载蓝牙
- 音频(重新编译FakePCIID.kext)
- 睡眠

## 遇到的坑
- WIFI AirportItlwm.kext v2.2.0-alpha（e0f745e）能驱动但扫描/连接热点太慢改itlwm.kext临时方案
- 声卡仿冒问题。官方FakePCIID.kext太过老旧，需要重新编译
